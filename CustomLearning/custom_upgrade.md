---
author: pkrebs
ms.author: pkrebs
title: Atualização de aprendizagem personalizada
ms.date: 02/10/2019
description: Aprendizagem personalizada para a configuração da Web Part manual do Office 365
ms.openlocfilehash: 72ac6f7a135697b816f2decbf010ec439562598f
ms.sourcegitcommit: e0adc8963419a4dd5c4d9bcc9f4f2cc1fbe291d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2019
ms.locfileid: "30523065"
---
# <a name="manual-upgrade-for-custom-learning"></a>Atualização manual para aprendizagem personalizada

O aprendizado personalizado para o Office 365 fornece um processo de atualização manual para organizações que participaram de pilotos mais antigos. Com o processo de atualização, as organizações podem continuar a usar seu site de aprendizado personalizado atual e atualizar adicionando a nova Web Part de aprendizado personalizado aprimorada ao seu catálogo de aplicativos do SharePoint e, em seguida, executando um script do PowerShell. O seguinte fornece uma visão geral do processo de atualização: 

- Validar que a pessoa responsável por carregar a nova Web Part e executar o script do PowerShell tem as permissões necessárias
- Carregue a Web Part, o arquivo customlearning. sppkg, para o catálogo de aplicativos do locatário do Office 365
- Executar um script do PowerShell que irá configurar seu locatário com os artefatos apropriados necessários para o aprendizado personalizado
- Navegue até a página CustomLearningAdmin. aspx no site de aprendizado personalizado para inicializar a configuração personalizada do ccontent.

## <a name="prerequisites"></a>Pré-requisitos
Para garantir uma atualização bem-sucedida do aprendizado personalizado, os pré-requisitos a seguir devem ser atendidos. 

- Você deve ter configurado um catálogo de aplicativos em todo o locatário. Se você não tiver um catálogo de aplicativos de locatário, confira [Configurar o locatário do Office 365](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) e siga a seção criar site de catálogo de aplicativos. 
- Se o catálogo de aplicativos de todo o locatário já tiver sido provisionado, você precisará ter acesso a uma conta que tenha direitos para carregar um pacote nele. Geralmente, esta é uma conta com a função de administrador do SharePoint. 
- Se uma conta com a função de administrador do SharePoint não funcionar: Vá para o centro de administração do SharePoint, selecione o catálogo de aplicativos, clique em proprietários e entre como um dos administradores de conjunto de sites ou adicione a conta de administrador do SharePoint que falhou ao site Lista de administradores de coleção. 

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>Etapa 1: obter o pacote de Web Part e o script de instalação do GitHub
Como parte do processo de instalação, você precisará do pacote de Web Part de aprendizado personalizado e do script de instalação do PowerShell.

1. Vá para o [repositório do GitHub de aprendizado personalizado](https://github.com/pnp/custom-learning-office-365).
2. Clique em **clonar ou baixar**e, em seguida, **Baixe zip**.   
3. Salve o arquivo **zip** em um local na sua unidade local.
4. Extraia o arquivo **zip** em sua unidade local.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>Etapa 2-carregar a Web Part no catálogo de aplicativos do locatário
Para configurar o aprendizado personalizado para o Office 365, você carrega o arquivo customlearning. sppkg no catálogo de aplicativos de todo o locatário e o implanta. Consulte [usar o catálogo de aplicativos para disponibilizar aplicativos de negócios personalizados para seu ambiente do SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) para obter instruções detalhadas sobre como adicionar um aplicativo ao catálogo de aplicativos.

1. No Office 365, clique em **administrador**.
2. Em **centros de administração**, clique em **SharePoint**.
3.  > Clique **** em**Catálogo** > **de aplicativos do aplicativo distribua aplicativos para SharePoint.**
4. Clique em **carregar** > **escolher arquivos**.
5. Na pasta onde você salvou o arquivo ZIP, selecione a pasta **WebPart** e, em seguida, selecione **customlearning. sppkg.**
6. Clique em **Implantar**.

## <a name="step-5--execute-powershell-configuration-script"></a>Etapa 5: executar o script de configuração do PowerShell
Um script `CustomLearningConfiguration.ps1` do PowerShell está incluído no download do zip no github. Você precisa executar o script para criar três [Propriedades de locatário](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties) que a solução usa. Além disso, o script cria duas [páginas de aplicativo de parte única](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages) na biblioteca de páginas do site para hospedar as Web Parts de administrador e usuário em um local conhecido. Essas páginas de aplicativos são:

- CustomAdministration. aspx
- CustomViewer. aspx

### <a name="to-run-the-powershell-script"></a>Para executar o script do PowerShell
- Usando o PowerShell, execute `CustomLearningConfiguration.ps1` o script localizado na pasta WEBPART do zip do github. Se tiver êxito, você verá três pares chave/valor e **administrador de aprendizado personalizado para desativar...** na janela de comando.

### <a name="disabling-telemetry-collection"></a>Desabilitando a coleção de teleMetria
O aprendizado personalizado inclui consentimento de controle de telemetria anônimo, que por padrão é definido como ativado. Se quiser desativar o rastreamento de telemetria, altere o `CustomlearningConfiguration.ps1` script para definir a `$optInTelemetry` variável como. `$false`

## <a name="step-6---initialize-web-part-custom-configuration"></a>Etapa 6-inicializar a configuração personalizada da Web Part
Após o script do PowerShell ser executado com êxito, navegue `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`até. Abrir **CustomLearningAdmin. aspx** Inicializa o item de lista **CustomConfig** que configura o aprendizado personalizado para o primeiro uso. Você verá uma página parecida com esta:

![CG-adminapppage. png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Adicionar proprietários ao site
Como administrador de locatários, é improvável que você seja a pessoa que personaliza o site, portanto, você precisará atribuir alguns proprietários ao site. Os proprietários têm privilégios administrativos no site para que eles possam modificar as páginas do site e remarcar o site. Eles também podem ocultar e mostrar o conteúdo fornecido por meio da Web Part de aprendizado personalizado. Eles também terão a capacidade de criar uma lista de reprodução personalizada e atribuí-las às subcategorias personalizadas.  

1. No menu **configurações** do SharePoint, clique em **permissões do site**.
2. Clique em **configurações de permissão avançadas**.
3. Clique em **aprendizagem personalizada para proprietários do Office 365**.
4. Clique em **novo** > **Adicionar usuários a este grupo**, adicione as pessoas que você deseja que sejam proprietários e clique em **compartilhar**.

A atualização já está concluída. Para saber mais sobre como personalizar o site de aprendizado personalizado e a Web Part para seu ambiente, consulte [Customize The Training Experience](custom_overview.md).

## <a name="upgrade-instructions-for-site-owners"></a>Instruções de atualização para proprietários de site
O aprendizado personalizado para o Office 365 introduziu uma variedade de aprimoramentos na Web Part. Trabalhar com a Web Part é abordado em detalhes na seção [Personalizar a experiência de aprendizagem](custom_overview.md) . Por enquanto, o proprietário do site deve:  

- Verifique se a Web Part de aprendizagem personalizada para Office 365 está disponível. 
- Substituir a Web Part existente em páginas com a nova Web Part
- Substitua os links que apontam para a Web Part antiga

### <a name="verify-the-custom-learning-for-office-365-web-part-is-available"></a>Verifique se a Web Part de aprendizagem personalizada para Office 365 está disponível
1.  No site de aprendizado personalizado, clique em **configurações**e, em seguida, clique em ***Adicionar uma página**.
2.  Clique no **+** ícone da página para adicionar uma Web Part e selecione a Web Part **aprendizado personalizado para o Office 365** . A página agora deve ser semelhante ao seguinte gráfico:

[CG-adminapppage. png](media/cg-adminapppage.png)
 
### <a name="replace-the-old-web-part-with-the-new-web-part"></a>Substituir a Web Part antiga pela Web Part nova
Antes de substituir a Web Part de aprendizado personalizada ou fazer alterações no site, recomendamos que você leia a documentação [Personalizar a experiência de aprendizagem](custom_overview.md) , conforme explica como usar a nova Web Part. 

Para atualizar o site de aprendizado personalizado, substitua as instâncias existentes da Web Part pela nova Web Part. Embora não possamos ter certeza de onde a Web Part foi adicionada, a orientação para os pilotos anteriores era adicionar a Web Part às seguintes páginas, portanto, procure substituir a Web Part nessas páginas:

- Get-started-with-Office-365. aspx
- Get-started-with-Microsoft-Teams. aspx
- Get-started-with-OneDrive. aspx
- Get-started-with-SharePoint. aspx

### <a name="replace-existing-links-to-the-web-part"></a>Substituir links existentes à Web Part
Com os aprimoramentos da nova Web Part, a forma de vincular a uma lista de reprodução foi alterada. Como parte da atualização, você deve substituir todos os links para a Web Part, incluindo itens de menu e links na página inicial. Antes de substituir a Web Part de aprendizado personalizada ou fazer alterações no site, recomendamos que você leia a documentação [Personalizar a experiência de aprendizagem](custom_overview.md) , conforme explica como usar a nova Web Part. 

## <a name="recreate-existing-playlists"></a>Recriar playlists existentes 
Para garantir que as listas de reprodução funcionem corretamente, qualquer lista de reprodução que tenha sido criada com a versão anterior da Web Part precisará ser recriada. Antes de excluir as listas de reprodução, faça uma lista das listas de reprodução e dos ativos associados para que você possa recriá-las facilmente com a nova Web Part de aprendizado personalizado. Faça uma cópia de uma lista de reprodução e, em seguida, exclua-a. Você pode usar o campo JSONData para fazer uma cópia do conteúdo de uma lista de reprodução antes de excluir. Isso facilitará a criação mais tarde.


1. No site de aprendizado personalizado, clique em**conteúdo do site**de **configurações** > . 
2. Selecione uma lista de reprodução, selecione as reticências, selecione **Editar**e copie o conteúdo do campo **JSONData** e salve no bloco de notas ou em um documento separado para referência posterior. Selecione **Cancelar**.
3. Selecione a lista de reprodução, selecione as reticências e, em seguida, selecione **excluir**.
4. Agora você está pronto para recriar a lista de reprodução com a nova Web Part.
Para obter instruções sobre como usar a Web Part de aprendizagem personalizada para o Office 365, consulte [personalizar a experiência de aprendizado (custom_overview. MD).

### <a name="next-steps"></a>Próximos passos
- [Personalizar](custom_overview.md) a experiência de treinamento da sua organização.

