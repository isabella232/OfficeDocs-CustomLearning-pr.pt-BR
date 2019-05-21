---
author: pkrebs
ms.author: pkrebs
title: Criar páginas do SharePoint para playlists
ms.date: 02/10/2019
description: Criar páginas do SharePoint para playlists
ms.openlocfilehash: 97ef3e7fd37b11011afcc0738245f364a71f5112
ms.sourcegitcommit: 1a111a49a0413a56a880e29109ba01b5e5f33d09
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2019
ms.locfileid: "34247528"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="aeb5c-103">Criar páginas do SharePoint para listas de reprodução personalizadas</span><span class="sxs-lookup"><span data-stu-id="aeb5c-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="aeb5c-104">Um dos recursos exclusivos dos caminhos de aprendizado é a capacidade de criar listas de reprodução remontadas de ativos da Microsoft e de ativos do SharePoint que você cria.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-104">One of the unique features of learning pathways is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create.</span></span> <span data-ttu-id="aeb5c-105">Neste exemplo, criaremos uma página do SharePoint com antecedência da criação de uma lista de reprodução.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-105">In this example, we’ll create a SharePoint page in advance of creating a playlist.</span></span> <span data-ttu-id="aeb5c-106">A capacidade de criar listas de reprodução a partir de páginas do SharePoint oferece uma variedade de oportunidades para criar páginas usando as Web Parts disponíveis na Microsoft ou em sua organização.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-106">The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization.</span></span> <span data-ttu-id="aeb5c-107">Por exemplo, uma lista de reprodução pode incluir uma página do SharePoint com vídeos incorporados do YouTube ou um formulário criado a partir de formulários do Office 365 ou um relatório incorporado do Power BI.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-107">For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report.</span></span> <span data-ttu-id="aeb5c-108">Neste exemplo, mostraremos como criar uma página com a Web Part de inserção e a Web Part de texto.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-108">In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="aeb5c-109">Criar uma página do SharePoint para uma lista de reprodução personalizada</span><span class="sxs-lookup"><span data-stu-id="aeb5c-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="aeb5c-110">Clique no ícone de **engrenagem** do SharePoint e, em seguida, clique em **Adicionar uma página**.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="aeb5c-111">Clique em **Adicionar uma nova seção (+)** no lado esquerdo da página e, em seguida, clique **duas colunas** para o layout da seção.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="aeb5c-112">Na coluna à esquerda, clique em + e, em seguida \*\*\*\* , clique na Web Part de incorporação.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="aeb5c-113">Na coluna à direita, clique em + e, em seguida, clique na Web Part de **texto** .</span><span class="sxs-lookup"><span data-stu-id="aeb5c-113">In the right column, click +, and then click the **Text** web part.</span></span> <span data-ttu-id="aeb5c-114">A página deve ter a seguinte aparência.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-114">Your page should look like this.</span></span>

![CG-pagenewstart. png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="aeb5c-116">Adicionar um vídeo e um texto do YouTube</span><span class="sxs-lookup"><span data-stu-id="aeb5c-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="aeb5c-117">No navegador, vá para YouTube.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-117">In your browser, go to YouTube.</span></span> <span data-ttu-id="aeb5c-118">Para este exemplo, pesquise por "What is Office 365 – Best Productivity aplicativos da Microsoft".</span><span class="sxs-lookup"><span data-stu-id="aeb5c-118">For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="aeb5c-119">Clique no vídeo para reproduzi-lo, depois Pause-o e, em seguida, clique com o botão direito do mouse nele.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="aeb5c-120">Clique em **copiar código de inserção**e retorne para a página do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="aeb5c-121">Clique em **Adicionar código** de incorporação na Web Part de **incorporação** e, em seguida, adicione o código do vídeo do YouTube.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="aeb5c-122">Retorne à página YouTube e copie o texto da **Descrição** do vídeo.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="aeb5c-123">Retorne à página do SharePoint, selecione a Web Part de **texto** e copie o texto do vídeo do YouTube.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="aeb5c-124">Selecione o ícone **Editar Web Part** na área título da página do SharePoint e, em seguida, nomeie a página "introdução à playlist personalizada".</span><span class="sxs-lookup"><span data-stu-id="aeb5c-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="aeb5c-125">Em **layout**, selecione **simples**e, em seguida, fechar painel de propriedades da **região de título** .</span><span class="sxs-lookup"><span data-stu-id="aeb5c-125">For **Layout**, select **Plain**, then close **Title Region** properties pane.</span></span> <span data-ttu-id="aeb5c-126">A página agora deve ter a seguinte aparência.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-126">The page should now look something like the following.</span></span> 

![CG-pagenewfinish. png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="aeb5c-128">Publicar a página</span><span class="sxs-lookup"><span data-stu-id="aeb5c-128">Publish the page</span></span>

- <span data-ttu-id="aeb5c-129">Selecione o botão **publicar** .</span><span class="sxs-lookup"><span data-stu-id="aeb5c-129">Select the **Publish** button.</span></span> <span data-ttu-id="aeb5c-130">Agora você está pronto para adicionar esta página do SharePoint à sua lista de reprodução personalizada.</span><span class="sxs-lookup"><span data-stu-id="aeb5c-130">Now you're ready to add this SharePoint page to your custom playlist.</span></span> 