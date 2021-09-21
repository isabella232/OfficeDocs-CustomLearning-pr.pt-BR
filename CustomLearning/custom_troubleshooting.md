---
author: pkrebs
ms.author: pkrebs
title: Solucionar problemas com os caminhos de aprendizagem do Microsoft 365
ms.date: 02/10/2019
description: Saiba como solucionar problemas Microsoft 365 de aprendizado
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
ms.openlocfilehash: 2afaaf8291f284b641172e816c4a3946fa8145e8
ms.sourcegitcommit: 6005c2551bdea334767e6a056fdcb79533f2c858
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/21/2021
ms.locfileid: "59461140"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a>Solucionar Microsoft 365 de aprendizado

Aqui estão as dicas de solução de problemas para problemas que podem ocorrer com Microsoft 365 de aprendizado ou o Serviço de Provisionamento SharePoint Online.

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a>Como saber se você tem permissões de Administrador de Locatários

Entre no Serviço de Provisionamento SharePoint Online e o provisionamento personalizado Learning requer permissões de Administrador de Locatários. Se você estiver enfrentando problemas de logom com o serviço de provisionamento SharePoint Online, certifique-se de ter sido atribuído a função de administrador global. A solução De Learning requer permissões de Administrador de Locatário, também conhecidas como Office 365 função de Administrador Global. Veja como determinar se você foi atribuído à função Administrador Global.

1.  Entre em Office.com.
2.  Clique **em Administrador**
3.  Em **Usuários**, selecione **Usuários Ativos**
4.  Pesquisar seu nome
5.  Clique em seu nome nos resultados da pesquisa. Você deve ver Administrador global para sua função.

![Administrador global para função](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a>Se você não tiver a função de administrador global
- Encontre um Administrador Global em sua organização e faça com que essa pessoa entre no serviço ou faça com que ela atribua a função de administrador global a você.

## <a name="tenant-app-catalog-troubleshooting"></a>Solução de problemas de catálogo de aplicativos de locatários
O Learning exige que um Catálogo de Aplicativos seja provisionado no locatário de destino. A criação de um catálogo de aplicativos requer permissões de Administrador Global. Aqui estão as etapas de solução de problemas para problemas comuns do Catálogo de Aplicativos:

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a>Como saber se você tem um catálogo de aplicativos tenant 
Para começar, verifique se você tem permissões de administrador global. Consulte as etapas para permissões de Administrador de Locatários acima.

1. No Office 365, clique em **Admin**, clique na seta expandir >, clique em **Mostrar todos** os  >  **centros de** administração  >  **SharePoint**.
2. Clique **em Administrador Clássico SharePoint Catálogo de**  >  **Aplicativos**  >  **do Centro.**
3. Em **Aplicativos,** você deve ver um tile intitulado **Distribuir aplicativos para SharePoint**. Se você vir o azulejo, terá um Catálogo de Aplicativos de Locatários. Consulte a **seção Como garantir que você seja uma Colagem de Site...** abaixo. Se você não vir o azulejo, precisará criar um catálogo de aplicativos de locatário para seu locatário. Consulte a **seção Como criar um Catálogo de Aplicativos de Locatário** abaixo .

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a>Como garantir que você seja um Proprietário do Conjunto de Sites no Catálogo de Aplicativos de Locatários 
Para provisionar Microsoft 365 de aprendizado, você precisará ser um Proprietário do Conjunto de Sites no Catálogo de Aplicativos de Locatário. Veja como determinar se você é um Proprietário.

1. No Office 365, clique em **Admin**, clique na seta expandir >, clique em **Mostrar todos** os  >  **centros de** administração  >  **SharePoint**.
2. Clique **em Centro de SharePoint De** administração clássico e selecione o catálogo de **aplicativos**.
3. Selecione **Proprietário** e, em seguida, verifique se você é um Proprietário do Conjunto de Sites. Deve se parecer com isso.
 
![Proprietário do conjunto de sites](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a>Como criar um Catálogo de Aplicativos de Locatário se não existir 
1. Entre no Office 365 com sua conta de administrador do SharePoint Online.
2. Clique em **Administrador**.
3. Em **Centros de administração,** clique **em SharePoint**. 
4. Clique **em Catálogo de**  >  **Aplicativos.**
5. Clique **em Criar um novo site de catálogo de aplicativos** e clique em **OK**. 
6.  Insira as informações do Catálogo de Aplicativos. Talvez você queira incluir mais de um Administrador. A seguir, mostra um exemplo.  

![Concluir a inserção de informações para o catálogo de aplicativos](media/cg-appcatalogfinish.png)

7.  É isso. Você terminou. Mas antes de passar para o provisionamento Learning, você precisa esperar pelo menos 30 minutos para garantir que a criação do Catálogo de Aplicativos seja concluída. 

> [!IMPORTANT]
> Aguarde pelo menos 30 minutos após a criação do Catálogo de Aplicativos de Locatário antes de provisionar a Learning. Isso garante que o processo de provisionamento do Catálogo de Aplicativos seja concluído SharePoint. 