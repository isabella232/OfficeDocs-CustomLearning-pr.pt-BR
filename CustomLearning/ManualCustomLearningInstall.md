---
author: pkrebs
ms.author: pkrebs
title: Caminhos de aprendizado da instalação manual
ms.date: 02/18/2019
description: Caminhos de aprendizado da instalação manual
ms.service: sharepoint online
ms.openlocfilehash: a9ae97bbafcc82c54251cae9a0ad658b7a0c16f4
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48234663"
---
# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>Instalando e Configurando manualmente o aprendizado personalizado para o Office 365

A Web Part de aprendizado personalizado da Microsoft é compilar usando a versão 1.7.1 da [estrutura do SharePoint](https://docs.microsoft.com/sharepoint/dev/spfx/sharepoint-framework-overview) .

Para instalar e configurar manualmente a Web Part e o conjunto de sites, você precisará concluir as seguintes etapas:

1. Valide se você atendeu a todos os pré-requisitos.
1. Instale o arquivo customlearning. sppkg no catálogo de aplicativos do locatário do Office 365.
1. Provisione/identifique um site de comunicação moderna para atuar como seu aprendizado personalizado para o site do Office 365 Home.
1. Execute um script do PowerShell que configurará seu locatário com os artefatos apropriados de que o aprendizado personalizado depende.
1. Navegue até a página do site CustomLearningAdmin. aspx para carregar a Web Part de administração para inicializar a configuração de conteúdo personalizado.

## <a name="prerequisites"></a>Pré-requisitos

Você deve ter configurado e configurado o catálogo de aplicativos de todo o locatário. Confira [Configurar o locatário do Office 365](https://docs.microsoft.com/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) e siga a seção criar site de catálogo de aplicativos. Se o catálogo de aplicativos de todo o locatário já tiver sido provisionado, você precisará ter acesso a uma conta que tenha direitos para carregar um pacote para concluir esse processo de instalação. Geralmente, esta é uma conta com a função de administrador do SharePoint. Se uma conta com essa função não funcionar, vá para o centro de administração do SharePoint e encontre os administradores do conjunto de sites para o conjunto de sites do catálogo de aplicativos e faça o logon como um dos administradores de conjunto de sites ou adicione a conta de administrador do SharePoint que falhou aos administradores do conjunto de sites. Você também precisará de acesso a uma conta que seja um administrador de locatários do SharePoint.

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>Carregar a Web Part no catálogo de aplicativos do locatário

Para configurar o aprendizado personalizado para o Office 365, você carrega o arquivo customlearning. sppkg no catálogo de aplicativos de todo o locatário e o implanta. Consulte [usar o catálogo de aplicativos para disponibilizar aplicativos de negócios personalizados para seu ambiente do SharePoint Online](https://docs.microsoft.com/sharepoint/use-app-catalog) para obter instruções detalhadas sobre como adicionar um aplicativo ao catálogo de aplicativos.

## <a name="provisionidentify-modern-communication-site"></a>Provisionar/identificar o site de comunicação moderna

Identifique um site de comunicação existente do SharePoint ou provisione um novo em seu locatário do SharePoint Online. Para obter mais informações sobre como provisionar um site de comunicação, consulte [criar um site de comunicação no SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) e siga as etapas para criar um site de comunicação.

## <a name="set-permissions-for-the-site"></a>Definir permissões para o site

Você desejará adicionar todos os usuários que devem ser capazes de exibir conteúdo para o grupo de visitantes e todos que possam administrar listas de reprodução personalizadas para o grupo de membros. Para configurar o site para aprendizado personalizado na primeira vez que o usuário deve ser um administrador de conjunto de sites ou parte do grupo de proprietários.

Adicione o aprendizado personalizado para o aplicativo do Office 365 ao conjunto de sites.

## <a name="execute-powershell-configuration-script"></a>Executar script de configuração do PowerShell

Um script do PowerShell `CustomLearningConfiguration.ps1` é incluído, que você precisará executar para criar três [Propriedades de locatário](https://docs.microsoft.com/sharepoint/dev/spfx/tenant-properties) que a solução usa. Além disso, o script cria duas [páginas de aplicativo de parte única](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/single-part-app-pages) na biblioteca de páginas do site para hospedar as Web Parts de administrador e usuário em um local conhecido.

### <a name="disabling-telemetry-collection"></a>Desabilitando a coleção de telemetria

Parte dessa solução inclui consentimento de controle de telemetria anônimo, que por padrão é definido como ativado. Se você estiver executando uma instalação manual e quiser desativar o rastreamento de telemetria, altere o `CustomlearningConfiguration.ps1` script para definir a variável $optInTelemetry como $false.

Se você não estiver executando uma instalação manual e quiser desativar o rastreamento de telemetria, um script separado foi incluído e, `TelemetryOptOut.ps1` quando executado, o rastreamento de telemetria será desabilitado.

## <a name="initialize-web-part-custom-configuration"></a>Inicializar a configuração personalizada da Web Part

Após o script do PowerShell ser executado com êxito, navegue até `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` . Isso inicializa o item de lista CustomConfig que configura o aprendizado personalizado para seu primeiro uso.

A configuração agora está concluída e você pode continuar usando o aprendizado personalizado para o Office 365. Confira a documentação do usuário para obter mais informações.