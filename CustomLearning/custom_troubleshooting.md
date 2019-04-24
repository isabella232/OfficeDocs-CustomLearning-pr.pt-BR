---
author: pkrebs
ms.author: pkrebs
title: Solucionando problemas de aprendizagem personalizada
ms.date: 02/10/2019
description: Saiba como solucionar problemas de aprendizado personalizado
ms.openlocfilehash: 7cbd049d4794d14f9e8cc26fd0db5f444812d688
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055074"
---
# <a name="troubleshoot-custom-learning"></a>Solucionar problemas de aprendizagem personalizada

Aqui estão dicas de solução de problemas que podem ocorrer com o aprendizado personalizado para o Office 365 ou o serviço de provisionamento do SharePoint Online.

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a>Como saber se você tem permissões de administrador de locatários

Entrar no serviço de provisionamento do SharePoint Online e provisionar o aprendizado personalizado requer permissões de administração de locatários. Se você estiver tendo problemas de entrada com o serviço de provisionamento do SharePoint Online, verifique se você recebeu a função de administrador global. A solução de aprendizado personalizada exige permissões de administrador de locatário, caso contrário, conhecida como função de administrador global do Office 365. ConFira aqui como determinar se você recebeu a função de administrador global.

1.  Entre no Office.com.
2.  Clique em **administrador**
3.  Em **usuários**, selecione **usuários ativos**
4.  Procurar seu nome
5.  Clique no seu nome nos resultados da pesquisa. Você deve ver administrador global para sua função.

![CG-globaladminrole. png](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a>Se você não tiver a função de administrador global
- Encontre um administrador global em sua organização e peça que a pessoa entre no serviço ou peça a ele para você atribuir a função de administrador global.

## <a name="tenant-app-catalog-troubleshooting"></a>Solução de problemas do catálogo de aplicativos do locatário
O aprendizado personalizado exige que um catálogo de aplicativos seja provisionado no locatário de destino. A criação de um catálogo de aplicativos requer permissões de administrador global. Veja a seguir as etapas de solução de problemas para problemas comuns do catálogo de aplicativos:

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a>Como saber se você tem um catálogo de aplicativos do locatário 
Para começar, verifique se você tem permissões de administrador global. Consulte as etapas das permissões de administrador de locatário acima.

1. no Office 365, clique em **administrador**, clique na seta para expandir >, clique em **mostrar todos os** > **centros** > de administração**do SharePoint**.
2. Clique em catálogo de**** > **aplicativos**de **Administração clássica do SharePoint Center** > .
3. Em **aplicativos**, você deve ver um bloco intitulado **distribuir aplicativos para SharePoint**. Se você vir o bloco, você tem um catálogo de aplicativos de locatário. Consulte a seção **como verificar se você é um site do Colllection..** . abaixo. Se você não vir o bloco, será necessário criar um catálogo de aplicativos de locatário para o locatário. Consulte a seção **como criar um catálogo de aplicativos do locatário** abaixo.

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a>Como garantir que você seja proprietário do conjunto de sites no catálogo de aplicativos do locatário 
Para provisionar o aprendizado personalizado para o Office 365, você precisará ser um proprietário do conjunto de sites no catálogo de aplicativos do locatário. Veja como determina se você é proprietário.

1. no Office 365, clique em **administrador**, clique na seta para expandir >, clique em **mostrar todos os** > **centros** > de administração**do SharePoint**.
2. Clique em **central de administração clássica do SharePoint**e selecione o **Catálogo de aplicativos**.
3. Selecione **proprietário**e, em seguida, verifique se você é um proprietário de conjunto de sites. Ele deverá ter uma aparência semelhante a esta.
 
![CG-sitecollectionowner. png](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a>Como criar um catálogo de aplicativos do locatário se não houver um 
1. Entre no Office 365 com sua conta de administrador do SharePoint Online.
2. Clique em **Administrador**.
3. Em **centros de administração**, clique em **SharePoint**. 
4. Clique em**Catálogo**de aplicativos de **aplicativos** > .
5. Clique em **criar um novo site de catálogo de aplicativos**e clique em **OK**. 
6.  Insira as informações para o catálogo de aplicativos. Talvez você queira incluir mais de um administrador. O exemplo a seguir mostra um exemplo.  

![CG-appcatalogfinish. png](media/cg-appcatalogfinish.png)

7.  É isso. Você concluiu. Mas antes de mudar para o provisionamento de aprendizado personalizado, você precisa aguardar pelo menos 30 minutos para garantir que a criação do catálogo de aplicativos esteja concluída. 

> [!IMPORTANT]
> Aguarde pelo menos 30 minutos depois de criar o catálogo de aplicativos do locatário antes de provisionar o aprendizado personalizado. Isso garante que o processo de provisionamento do catálogo de aplicativos seja concluído no SharePoint. 