---
author: karuanag
ms.author: karuanag
title: Instalando a Web Part de solução de aprendizado personalizada
ms.date: 02/10/2019
description: Instruções de instalação para a Web Part de solução de aprendizado personalizada
ms.openlocfilehash: 53229e5b1b8175b06d888091963d1a9f2f0bd361
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989682"
---
# <a name="installing-the-custom-learning-solution-webpart"></a><span data-ttu-id="dbc92-103">Instalando a Web Part de solução de aprendizado personalizada</span><span class="sxs-lookup"><span data-stu-id="dbc92-103">Installing the Custom Learning Solution Webpart</span></span>

## <a name="prerequisites-for-a-tenant-wide-installation"></a><span data-ttu-id="dbc92-104">Pré-requisitos para uma instalação em todo o locatário</span><span class="sxs-lookup"><span data-stu-id="dbc92-104">Prerequisites for a tenant-wide installation</span></span>

- <span data-ttu-id="dbc92-p101">Para instalar o Web Part de aprendizado personalizado para o seu locatário inteiro, você precisará ter permissões administrativas do Office 365.  Se você não tiver essas permissões, poderá trabalhar com o administrador do Office 365 ou instalar a Web Part para um conjunto de sites individual.</span><span class="sxs-lookup"><span data-stu-id="dbc92-p101">To install the Custom Learning webpart for your entire tenant you will need to have Office 365 Administrative permissions.  If you do not have these permissions you can either work with your Office 365 Administrator or install the webpart for an individual site collection.</span></span>
- <span data-ttu-id="dbc92-107">Você ou seu administrador do Office 365 deve ter a configuração e configurado um [Catálogo de aplicativos](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) em todo o locatário ou um catálogo de aplicativos do [conjunto de sites](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)para receber a Web Part.]</span><span class="sxs-lookup"><span data-stu-id="dbc92-107">You or your Office 365 Administrator must have setup and configured a tenant-wide [App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) or a [Site Collection App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)to receive the webpart.]</span></span>
- <span data-ttu-id="dbc92-p102">Oferecemos suporte somente ao SharePoint Online. A Web Part não é compatível com a instalação em qualquer versão do SharePoint local.</span><span class="sxs-lookup"><span data-stu-id="dbc92-p102">We support SharePoint Online only. The web part is not support for installation on any version of SharePoint on premises.</span></span>

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a><span data-ttu-id="dbc92-110">Adicionar a Web Part de aprendizado personalizada ao seu locatário</span><span class="sxs-lookup"><span data-stu-id="dbc92-110">Add the Custom Learning webpart to your tenant</span></span> 

1. <span data-ttu-id="dbc92-p103">Baixe o Web Part de aprendizado personalizado e salve-o em sua unidade local.  Esse arquivo é chamado de "MS-Custom-Learning. sppkg".  Não altere o nome nem o sufixo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="dbc92-p103">Download the Custom Learning webpart and save it to your local drive.  This file is named "ms-custom-learning.sppkg".  Do not change the name or suffix of the file.</span></span> 
2. <span data-ttu-id="dbc92-114">Navegue até o [portal de administração do Office 365](https://admin.microsoft.com/AdminPortal/Home#/homepage) para o locatário</span><span class="sxs-lookup"><span data-stu-id="dbc92-114">Navigate to the [Office 365 Admin portal](https://admin.microsoft.com/AdminPortal/Home#/homepage) for your tenant</span></span>
3. <span data-ttu-id="dbc92-p104">Na navegação à esquerda, selecione centros de administração, SharePoint. Isso será aberto em uma nova guia. no centro de administração do SharePoint, selecione aplicativos, catálogo de aplicativos, aplicativos para SharePoint</span><span class="sxs-lookup"><span data-stu-id="dbc92-p104">From the left navigation select Admin Centers, SharePoint. This will open in a new tab. , In the SharePoint Admin Center select Apps, App Catalog, Apps for SharePoint</span></span> 
4. <span data-ttu-id="dbc92-117">Selecione carregar a Web Part e escolha o arquivo "MS-Custom-Learning. sppkg" que você baixou</span><span class="sxs-lookup"><span data-stu-id="dbc92-117">Select upload the webpart and choose the "ms-custom-learning.sppkg" file you downloaded</span></span>
5. <span data-ttu-id="dbc92-118">Para esta instalação em todo o locatário, marque a caixa ao lado de "tornar esta solução disponível para todos" na organização.</span><span class="sxs-lookup"><span data-stu-id="dbc92-118">For this tenant-wide installation check the box next to "Make this solution available to all sits in the organization."</span></span>  
 
> [!NOTE]
> <span data-ttu-id="dbc92-p105">Após instalar o WebPart, você o encontrará na Galeria de Web Parts no SharePoint Online.  **Na Galeria, a Web Part é chamada "Microsoft Learning"**</span><span class="sxs-lookup"><span data-stu-id="dbc92-p105">Once the webpart is installed you will find it in your webpart gallery in SharePoint Online.  **In the gallery the webpart is named "Microsoft Learning"**</span></span>

![Implantar solução](media/trustapp_sm.png)


## <a name="add-the-microsoft-learning-webpart-to-a-sharepoint-online-page"></a><span data-ttu-id="dbc92-122">Adicionar a Web Part do Microsoft Learning a uma página do SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="dbc92-122">Add the Microsoft Learning webpart to a SharePoint Online Page</span></span>

<span data-ttu-id="dbc92-p106">Após o aprendizado personalizado ser instalado em seu locatário, você pode adicionar a Web Part a uma página do SharePoint. Quando você faz o treinamento do Office 365 e do Windows 10 está disponível para seu site.</span><span class="sxs-lookup"><span data-stu-id="dbc92-p106">After Custom Learning is installed in your tenant you can add the Web part to a SharePoint page. When you do Office 365 and Windows 10 training is available to your site.</span></span>

1. <span data-ttu-id="dbc92-125">Adicione a Web Part de aprendizado personalizada em um layout de coluna de largura total:</span><span class="sxs-lookup"><span data-stu-id="dbc92-125">Add the Custom Learning webpart in a full width column layout:</span></span>

![Layout de página do SharePoint](media/clo365fullcolumnwidth.png)

2. <span data-ttu-id="dbc92-p107">Na página do SharePoint, selecione Adicionar seção e, em seguida, selecione coluna de largura total.  Você verá o seguinte prompt:</span><span class="sxs-lookup"><span data-stu-id="dbc92-p107">In the SharePoint page, select Add section and then select full width column.  You'll see the following prompt:</span></span>

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. <span data-ttu-id="dbc92-p108">Selecione Microsoft Learning.  Agora você deve ver o seguinte:</span><span class="sxs-lookup"><span data-stu-id="dbc92-p108">Select Microsoft Learning.  You should now see the following:</span></span> 

![Web Part de aprendizado personalizada](media/clo365addwebpart.png)

 <span data-ttu-id="dbc92-133">Agora você pode clicar nos blocos para explorar o conteúdo padrão incluído na solução.</span><span class="sxs-lookup"><span data-stu-id="dbc92-133">You can now click on the tiles to explore the default content included in the solution.</span></span>  

### <a name="next-steps"></a><span data-ttu-id="dbc92-134">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="dbc92-134">Next Steps</span></span>
- <span data-ttu-id="dbc92-135">Explore o [conteúdo padrão](webpartcontent.md) incluído na Web Part.</span><span class="sxs-lookup"><span data-stu-id="dbc92-135">Explore the [default content](webpartcontent.md) included in the webpart.</span></span>
- <span data-ttu-id="dbc92-136">[Personalizar](customization.md) a experiência de treinamento da sua organização.</span><span class="sxs-lookup"><span data-stu-id="dbc92-136">[Customize](customization.md) the training experience for your organization.</span></span>
- <span data-ttu-id="dbc92-137">[Impulsionar a adoção](driveadoption.md) de sua solução de treinamento.</span><span class="sxs-lookup"><span data-stu-id="dbc92-137">[Drive adoption](driveadoption.md) of your training solution.</span></span>

