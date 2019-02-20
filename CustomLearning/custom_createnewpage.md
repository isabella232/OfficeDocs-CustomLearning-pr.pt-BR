---
author: pkrebs
ms.author: pkrebs
title: Criar páginas do SharePoint para playlists
ms.date: 02/10/2019
description: Criar páginas do SharePoint para playlists
ms.openlocfilehash: c2de66a0746260e8f6539656ad70052b209c54ba
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/19/2019
ms.locfileid: "30103686"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="b4422-103">Criar páginas do SharePoint para listas de reprodução personalizadas</span><span class="sxs-lookup"><span data-stu-id="b4422-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="b4422-p101">Um dos recursos exclusivos de aprendizado personalizado é a capacidade de criar listas de reprodução remontadas de ativos da Microsoft e de ativos do SharePoint que você cria. Neste exemplo, criaremos uma página do SharePoint com antecedência da criação de uma lista de reprodução. A capacidade de criar listas de reprodução a partir de páginas do SharePoint oferece uma variedade de oportunidades para criar páginas usando as Web Parts disponíveis na Microsoft ou em sua organização. Por exemplo, uma lista de reprodução pode incluir uma página do SharePoint com vídeos incorporados do YouTube ou um formulário criado a partir de formulários do Office 365 ou um relatório incorporado do Power BI. Neste exemplo, mostraremos como criar uma página com a Web Part de inserção e a Web Part de texto.</span><span class="sxs-lookup"><span data-stu-id="b4422-p101">One of the unique features of Custom Learning is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create. In this example, we’ll create a SharePoint page in advance of creating a playlist. The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization. For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report. In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="b4422-109">Criar uma página do SharePoint para uma lista de reprodução personalizada</span><span class="sxs-lookup"><span data-stu-id="b4422-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="b4422-110">Clique no ícone de **engrenagem** do SharePoint e, em seguida, clique em **Adicionar uma página**.</span><span class="sxs-lookup"><span data-stu-id="b4422-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="b4422-111">Clique em **Adicionar uma nova seção (+)** no lado esquerdo da página e, em seguida, clique **duas colunas** para o layout da seção.</span><span class="sxs-lookup"><span data-stu-id="b4422-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="b4422-112">Na coluna à esquerda, clique em + e, em seguida \*\*\*\* , clique na Web Part de incorporação.</span><span class="sxs-lookup"><span data-stu-id="b4422-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="b4422-p102">Na coluna à direita, clique em + e, em seguida, clique na Web Part de **texto** . A página deve ter a seguinte aparência.</span><span class="sxs-lookup"><span data-stu-id="b4422-p102">In the right column, click +, and then click the **Text** web part. Your page should look like this.</span></span>

![CG-pagenewstart. png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="b4422-116">Adicionar um vídeo e um texto do YouTube</span><span class="sxs-lookup"><span data-stu-id="b4422-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="b4422-p103">No navegador, vá para YouTube. Para este exemplo, pesquise por "What is Office 365 – Best Productivity aplicativos da Microsoft".</span><span class="sxs-lookup"><span data-stu-id="b4422-p103">In your browser, go to YouTube. For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="b4422-119">Clique no vídeo para reproduzi-lo, depois Pause-o e, em seguida, clique com o botão direito do mouse nele.</span><span class="sxs-lookup"><span data-stu-id="b4422-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="b4422-120">Clique em **copiar código de inserção**e retorne para a página do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b4422-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="b4422-121">Clique em **Adicionar código** de incorporação na Web Part de **incorporação** e, em seguida, adicione o código do vídeo do YouTube.</span><span class="sxs-lookup"><span data-stu-id="b4422-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="b4422-122">ReTorne à página YouTube e copie o texto da **Descrição** do vídeo.</span><span class="sxs-lookup"><span data-stu-id="b4422-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="b4422-123">ReTorne à página do SharePoint, selecione a Web Part de **texto** e copie o texto do vídeo do YouTube.</span><span class="sxs-lookup"><span data-stu-id="b4422-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="b4422-124">Selecione o ícone **Editar Web Part** na área título da página do SharePoint e, em seguida, nomeie a página "introdução à playlist personalizada".</span><span class="sxs-lookup"><span data-stu-id="b4422-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="b4422-p104">Em **layout**, selecione **simples**e, em seguida, fechar painel de propriedades da **região de título** . A página agora deve ter a seguinte aparência.</span><span class="sxs-lookup"><span data-stu-id="b4422-p104">For **Layout**, select **Plain**, then close **Title Region** properties pane. The page should now look something like the following.</span></span> 

![CG-pagenewfinish. png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="b4422-128">Publicar a página</span><span class="sxs-lookup"><span data-stu-id="b4422-128">Publish the page</span></span>

- <span data-ttu-id="b4422-p105">Selecione o botão **publicar** . Agora você está pronto para adicionar esta página do SharePoint à sua lista de reprodução personalizada.</span><span class="sxs-lookup"><span data-stu-id="b4422-p105">Select the **Publish** button. Now you're ready to add this SharePoint page to your custom playlist.</span></span> 