---
author: pkrebs
ms.author: pkrebs
title: Configuração de Web Part autônoma
ms.date: 02/10/2019
description: Aprendizagem personalizada para a configuração da Web Part manual do Office 365
ms.openlocfilehash: 650e6c12ebe8ca7fedc6edc107b5822c48ead99a
ms.sourcegitcommit: b6617bbbaee0784d6216e96052c2469f97cf51e9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2019
ms.locfileid: "30411871"
---
# <a name="stand-alone-web-part-setup"></a>Configuração de Web Part autônoma

O aprendizado personalizado oferece uma configuração manual de Web Part autônoma para as organizações que já têm um site de comunicação moderna do SharePoint Online estabelecido dedicado ao treinamento ou que apenas desejam configurar a Web Part de aprendizado personalizada por conta própria site de comunicação. Observe que a configuração manual requer experiência que funcione com o Windows PowerShell e o Shell de gerenciamento do SharePoint Online. As etapas para uma configuração manual da Web Part de aprendizado personalizado da seguinte maneira:

- Valide se você atendeu a todos os pré-requisitos.
- Instale o arquivo customlearning. sppkg no catálogo de aplicativos do locatário do Office 365.
- ProVisione/identifique um site de comunicação moderna para atuar como seu aprendizado personalizado para o site do Office 365 Home.
- Execute um script do PowerShell que configurará seu locatário com os artefatos apropriados de que o aprendizado personalizado depende.
- Navegue até a página do site CustomLearningAdmin. aspx para carregar a Web Part de administração para inicializar a configuração de conteúdo personalizado.

> [!NOTE]
> Se você estiver procurando uma maneira rápida e fácil de configurar o aprendizado personalizado, confira proVisionar o [aprendizado personalizado](installsitepackage.md).

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

## <a name="step-4---set-permissions-for-the-site"></a>Etapa 4-definir permissões para o site
Verifique se as seguintes permissões estão definidas para o site:
- **Administrador do conjunto de sites ou parte do grupo proprietários** -permissões necessárias para inicializar o item de lista CustomConfig que configura o aprendizado personalizado para seu primeiro uso. 
- **Grupo de membros** – permissons necessário para administrar o aprendizado personalizado, incluindo ocultar e Mostrar conteúdo e administrar playlists personalizadas
- **Grupo de visitantes** -permissões necessárias para exibir o conteúdo do site. 

## <a name="step-5--execute-powershell-configuration-script"></a>Etapa 5: executar o script de configuração do PowerShell
Um script `CustomLearningConfiguration.ps1` do PowerShell é incluído, que você precisará executar para criar três [Propriedades de locatário](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties) que a solução usa. Além disso, o script cria duas [páginas de aplicativo de parte única](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages) na biblioteca de páginas do site para hospedar as Web Parts de administrador e usuário em um local conhecido.

### <a name="disabling-telemetry-collection"></a>Desabilitando a coleção de teleMetria
Parte dessa solução inclui consentimento de controle de telemetria anônimo, que por padrão é definido como ativado. Se você estiver executando uma instalação manual e quiser desativar o rastreamento de telemetria, altere o `CustomlearningConfiguration.ps1` script para definir a variável $optInTelemetry como $false.

Se você não estiver executando uma instalação manual e quiser desativar o rastreamento de telemetria, um script `TelemetryOptOut.ps1` separado foi incluído e, quando executado, o rastreamento de telemetria será desabilitado.

## <a name="step-6---initialize-web-part-custom-configuration"></a>Etapa 6-inicializar a configuração personalizada da Web Part
Após o script do PowerShell ser executado com êxito, navegue `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`até. Isso inicializa o item de lista **CustomConfig** que configura o aprendizado personalizado para seu primeiro uso.

A configuração já está concluída. Para saber mais sobre como personalizar o site de aprendizado personalizado e a Web Part para seu ambiente, consulte [Customize The Training Experience](custom_overview.md).

### <a name="next-steps"></a>Próximas etapas
- [Personalizar](custom_overview.md) a experiência de treinamento da sua organização.

