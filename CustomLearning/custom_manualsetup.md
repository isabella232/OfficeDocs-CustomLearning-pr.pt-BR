---
author: pkrebs
ms.author: pkrebs
title: Learning configuração manual de caminhos
ms.date: 07/06/2020
description: Microsoft 365 configuração manual de caminhos de aprendizagem
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
ms.openlocfilehash: 7c6fc47336d354304164cebd95768a4bf97ee60f
ms.sourcegitcommit: 6005c2551bdea334767e6a056fdcb79533f2c858
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/21/2021
ms.locfileid: "59460959"
---
# <a name="learning-pathways-manual-setup"></a>Learning configuração manual de caminhos

Microsoft 365 de aprendizado oferece uma configuração manual para organizações que precisam de suporte para um dos seguintes cenários: 

- Sua organização tem um site de comunicação SharePoint Online dedicado ao treinamento e você deseja adicionar caminhos de aprendizado a esse site. Nesse cenário, a Web Part de caminhos de aprendizado não foi configurada no site.

- Você deseja instalar caminhos de aprendizado para suporte multilíngue em um dos sites de comunicação SharePoint da sua organização. O site tem ou terá um idioma padrão que não é inglês e é um dos idiomas suportados pelos caminhos de aprendizado. Aqui estão os idiomas suportados pelos caminhos de aprendizado:

- English
- Chinês (simplificado)
- Francês
- Alemão
- Italiano (Itália)
- Japonês (Japão)
- Português (Brasil)
- Russo (russo)
- Spanish

A configuração manual de caminhos de aprendizagem requer experiência trabalhando com Windows PowerShell e o Shell de Gerenciamento SharePoint Online. Aqui está uma visão geral das etapas para a configuração manual dos caminhos de aprendizado: 

- Valide se você atendeu a todos os pré-requisitos.
- Verifique as configurações de idioma padrão para seu site. Se OK, continue com a instalação manual. Se você precisar de uma configuração de idioma padrão diferente, precisará criar um novo site. 
- Instale o arquivo customlearning.sppkg no catálogo de aplicativos SharePoint locatário.
- Provisionar/identificar um site de comunicação moderno para atuar como seu site Microsoft 365 de aprendizado.
- Execute um script do PowerShell que configurará seu locatário com os artefatos dos quais os caminhos de aprendizado dependem.
- Navegue até a página de site CustomLearningAdmin.aspx para carregar a Web Part de administrador para inicializar a configuração de conteúdo personalizado.

## <a name="prerequisites"></a>Pré-requisitos
Para garantir uma configuração manual bem-sucedida da Web Part de caminhos de aprendizado, os seguintes pré-requisitos devem ser atendidos. 

- Você deve ter configurado e configurado o Catálogo de Aplicativos em todo o locatário. Consulte [Configurar seu locatário Office 365 e](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) siga a seção "Criar Catálogo de Aplicativos". 
- Se o Catálogo de Aplicativos de todo o locatário já tiver sido provisionado, você precisará de acesso a uma conta que tenha direitos para carregar um pacote para ele. Geralmente, essa conta tem uma SharePoint de administrador. 
- Se uma conta com essa função não funcionar, vá para o centro de administração do SharePoint e encontre os Administradores do Conjunto de Sites para o conjunto de sites catálogo de aplicativos e faça logon como um dos Administradores do Conjunto de Sites ou adicione a conta de administrador do SharePoint que falhou aos Administradores do Conjunto de Sites. 
- Você também precisará de acesso a uma conta que seja SharePoint administrador de locatários.

## <a name="step-1---check-your-language-settings"></a>Etapa 1 - Verificar as configurações do idioma
Como a primeira etapa do processo de instalação manual, verifique as configurações do idioma do site. Aqui estão as opções possíveis:

### <a name="option-1---you-dont-want-multilingual-support"></a>Opção 1 - Você não deseja suporte multilíngue
Se você não quiser suporte multilíngue para seu site, certifique-se de que ele está desligado.
1.  No site SharePoint de comunicação, selecione **Configurações** Informações do site Exibir todas as configurações do  >    >  **site**  >  **Configurações de idioma.** 
2.  De definir **a opção Habilitar páginas** e notícias a serem traduzidas para vários idiomas alternar para **Off**.
3.  Clique em **Salvar**. 
4.  Continue até a Etapa 2.

## <a name="option-2---you-want-multilingual-support-and-youre-ok-with-the-default-language"></a>Opção 2 - Você deseja suporte multilíngue e está ok com o idioma padrão
Um SharePoint de comunicação tem um idioma padrão. O idioma padrão determina o idioma no qual você visualiza os caminhos de aprendizado, incluindo a página Administração dos caminhos de aprendizado. A configuração de idioma padrão é definida quando o site é criado pela primeira vez e não pode ser alterado posteriormente. Antes de continuar com a configuração manual, verifique se você está ok com o idioma padrão do site de destino.

1.  No site SharePoint de comunicação, selecione **Configurações** Informações do site Exibir todas as configurações do  >    >  **site**  >  **Configurações de idioma.** 
2.  De definir **a opção Habilitar páginas** e notícias a serem traduzidas em vários idiomas alterna para **Ativado.**
    - Se você estiver ok com o idioma que aparece na parte superior da lista em **Idioma,** você pode adicionar idiomas adicionais e clique em **Salvar**. Continue até a Etapa 2.
    - Se você quiser um idioma padrão diferente do que foi selecionado para o site, você precisará criar um novo site de comunicação SharePoint com o idioma que deseja. Continue até a Opção 3. 

## <a name="option-3---you-want-multilingual-support-but-want-a-different-default-language-for-the-site"></a>Opção #3 - Você deseja suporte multilíngue, mas deseja um idioma padrão diferente para o site
Com essa opção, você cria um novo site de comunicação SharePoint Online com o idioma padrão que deseja e, em seguida, definir as configurações de idioma para o site. 
1.  Para criar um novo site SharePoint de comunicação, consulte [Create a communication site in SharePoint Online](https://support.microsoft.com/office/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb). Ao criar o site, certifique-se de definir o idioma como o idioma padrão que você deseja para caminhos de aprendizado. 
2. No site que você criou, selecione **Configurações** Informações do site Exibir todas as configurações  >    >  **do site**  >  **Configurações de idioma.** 
2.  De definir **a opção Habilitar páginas** e notícias a serem traduzidas em vários idiomas alterna para **Ativado.**
3. Adicione idiomas adicionais, se necessário, e clique em **Salvar**. 
4. Continue até a Etapa 2. 

>! [Observação] Se você precisar migrar conteúdo personalizado de um site para um site recém-criado, consulte a seção "Migrar Conteúdo Personalizado" posteriormente neste documento. 

## <a name="step-2---get-the-web-part-package-and-setup-script-from-github"></a>Etapa 2 - Obter o pacote de Web Part e o script de instalação GitHub
Como parte do processo de instalação, você precisará do pacote de Web Part de caminhos de Microsoft 365 de aprendizagem e do Script de Instalação do PowerShell.

- Vá para [os caminhos de aprendizado GitHub Repositório](https://github.com/pnp/custom-learning-office-365).
- Clique **em Baixar** para salvar o pacote e o script da Web Part em uma unidade local. Você estará usando o script e o pacote de Web Part nas etapas posteriores deste processo.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>Etapa 2 - Upload web part para o Catálogo de Aplicativos de Locatários
Para configurar Microsoft 365 de aprendizado, carregue o arquivo customlearning.sppkg no Catálogo de Aplicativos de todo o locatário e implante-o. Consulte [Usar o Catálogo](/sharepoint/use-app-catalog) de Aplicativos para disponibilizar aplicativos comerciais personalizados para seu ambiente SharePoint Online para obter instruções detalhadas sobre como adicionar um aplicativo ao Catálogo de Aplicativos.

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>Etapa 3 - Provisionamento/identificação de um site de comunicação moderno
Identifique um site de SharePoint de comunicação existente ou provisione um novo no seu locatário SharePoint Online. Para obter mais informações sobre como provisionar um site de comunicação, consulte [Create a communication site in SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) e siga as etapas para criar um site de comunicação.

## <a name="step-4---add-the-microsoft-365-learning-pathways-app-to-the-site"></a>Etapa 4 - Adicionar o aplicativo Microsoft 365 de aprendizado ao site

1. No site SharePoint, clique no menu Sistema e clique **em Adicionar um Aplicativo**. 
2. Em **Seus Aplicativos,** clique **em Da Sua Organização** e clique em caminhos de aprendizado **para** Office 365 . 

## <a name="step-5---set-permissions-for-the-site"></a>Etapa 5 - Definir permissões para o site
Verifique se as seguintes permissões estão definidas para o site:
- **Administrador do Conjunto** de Sites ou parte do grupo Proprietários - Permissões necessárias para inicializar o item de lista CustomConfig que configura os caminhos de aprendizado para seu primeiro uso. 
- **Grupo de** membros - permissões necessárias para Administrar caminhos de aprendizado, incluindo ocultar e mostrar conteúdo e administrar playlists personalizadas
- **Grupo visitantes** - permissões necessárias para exibir o conteúdo do site. 

## <a name="step-6--execute-powershell-configuration-script"></a>Etapa 6- Executar o Script de Configuração do PowerShell
Um script do PowerShell está incluído que você precisará executar para criar três propriedades `CustomLearningConfiguration.ps1` [de locatário](/sharepoint/dev/spfx/tenant-properties) que a solução usa. Além disso, o [](/sharepoint/dev/spfx/web-parts/single-part-app-pages) script cria duas páginas de aplicativo de parte única na biblioteca de páginas do site para hospedar as Web Parts do administrador e do usuário em um local conhecido.

1. Se você ainda não baixou o Shell de Gerenciamento SharePoint Online, baixe-o agora. Consulte [SharePoint Download do Shell de Gerenciamento Online](https://go.microsoft.com/fwlink/p/?LinkId=255251).
2. Talvez seja necessário definir uma política de execução do PowerShell para executar o script. Para obter mais informações, consulte [About Execution Policies](/powershell/module/microsoft.powershell.core/about/about_execution_policies).
3. Execute o `CustomLearningConfiguration.ps1` script. Além de suas credenciais de Administrador de Locatários, o script solicitará o nome do locatário e o nome do site. Considerando o exemplo a seguir para a URL do seu `https://contoso.sharepoint.com/sites/O365CL` site, , `contoso` é o nome do locatário e é `O365CL` o nome do site. 

### <a name="disabling-telemetry-collection"></a>Desabilitando a coleção telemetria
Parte dessa solução inclui a aceitação de rastreamento de telemetria anonimizada, que por padrão está definida como. Se você estiver fazendo uma instalação manual e quiser desativar o controle de telemetria, altere o script para definir a variável $optInTelemetry como $false e execute `CustomlearningConfiguration.ps1` o script.

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Validar o sucesso do provisionamento e inicializar a lista CustomConfig

Depois que o script do PowerShell for executado com êxito, navegue até o site, inicialize o item de lista **CustomConfig** que configura os caminhos de aprendizado para seu primeiro uso e valide que o site está funcionando.

- Saiba mais em `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`. Abrir o **CustomLearningAdmin.aspx** inicializa o item de lista **CustomConfig** que configura os caminhos de aprendizado para o primeiro uso. Você deve ver uma página com esta aparência:

![Página do aplicativo de administrador](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Adicionar proprietários ao site
Como Administrador de Locatários, é improvável que você seja a pessoa que personalização do site, portanto, você precisará atribuir alguns proprietários ao site. Os proprietários têm privilégios administrativos no site para que possam modificar páginas do site e renomear o site. Eles também têm a capacidade de ocultar e mostrar o conteúdo fornecido por meio da Web Part de caminhos de aprendizado. Além disso, eles terão a capacidade de criar playlist personalizada e atribuí-las a subcategorias personalizadas.  

1. No menu SharePoint **Configurações,** clique em **Permissões do Site.**
2. Clique **em Permissão Avançada Configurações**.
3. Clique **em caminhos de aprendizado para Office 365 Proprietários.**
4. Clique **em Novo** Adicionar Usuários a esse grupo e adicione as pessoas que você deseja que sejam  >  Proprietários. 
5. Adicione um link para [Explorar o Site](custom_exploresite.md) na mensagem Compartilhar e clique em **Compartilhar**.

## <a name="migrate-custom-content"></a>Migrar conteúdo personalizado
Depois de restabelecer seu site de caminhos de aprendizado seguindo as etapas acima, você precisará mover o conteúdo da sua lista **CustomPlaylists** e sua **lista CustomAssets.** Você também pode, opcionalmente, mover as páginas personalizadas reais que comem seus ativos personalizados se elas morarem no site de caminhos de aprendizado existentes, e sua intenção é excluí-la. A tarefa pode ser difícil porque, para todos os itens na lista **CustomPlaylists,** a ID do item de lista na lista **CustomAssets** é sepultada no campo JSONData de cada item de lista de playlist. Portanto, simplesmente mover o conteúdo da lista **CustomPlaylists** de um site para o outro não será suficiente. Além disso, **a lista CustomAssets** contém a URL absoluta para a página do ativo personalizado no campo JSONData do item de lista. Se os ativos não são movidos e o site não é renomeado (alterando a URL absoluta para a página do ativo), **CustomAssets** poderá permanecer. Mas você precisará corrigir manualmente as entradas. Dada a complexidade desse tipo de migração, sugerimos que você considere inscrever um de nossos parceiros de caminhos de aprendizado para ajudá-lo a fazer essa transição. 

### <a name="next-steps"></a>Próximas etapas
- Consulte [Personalizar caminhos de aprendizagem.](custom_overview.md) 
- Consulte [Traduzir páginas de site](custom_translate_page_ml.md).