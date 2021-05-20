---
author: pkrebs
ms.author: pkrebs
title: Manual Install Learning Pathways
ms.date: 02/18/2019
manager: bpardi
description: Manual Install Learning Pathways
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: 6f106b569602730f16fc2b6f8a09fa44667e32e1
ms.sourcegitcommit: 33acfc2149de89e8375b064b2223cae505d2a102
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52575966"
---
# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>Instalando e configurando manualmente o Aprendizado Personalizado para Office 365

A Web Part do Microsoft Custom Learning é construída usando o [Estrutura do SharePoint](/sharepoint/dev/spfx/sharepoint-framework-overview) versão 1.7.1.

Para instalar e configurar manualmente a Web Part e o conjunto de sites, você precisará concluir as seguintes etapas:

1. Valide se você atendeu a todos os pré-requisitos.
1. Instale o arquivo customlearning.sppkg no catálogo de aplicativos Office 365 locatário.
1. Provisionar/identificar um site de comunicação moderno para atuar como seu Custom Learning para Office 365 site.
1. Execute um script do PowerShell que configurará seu locatário com os artefatos apropriados dos quais o Aprendizado Personalizado depende.
1. Navegue até a página de site CustomLearningAdmin.aspx para carregar a Web Part de administrador para inicializar a configuração de conteúdo personalizada.

## <a name="prerequisites"></a>Pré-requisitos

Você deve ter configurado e configurado o Catálogo de Aplicativos em todo o locatário. Consulte [Configurar seu locatário Office 365 e](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) siga a seção Criar site de catálogo de aplicativos. Se o Catálogo de Aplicativos de todo o locatário já tiver sido provisionado, você precisará acessar uma conta que tenha direitos para carregar um pacote para concluir esse processo de instalação. Geralmente, essa conta tem a função SharePoint administrador. Se uma conta com essa função não funcionar, vá para o centro de administração do SharePoint e encontre os Administradores do Conjunto de Sites para o conjunto de sites do catálogo de aplicativos e faça logon como um dos Administradores do Conjunto de Sites ou adicione a conta de administrador do SharePoint que falhou aos Administradores do Conjunto de Sites. Você também precisará de acesso a uma conta que seja SharePoint administrador de locatários.

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>Upload web part para o Catálogo de Aplicativos de Locatários

Para configurar o Custom Learning para Office 365, carregue o arquivo customlearning.sppkg no Catálogo de Aplicativos de todo o locatário e implante-o. Consulte [Usar o Catálogo](/sharepoint/use-app-catalog) de Aplicativos para disponibilizar aplicativos comerciais personalizados para seu ambiente SharePoint Online para obter instruções detalhadas sobre como adicionar um aplicativo ao catálogo de aplicativos.

## <a name="provisionidentify-modern-communication-site"></a>Provisionamento/Identificar Site de Comunicação Moderna

Identifique um site de SharePoint de comunicação existente ou provisione um novo no seu locatário SharePoint Online. Para obter mais informações sobre como provisionar um site de comunicação, consulte [Create a communication site in SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) e siga as etapas para criar um site de comunicação.

## <a name="set-permissions-for-the-site"></a>Definir permissões para o site

Você deseja adicionar todos os que devem ser capazes de exibir conteúdo para o grupo Visitantes e todos os que devem ser capazes de administrar playlists personalizadas ao grupo Membros. Para configurar o site para Aprendizado Personalizado na primeira vez, o usuário deve ser um administrador de conjunto de sites ou parte do grupo Proprietários.

Adicione Custom Learning for Office 365 App ao conjunto de sites.

## <a name="execute-powershell-configuration-script"></a>Executar o Script de Configuração do PowerShell

Um script do PowerShell está incluído que você precisará executar para criar três propriedades `CustomLearningConfiguration.ps1` [de locatário](/sharepoint/dev/spfx/tenant-properties) que a solução usa. Além disso, o [](/sharepoint/dev/spfx/web-parts/single-part-app-pages) script cria duas páginas de aplicativo de parte única na biblioteca de páginas do site para hospedar as Web Parts do administrador e do usuário em um local conhecido.

### <a name="disabling-telemetry-collection"></a>Desabilitando a coleção telemetria

Parte dessa solução inclui a aceitação de rastreamento de telemetria anonimizada, que por padrão está definida como. Se você estiver executando uma instalação manual e quiser desativar o controle de telemetria, altere o script para definir a variável $optInTelemetry `CustomlearningConfiguration.ps1` como $false.

Se você não estiver executando uma instalação manual e quiser desativar o controle de telemetria, um script separado foi incluído que, quando executado, desabilitará o controle `TelemetryOptOut.ps1` de telemetria.

## <a name="initialize-web-part-custom-configuration"></a>Inicializar a configuração personalizada da Web Part

Depois que o script do PowerShell for executado com êxito, navegue até `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` . Isso inicializa o item de lista CustomConfig que configura o aprendizado personalizado para seu primeiro uso.

A configuração agora está concluída e você pode avançar com o uso do Custom Learning para Office 365. Consulte a documentação do usuário para obter mais informações.
