---
author: pkrebs
ms.author: pkrebs
title: Criar SharePoint páginas para playlists
ms.date: 02/10/2019
description: Criar SharePoint páginas para playlists
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
ms.openlocfilehash: ce4a204b3072469840b6f3fa8f93d9e78833b181
ms.sourcegitcommit: 956ab22dd8ce23ee1779f1a01d34b434243c3cb1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2021
ms.locfileid: "52310655"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="e8e6e-103">Criar SharePoint páginas para playlists personalizadas</span><span class="sxs-lookup"><span data-stu-id="e8e6e-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="e8e6e-104">Um dos recursos exclusivos dos caminhos de aprendizado é a capacidade de criar listas de reprodução que são montadas a partir de ativos da Microsoft e SharePoint ativos que você cria.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-104">One of the unique features of learning pathways is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create.</span></span> <span data-ttu-id="e8e6e-105">Neste exemplo, criaremos uma página SharePoint antes de criar uma playlist.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-105">In this example, we’ll create a SharePoint page in advance of creating a playlist.</span></span> <span data-ttu-id="e8e6e-106">A capacidade de criar playlists SharePoint páginas oferece várias oportunidades para criar páginas usando as Web Parts disponíveis da Microsoft ou da sua organização.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-106">The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization.</span></span> <span data-ttu-id="e8e6e-107">Por exemplo, uma playlist pode incluir uma página de SharePoint com vídeos incorporados do YouTube ou um formulário criado a partir do Office 365 Forms ou um relatório Power BI incorporado.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-107">For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report.</span></span> <span data-ttu-id="e8e6e-108">Neste exemplo, mostraremos como criar uma página com a Web Part Incorporar e a Web Part Texto.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-108">In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="e8e6e-109">Criar uma SharePoint para uma playlist personalizada</span><span class="sxs-lookup"><span data-stu-id="e8e6e-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="e8e6e-110">Clique no SharePoint **de** engrenagem e clique **em Adicionar uma página.**</span><span class="sxs-lookup"><span data-stu-id="e8e6e-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="e8e6e-111">Clique **em Adicionar uma nova seção (+)** no lado esquerdo da página e clique em Duas **Colunas** para o layout da seção.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="e8e6e-112">Na coluna esquerda, clique em + e clique na Web Part **Incorporar.**</span><span class="sxs-lookup"><span data-stu-id="e8e6e-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="e8e6e-113">Na coluna direita, clique em +e clique na Web Part **Texto.**</span><span class="sxs-lookup"><span data-stu-id="e8e6e-113">In the right column, click +, and then click the **Text** web part.</span></span> <span data-ttu-id="e8e6e-114">Sua página deve ter esta aparência.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-114">Your page should look like this.</span></span>

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="e8e6e-116">Adicionar um vídeo e texto do YouTube</span><span class="sxs-lookup"><span data-stu-id="e8e6e-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="e8e6e-117">No navegador, vá para o YouTube.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-117">In your browser, go to YouTube.</span></span> <span data-ttu-id="e8e6e-118">Para este exemplo, pesquise "O que é Office 365 – os melhores aplicativos de produtividade da Microsoft".</span><span class="sxs-lookup"><span data-stu-id="e8e6e-118">For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="e8e6e-119">Clique no vídeo para reproduzi-lo, pause-o e clique com o botão direito do mouse nele.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="e8e6e-120">Clique **em Copiar código de incorporar** e retorne à página SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="e8e6e-121">Clique **em Adicionar código de** incorporar na Web Part Incorporar e, em seguida, adicione o código do vídeo do YouTube. </span><span class="sxs-lookup"><span data-stu-id="e8e6e-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="e8e6e-122">Volte para a página do YouTube e copie o texto **Descrição** do vídeo.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="e8e6e-123">Volte para a página SharePoint, selecione a Web Part **Texto** e copie o texto do vídeo do YouTube.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="e8e6e-124">Selecione o **ícone editar web part** na área Título da página SharePoint e, em seguida, nomee a página "Introdução personalizada da playlist".</span><span class="sxs-lookup"><span data-stu-id="e8e6e-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="e8e6e-125">Para **Layout,** selecione **Plain**, em seguida, feche o painel de propriedades **da** Região de Título.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-125">For **Layout**, select **Plain**, then close **Title Region** properties pane.</span></span> <span data-ttu-id="e8e6e-126">A página agora deve ter uma aparência parecida com a seguinte.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-126">The page should now look something like the following.</span></span> 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="e8e6e-128">Publicar a página</span><span class="sxs-lookup"><span data-stu-id="e8e6e-128">Publish the page</span></span>

- <span data-ttu-id="e8e6e-129">Selecione o **botão Publicar.**</span><span class="sxs-lookup"><span data-stu-id="e8e6e-129">Select the **Publish** button.</span></span> <span data-ttu-id="e8e6e-130">Agora você está pronto para adicionar essa página SharePoint à sua playlist personalizada.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-130">Now you're ready to add this SharePoint page to your custom playlist.</span></span> 