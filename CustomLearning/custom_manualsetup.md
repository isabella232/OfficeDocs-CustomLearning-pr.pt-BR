---
author: pkrebs
ms.author: pkrebs
title: Configuração de Web Part autônoma
ms.date: 02/10/2019
description: Aprendizagem personalizada para a configuração da Web Part manual do Office 365
ms.openlocfilehash: 8bf6292518c36eda74a49f9968c8e0559fcf8320
ms.sourcegitcommit: 5ea8d7fdc255ef7de06f41b3c794bc40551cf5bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30577847"
---
# <a name="stand-alone-web-part-setup"></a>Configuração de Web Part autônoma

O aprendizado personalizado oferece uma configuração manual de Web Part autônoma para as organizações que já têm um site de comunicação moderna do SharePoint Online estabelecido dedicado ao treinamento ou que apenas desejam configurar a Web Part de aprendizado personalizada por conta própria site de comunicação. Observe que a configuração manual requer experiência que funcione com o Windows PowerShell e o Shell de gerenciamento do SharePoint Online. As etapas para uma configuração manual da Web Part de aprendizado personalizado da seguinte maneira:

- Valide se você atendeu a todos os pré-requisitos.
- Instale o arquivo customlearning. sppkg no catálogo de aplicativos do locatário do Office 365.
- ProVisione/identifique um site de comunicação moderna para atuar como seu aprendizado personalizado para o site do Office 365 Home.
- Execute um script do PowerShell que configurará seu locatário com os artefatos apropriados de que o aprendizado personalizado depende.
- Navegue até a página do site CustomLearningAdmin. aspx para carregar a Web Part de administração para inicializar a configuração de conteúdo personalizado.

> [!NOTE]
> Se você estiver procurando uma maneira rápida e fácil de configurar o aprendizado personalizado, confira proVisionar o [aprendizado personalizado](custom_provision.md).

## <a name="prerequisites"></a>Pré-requisitos
Para garantir uma configuração manual bem-sucedida da Web Part de aprendizado personalizada, os pré-requisitos a seguir devem ser atendidos. 

- Você deve ter configurado e configurado o catálogo de aplicativos de todo o locatário. Confira [Configurar o locatário do Office 365](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) e siga a seção criar site de catálogo de aplicativos. 
- Se o catálogo de aplicativos de todo o locatário já tiver sido provisionado, você precisará ter acesso a uma conta que tenha direitos para carregar um pacote para concluir esse processo de instalação. Geralmente, esta é uma conta com a função de administrador do SharePoint. 
- Se uma conta com essa função não funcionar, vá para o centro de administração do SharePoint e encontre os administradores do conjunto de sites para o conjunto de sites do catálogo de aplicativos e faça o logon como um dos administradores do conjunto de sites ou adicione a conta de administrador do SharePoint que falharam nos administradores de conjunto de sites. 
- Você também precisará de acesso a uma conta que seja um administrador de locatários do SharePoint.

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>Etapa 1: obter o pacote de Web Part e o script de instalação do GitHub
Como parte do processo de instalação, você precisará do pacote de Web Part de aprendizado personalizado e do script de instalação do PowerShell.

- Vá para o [repositório do GitHub de aprendizado personalizado](https://github.com/pnp/custom-learning-office-365).
- Clique em **baixar** para salvar o pacote de Web Parts e o script em uma unidade local. Você usará o script e o pacote de Web Parts em etapas posteriores desse processo.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>Etapa 2-carregar a Web Part no catálogo de aplicativos do locatário
Para configurar o aprendizado personalizado para o Office 365, você carrega o arquivo customlearning. sppkg no catálogo de aplicativos de todo o locatário e o implanta. Consulte [usar o catálogo de aplicativos para disponibilizar aplicativos de negócios personalizados para seu ambiente do SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) para obter instruções detalhadas sobre como adicionar um aplicativo ao catálogo de aplicativos.

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>Etapa 3-proVisionar/identificar um site de comunicação moderna
Identifique um site de comunicação existente do SharePoint ou provisione um novo em seu locatário do SharePoint Online. Para obter mais informações sobre como provisionar um site de comunicação, consulte [criar um site de comunicação no SharePoint Online](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) e siga as etapas para criar um site de comunicação.

## <a name="step-4---add-the-custom-learning-for-office-365-app-to-the-site"></a>Etapa 4: Adicionar o aplicativo de aprendizado personalizado para o Office 365 ao site

1. No site do SharePoint, clique no menu sistema e, em seguida, clique em **Adicionar um aplicativo**. 
2. Em **seus aplicativos**, clique em **da sua organização**e, em seguida, clique em **aprendizado personalizado para o Office 365**. 

## <a name="step-5---set-permissions-for-the-site"></a>Etapa 5-definir permissões para o site
Verifique se as seguintes permissões estão definidas para o site:
- **Administrador do conjunto de sites ou parte do grupo proprietários** -permissões necessárias para inicializar o item de lista CustomConfig que configura o aprendizado personalizado para seu primeiro uso. 
- **Grupo de membros** – permissons necessário para administrar o aprendizado personalizado, incluindo ocultar e Mostrar conteúdo e administrar playlists personalizadas
- **Grupo de visitantes** -permissões necessárias para exibir o conteúdo do site. 

## <a name="step-6--execute-powershell-configuration-script"></a>Etapa 6: executar o script de configuração do PowerShell
Um script `CustomLearningConfiguration.ps1` do PowerShell é incluído, que você precisará executar para criar três [Propriedades de locatário](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties) que a solução usa. Além disso, o script cria duas [páginas de aplicativo de parte única](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages) na biblioteca de páginas do site para hospedar as Web Parts de administrador e usuário em um local conhecido.

1. Se você ainda não baixou o Shell de gerenciamento do SharePoint Online, baixe-o agora. ConFira [download do Shell de gerenciamento do SharePoint Online](https://go.microsoft.com/fwlink/p/?LinkId=255251).
2. Talvez seja necessário definir uma política de execução do PowerShell para executar o script. Para obter mais informações, consulte [sobre políticas de execução](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).
3. Executar o `CustomLearningConfiguration.ps1` script. Além de suas credenciais de administrador de locatário, o script solicitará o nome do seu locatário e o nome do site. Considerar o seguinte exemplo para a URL do seu `https://contoso.sharepoint.com/sites/O365CL`site `contoso` ,, é o nome `O365CL` do locatário e é o nome do site. 

### <a name="disabling-telemetry-collection"></a>Desabilitando a coleção de teleMetria
Parte dessa solução inclui consentimento de controle de telemetria anônimo, que por padrão é definido como ativado. Se você estiver executando uma instalação manual e quiser desativar o rastreamento de telemetria, altere o `CustomlearningConfiguration.ps1` script para definir a variável $optInTelemetry como $false e execute o script.

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Validar o êxito do provisionamento e inicializar a lista CustomConfig

Depois que o script do PowerShell for executado com êxito, navegue até o site, inicialize o item de lista **CustomConfig** que configura o aprendizado personalizado para seu primeiro uso e validar o site está funcionando.

- Acesse `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`. Abrir **CustomLearningAdmin. aspx** Inicializa o item de lista **CustomConfig** que configura o aprendizado personalizado para o primeiro uso. Você verá uma página parecida com esta:

![CG-adminapppage. png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Adicionar proprietários ao site
Como administrador de locatários, é improvável que você seja a pessoa que personaliza o site, portanto, você precisará atribuir alguns proprietários ao site. Os proprietários têm privilégios administrativos no site para que eles possam modificar as páginas do site e remarcar o site. Eles também podem ocultar e mostrar o conteúdo fornecido por meio da Web Part de aprendizado personalizado. Além disso, eles terão a capacidade de criar uma lista de reprodução personalizada e atribuí-las às subcategorias personalizadas.  

1. No menu **configurações** do SharePoint, clique em **permissões do site**.
2. Clique em **configurações de permissão avançadas**.
3. Clique em **aprendizagem personalizada para proprietários do Office 365**.
4. Clique em **novo** > **Adicionar usuários a este grupo**e adicione as pessoas que você deseja que sejam proprietários. 
5. Adicione um link para [explorar o site](https://docs.microsoft.com/en-us/Office365/CustomLearning/custom_explore) na mensagem de compartilhamento e clique em **compartilhar**.

### <a name="next-steps"></a>Próximos passos
- [Personalizar](custom_overview.md) a experiência de treinamento da sua organização.

