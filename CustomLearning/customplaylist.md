---
author: karuanag
ms.author: karuanag
manager: alexb
title: Personalizar e compartilhar playlists
ms.date: 02/10/2019
description: Criar playlists personalizadas de conteúdo existente ou novas páginas do SharePoint
ms.service: sharepoint-online
audience: itpro
ms.topic: article
ms.openlocfilehash: 31a0e5524181d26f4d62ae7206636c9e553b6f8f
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000207"
---
# <a name="customize-and-share-playlists"></a><span data-ttu-id="b743d-103">Personalizar e compartilhar playlists</span><span class="sxs-lookup"><span data-stu-id="b743d-103">Customize and share playlists</span></span>

## <a name="create-a-playlist"></a><span data-ttu-id="b743d-104">Criar uma playlist</span><span class="sxs-lookup"><span data-stu-id="b743d-104">Create a Playlist</span></span>

<span data-ttu-id="b743d-105">Uma playlist é um compliation de "assets".</span><span class="sxs-lookup"><span data-stu-id="b743d-105">A playlist is a compliation of "assets".</span></span> <span data-ttu-id="b743d-106">Um "ativo" é uma página do SharePoint ou um item existente do conteúdo de treinamento da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b743d-106">An "asset" is a SharePoint page or existing item of Microsoft training content.</span></span> <span data-ttu-id="b743d-107">Ao criar uma playlist, você seleciona ativos que se juntam para criar um caminho de aprendizado para o usuário.</span><span class="sxs-lookup"><span data-stu-id="b743d-107">When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="b743d-108">O benefício de adicionar páginas do SharePoint é que você pode criar páginas do SharePoint com vídeos ou vídeos do YouTube hospedados em sua organização.</span><span class="sxs-lookup"><span data-stu-id="b743d-108">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization.</span></span> <span data-ttu-id="b743d-109">Você também pode criar páginas com Formulários ou outro conteúdo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b743d-109">You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="b743d-110">Etapa 1: Criar uma página do SharePoint para sua playlist</span><span class="sxs-lookup"><span data-stu-id="b743d-110">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="b743d-111">Neste exemplo, primeiro criaremos uma página do SharePoint para adicionar à playlist.</span><span class="sxs-lookup"><span data-stu-id="b743d-111">In this example, we’ll first create a SharePoint page to add to the playlist.</span></span> <span data-ttu-id="b743d-112">Criaremos uma página com uma Web Part de vídeo do YouTube e Uma Web Part text.</span><span class="sxs-lookup"><span data-stu-id="b743d-112">We’ll create a page with a YouTube video web part and Text web part.</span></span>  <span data-ttu-id="b743d-113">Estas instruções pressuem que você está usando o serviço do SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="b743d-113">These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="b743d-114">Criar uma página</span><span class="sxs-lookup"><span data-stu-id="b743d-114">Create a new page</span></span>
1.  <span data-ttu-id="b743d-115">Selecione o menu Configurações > Conteúdo do Site > Páginas do Site > Página novo > Site.</span><span class="sxs-lookup"><span data-stu-id="b743d-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="b743d-116">Na área título, digite Usar a caixa de comando Do Teams</span><span class="sxs-lookup"><span data-stu-id="b743d-116">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="b743d-117">Selecione a seção Adicionar uma nova e selecione Duas Colunas.</span><span class="sxs-lookup"><span data-stu-id="b743d-117">Select the Add a new section, and then select Two Columns.</span></span>

![adicionar duas colunas](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="b743d-119">Na caixa à esquerda, selecione Adicionar uma nova Web Part e selecione Incorporar.</span><span class="sxs-lookup"><span data-stu-id="b743d-119">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="b743d-120">Em um navegador da Web, vá até essa URL e receba o código https://youtu.be/wYrRCRphrp0 de incorporar do vídeo.</span><span class="sxs-lookup"><span data-stu-id="b743d-120">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="b743d-121">Na Web Part do SharePoint, selecione Adicionar código incorporar e, em seguida, colar-o na caixa Incorporar.</span><span class="sxs-lookup"><span data-stu-id="b743d-121">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="b743d-122">Na caixa à direita, selecione Adicionar uma nova Web Part e selecione Texto.</span><span class="sxs-lookup"><span data-stu-id="b743d-122">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="b743d-123">Em um navegador da Web, acesse esta URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b e copie o Try it!</span><span class="sxs-lookup"><span data-stu-id="b743d-123">In a Web browser, go to this URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it!</span></span> <span data-ttu-id="b743d-124">Instruções da página e colar-as na Web Part texto.</span><span class="sxs-lookup"><span data-stu-id="b743d-124">Instructions from the page and paste them into the Text Web part.</span></span> <span data-ttu-id="b743d-125">Sua página deve ter a seguinte aparência.</span><span class="sxs-lookup"><span data-stu-id="b743d-125">Your page should look like the following.</span></span> 
<span data-ttu-id="b743d-126">![Página incorporar](media/clo365teamscommandbox.png)</span><span class="sxs-lookup"><span data-stu-id="b743d-126">![Embed page](media/clo365teamscommandbox.png)</span></span>
9.  <span data-ttu-id="b743d-127">Clique **em Publicar** e copie a URL da página e a colar no Bloco de Notas</span><span class="sxs-lookup"><span data-stu-id="b743d-127">Click **Publish**, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="b743d-128">Etapa 2: Criar a playlist</span><span class="sxs-lookup"><span data-stu-id="b743d-128">Step 2: Create the Playlist</span></span>

1. <span data-ttu-id="b743d-129">Navegue até **a página Administração de Aprendizagem Personalizada** em sua experiência de site.</span><span class="sxs-lookup"><span data-stu-id="b743d-129">Navigate to the **Custom Learning Administration** page in your site experience.</span></span>
<span data-ttu-id="b743d-130">![Tela em que você seleciona Administração de Aprendizagem Personalizada.](media/custom_admin.png)</span><span class="sxs-lookup"><span data-stu-id="b743d-130">![Screen where you select Custom Learning Administration.](media/custom_admin.png)</span></span>
1. <span data-ttu-id="b743d-131">Certifique-se **de que Category** está selecionado</span><span class="sxs-lookup"><span data-stu-id="b743d-131">Make sure **Category** is selected</span></span> 
1. <span data-ttu-id="b743d-132">Clique na categoria na qual você gostaria que sua nova playlist fosse exibida</span><span class="sxs-lookup"><span data-stu-id="b743d-132">Click on the category where you'd like your new playlist to appear</span></span>
1. <span data-ttu-id="b743d-133">Ao lado do nome da categoria, clique no símbolo de adição Janela com a opção Categoria e ![ o sinal Plus realçado.](media/custom_addplay.png)</span><span class="sxs-lookup"><span data-stu-id="b743d-133">Next to the category name, click on the plus symbol ![Window with the Category option and the Plus sign highlighted.](media/custom_addplay.png)</span></span>

1. <span data-ttu-id="b743d-134">Preencha os valores conforme mostrado no exemplo abaixo e selecione **Criar**.</span><span class="sxs-lookup"><span data-stu-id="b743d-134">Fill in the values as shown in the example below and select **Create**.</span></span> 
<span data-ttu-id="b743d-135">![Página onde você inserir detalhes da lista de reprodução.](media/custom_details.png)</span><span class="sxs-lookup"><span data-stu-id="b743d-135">![Page where you enter playlist details.](media/custom_details.png)</span></span>
- <span data-ttu-id="b743d-136">**Título** - Nome de exibição da playlist</span><span class="sxs-lookup"><span data-stu-id="b743d-136">**Title** - Display name of the playlist</span></span>
- <span data-ttu-id="b743d-137">**Descrição** - Informações sobre o que será aprendido</span><span class="sxs-lookup"><span data-stu-id="b743d-137">**Description** - Information about what will be learned</span></span>
- <span data-ttu-id="b743d-138">**Categoria** - Pré-selecionado com base em sua seleção inicial</span><span class="sxs-lookup"><span data-stu-id="b743d-138">**Category** - Preselected based on your initial selection</span></span>
- <span data-ttu-id="b743d-139">**Sub Category** - Pré-selecionado com base em sua seleção intial</span><span class="sxs-lookup"><span data-stu-id="b743d-139">**Sub Category** - Preselected based on your intial selection</span></span>
- <span data-ttu-id="b743d-140">**Tecnologia** - Selecione conforme aplicável</span><span class="sxs-lookup"><span data-stu-id="b743d-140">**Technology** - Select as applicable</span></span>
- <span data-ttu-id="b743d-141">**Nível** - Iniciante, Intermidate ou Avançado</span><span class="sxs-lookup"><span data-stu-id="b743d-141">**Level** - Beginner, Intermidate or Advanced</span></span>
- <span data-ttu-id="b743d-142">**Público-** Isso permite direcionar conteúdo com base em uma lista pré-definida de funções fornecidas pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b743d-142">**Audience** - This allows you to target content based on a pre-defined list of roles provided by Microsoft.</span></span>

6. <span data-ttu-id="b743d-143">Clique **em Salvar Detalhes**</span><span class="sxs-lookup"><span data-stu-id="b743d-143">Click **Save Detail**</span></span>

> [!TIP]
> <span data-ttu-id="b743d-144">Você pode personalizar a imagem do ícone da sua playlist.</span><span class="sxs-lookup"><span data-stu-id="b743d-144">You can customize the icon image for your playlist.</span></span>  <span data-ttu-id="b743d-145">Clique no ícone da imagem e insira uma URL de uma imagem carregada anteriormente.</span><span class="sxs-lookup"><span data-stu-id="b743d-145">Click the image icon and insert an URL of a previously uploaded image.</span></span>  <span data-ttu-id="b743d-146">Certifique-se de que a imagem está localizada no conjunto de sites De Aprendizagem Personalizada ou em outro local que todos os usuários terão acesso ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="b743d-146">Make sure the image is located within the Custom Learning site collection or in another location that all users will have access to the file.</span></span>  
<span data-ttu-id="b743d-147">![Escolha uma janela de imagem.](media/custom_image.png)</span><span class="sxs-lookup"><span data-stu-id="b743d-147">![Choose an image window.](media/custom_image.png)</span></span>

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="b743d-148">Etapa 3: Adicionar ativos à playlist</span><span class="sxs-lookup"><span data-stu-id="b743d-148">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="b743d-149">Nesta etapa, você adicionará ativos existentes da Microsoft e a página do SharePoint criada à playlist.</span><span class="sxs-lookup"><span data-stu-id="b743d-149">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1. <span data-ttu-id="b743d-150">Depois de salvar os detalhes da playlist, você pode usar a Pesquisa de Ativos Existentes.</span><span class="sxs-lookup"><span data-stu-id="b743d-150">Once you have saved the details for your Playlist you can use the Search for Existing Assets.</span></span>
1. <span data-ttu-id="b743d-151">**Insira em qualquer termo de pesquisa** para ver uma lista de ativos predefinidos que estão disponíveis em outras listas de reprodução.</span><span class="sxs-lookup"><span data-stu-id="b743d-151">**Enter in any search term** to see a list of predefined assets that are available from other playlists.</span></span> <span data-ttu-id="b743d-152">**Clique no nome de** um ativo para incluí-lo em sua nova playlist.</span><span class="sxs-lookup"><span data-stu-id="b743d-152">**Click on the name** of an asset to include it in your new playlist.</span></span><br/>
<span data-ttu-id="b743d-153">![Página ativos de playlist](media/custom_slist.png)</span><span class="sxs-lookup"><span data-stu-id="b743d-153">![Playlist assets page](media/custom_slist.png)</span></span>

<span data-ttu-id="b743d-154">Você também pode adicionar a página do SharePoint criada anteriormente ou criar uma do zero na experiência.</span><span class="sxs-lookup"><span data-stu-id="b743d-154">You can also add the SharePoint page you created earlier or create one from scratch in the experience.</span></span>

1. <span data-ttu-id="b743d-155">Clique na opção **Novo Ativo** na caixa de diálogo Ativos de Playlist.</span><span class="sxs-lookup"><span data-stu-id="b743d-155">Click on the **New Asset** option in the Playlist Assets dialog.</span></span>
1. <span data-ttu-id="b743d-156">Dê a seu ativo um **Título**.</span><span class="sxs-lookup"><span data-stu-id="b743d-156">Give your asset a **Title**.</span></span> <span data-ttu-id="b743d-157">Depois de inserido, opções adicionais serão exibidas.</span><span class="sxs-lookup"><span data-stu-id="b743d-157">Once entered, additional options will display.</span></span>
<span data-ttu-id="b743d-158">![Formulário em que você institui seu título e detalhes adicionais.](media/custom_newpage.png)</span><span class="sxs-lookup"><span data-stu-id="b743d-158">![Form where you enter your title and additional details.](media/custom_newpage.png)</span></span>
1. <span data-ttu-id="b743d-159">Agora você pode criar uma nova página de ativos no SharePoint Online ou inserir a URL de uma página existente para adicioná-la à sua playlist personalizada.</span><span class="sxs-lookup"><span data-stu-id="b743d-159">You can now create a new asset page in SharePoint Online or enter in the URL of an existing page to add it to your custom playlist.</span></span> 
1. <span data-ttu-id="b743d-160">**Os** campos Categoria **, Sub** Categoria e **Tecnologia** serão pré-preenchidos com base em suas seleções anteriores para esta playlist.</span><span class="sxs-lookup"><span data-stu-id="b743d-160">**Category**, **Sub Category** and **Technology** fields will be pre-populated based on your previous selections for this playlist.</span></span>
1. <span data-ttu-id="b743d-161">Faça as seleções apropriadas para Nível e Audiência para esse ativo individual.</span><span class="sxs-lookup"><span data-stu-id="b743d-161">Make the appropriate selections for Level and Audience for this individual asset.</span></span>  
1. <span data-ttu-id="b743d-162">Clique **em Salvar Ativo** para adicioná-lo à playlist personalizada</span><span class="sxs-lookup"><span data-stu-id="b743d-162">Click **Save Asset** to add it to the custom playlist</span></span>
1. <span data-ttu-id="b743d-163">Repita estas etapas, pesquisando ou adicionando páginas individuais, até que sua playlist seja concluída.</span><span class="sxs-lookup"><span data-stu-id="b743d-163">Repeat these steps, either searching or adding individual pages, until your playlist is complete.</span></span> 
1. <span data-ttu-id="b743d-164">Clique **em Fechar Playlist** para salvar</span><span class="sxs-lookup"><span data-stu-id="b743d-164">Click **Close Playlist** to save</span></span>

<span data-ttu-id="b743d-165">Sua playlist com esse conteúdo agora estará disponível em qualquer lugar que você instalou/inserou a webpart de Aprendizado Personalizado.</span><span class="sxs-lookup"><span data-stu-id="b743d-165">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

> [!NOTE]
> <span data-ttu-id="b743d-166">Se você cometer um erro depois de fechar a playlist, poderá excluí-la da categoria clicando no X ao lado do nome da playlist.</span><span class="sxs-lookup"><span data-stu-id="b743d-166">If you make a mistake once you have closed the playlist, you can delete it from the category by clicking the X next to the playlist name.</span></span>  

#### <a name="things-to-think-about"></a><span data-ttu-id="b743d-167">Coisas para pensar</span><span class="sxs-lookup"><span data-stu-id="b743d-167">Things to Think About</span></span>

<span data-ttu-id="b743d-168">Listas de reprodução personalizadas podem ser usadas para ajudar os usuários finais em várias tarefas.</span><span class="sxs-lookup"><span data-stu-id="b743d-168">Custom playlists can be used to assist your end users in a variety of tasks.</span></span>  <span data-ttu-id="b743d-169">Você tem um formulário de solicitação de tempo de folga?</span><span class="sxs-lookup"><span data-stu-id="b743d-169">Do you have a time off request form?</span></span>  <span data-ttu-id="b743d-170">Um formulário para solicitar equipamento de hardware?</span><span class="sxs-lookup"><span data-stu-id="b743d-170">A form to request hardware equipment?</span></span>  <span data-ttu-id="b743d-171">Todos os ativos de treinamento existentes podem ser programados na experiência.</span><span class="sxs-lookup"><span data-stu-id="b743d-171">Any existing training assets can be programmed into the experience.</span></span>  

## <a name="share-playlists"></a><span data-ttu-id="b743d-172">Compartilhar Playlists</span><span class="sxs-lookup"><span data-stu-id="b743d-172">Share Playlists</span></span>

1. <span data-ttu-id="b743d-173">Navegue até qualquer playlist dentro da webpart ou experiência do site</span><span class="sxs-lookup"><span data-stu-id="b743d-173">Navigate to any playlist within the webpart or site experience</span></span>
1. <span data-ttu-id="b743d-174">No canto superior esquerdo, você verá três ícones</span><span class="sxs-lookup"><span data-stu-id="b743d-174">In the upper left hand corner you will see three icons</span></span>
1. <span data-ttu-id="b743d-175">Clique no ícone que representa um link</span><span class="sxs-lookup"><span data-stu-id="b743d-175">Click on the icon representing a link</span></span>
1. <span data-ttu-id="b743d-176">Copie a URL para a Tela de playlist ![ onde você clica em Copiar ao lado da URL.](media/share.png)</span><span class="sxs-lookup"><span data-stu-id="b743d-176">Copy the URL to the playlist ![Screen where you click Copy next to the URL.](media/share.png)</span></span>
<span data-ttu-id="b743d-177">Essa URL agora pode ser inserida na navegação do site ou usada em outras comunicações para levar seus funcionários diretamente para essa playlist.</span><span class="sxs-lookup"><span data-stu-id="b743d-177">This URL can now be inserted in your site navigation or utilized in other communications to take your employees directly to that playlist.</span></span> 

### <a name="next-steps---drive-adoption"></a><span data-ttu-id="b743d-178">Próximas etapas - [Impulsionar a adoção](driveadoption.md)</span><span class="sxs-lookup"><span data-stu-id="b743d-178">Next Steps - [Drive Adoption](driveadoption.md)</span></span>
