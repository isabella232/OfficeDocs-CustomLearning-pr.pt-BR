---
author: karuanag
ms.author: karuanag
title: Personalizar e compartilhar listas de reprodução
ms.date: 02/10/2019
description: Criar playlists personalizadas a partir de conteúdo existente ou de novas páginas do SharePoint
ms.openlocfilehash: d330b6e401c9020eb68877bc8a132350811a2f31
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32056365"
---
# <a name="customize-and-share-playlists"></a><span data-ttu-id="8d8ca-103">Personalizar e compartilhar listas de reprodução</span><span class="sxs-lookup"><span data-stu-id="8d8ca-103">Customize and Share Playlists</span></span>

## <a name="create-a-playlist"></a><span data-ttu-id="8d8ca-104">Criar uma lista de reprodução</span><span class="sxs-lookup"><span data-stu-id="8d8ca-104">Create a Playlist</span></span>

<span data-ttu-id="8d8ca-105">Uma lista de reprodução é uma compliation de "ativos".</span><span class="sxs-lookup"><span data-stu-id="8d8ca-105">A playlist is a compliation of "assets".</span></span> <span data-ttu-id="8d8ca-106">Um "ativo" é uma página do SharePoint ou um item existente de conteúdo de treinamento da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-106">An "asset" is a SharePoint page or existing item of Microsoft training content.</span></span> <span data-ttu-id="8d8ca-107">Ao criar uma lista de reprodução, você seleciona ativos que se unem para criar um caminho de aprendizado para o usuário.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-107">When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="8d8ca-108">O benefício de adicionar páginas do SharePoint é que você pode criar páginas do SharePoint com vídeos ou vídeos do YouTube hospedados na sua organização.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-108">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization.</span></span> <span data-ttu-id="8d8ca-109">Você também pode criar páginas com formulários ou outros conteúdos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-109">You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="8d8ca-110">Etapa 1: criar uma página do SharePoint para sua lista de reprodução</span><span class="sxs-lookup"><span data-stu-id="8d8ca-110">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="8d8ca-111">Neste exemplo, primeiro criaremos uma página do SharePoint para adicionar à lista de reprodução.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-111">In this example, we’ll first create a SharePoint page to add to the playlist.</span></span> <span data-ttu-id="8d8ca-112">Criaremos uma página com uma Web Part de vídeo e texto do YouTube.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-112">We’ll create a page with a YouTube video web part and Text web part.</span></span>  <span data-ttu-id="8d8ca-113">Estas instruções pressupõem que você esteja usando o serviço do SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-113">These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="8d8ca-114">Criar uma página</span><span class="sxs-lookup"><span data-stu-id="8d8ca-114">Create a new page</span></span>
1.  <span data-ttu-id="8d8ca-115">Selecione o menu configurações > conteúdo do site > páginas do site > nova página do site do >.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="8d8ca-116">Na área título, digite usar a caixa de comando Teams</span><span class="sxs-lookup"><span data-stu-id="8d8ca-116">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="8d8ca-117">Selecione a seção adicionar uma nova e, em seguida, selecione duas colunas.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-117">Select the Add a new section, and then select Two Columns.</span></span>

![adição de duas colunas](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="8d8ca-119">Na caixa à esquerda, selecione Adicionar uma nova Web Part e, em seguida, selecione incorporar.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-119">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="8d8ca-120">Em um navegador da Web, acesse esta https://youtu.be/wYrRCRphrp0 URL e obtenha o código de inserção para o vídeo.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-120">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="8d8ca-121">Na Web Part do SharePoint, selecione Adicionar código incorporado e cole-o na caixa incorporar.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-121">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="8d8ca-122">Na caixa à direita, selecione Adicionar uma nova Web Part e, em seguida, selecione texto.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-122">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="8d8ca-123">Em um navegador da Web, acesse esta URL https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b : e copie o teste try!</span><span class="sxs-lookup"><span data-stu-id="8d8ca-123">In a Web browser, go to this URL: https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it!</span></span> <span data-ttu-id="8d8ca-124">Instruções da página e cole-as na Web Part de texto.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-124">Instructions from the page and paste them into the Text Web part.</span></span> <span data-ttu-id="8d8ca-125">A página deve ter a seguinte aparência.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-125">Your page should look like the following.</span></span> 

![Inserir página](media/clo365teamscommandbox.png)

9.  <span data-ttu-id="8d8ca-127">Clique em **publicar**e copie o URL da página e cole-o no bloco de notas</span><span class="sxs-lookup"><span data-stu-id="8d8ca-127">Click **Publish**, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="8d8ca-128">Etapa 2: criar a lista de reprodução</span><span class="sxs-lookup"><span data-stu-id="8d8ca-128">Step 2: Create the Playlist</span></span>

1. <span data-ttu-id="8d8ca-129">Navegue até a página de **Administração de aprendizado personalizada** em sua experiência de site.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-129">Navigate to the **Custom Learning Administration** page in your site experience.</span></span>
<span data-ttu-id="8d8ca-130">![custom_admin. png](media/custom_admin.png)</span><span class="sxs-lookup"><span data-stu-id="8d8ca-130">![custom_admin.png](media/custom_admin.png)</span></span>
1. <span data-ttu-id="8d8ca-131">Certifique-se de que **categoria** esteja selecionada</span><span class="sxs-lookup"><span data-stu-id="8d8ca-131">Make sure **Category** is selected</span></span> 
1. <span data-ttu-id="8d8ca-132">Clique na categoria onde você deseja que sua nova lista de reprodução seja exibida</span><span class="sxs-lookup"><span data-stu-id="8d8ca-132">Click on the category where you'd like your new playlist to appear</span></span>
1. <span data-ttu-id="8d8ca-133">Ao lado do nome da categoria, clique no símbolo ![de adição custom_addplay. png](media/custom_addplay.png)</span><span class="sxs-lookup"><span data-stu-id="8d8ca-133">Next to the category name, click on the plus symbol ![custom_addplay.png](media/custom_addplay.png)</span></span>

1. <span data-ttu-id="8d8ca-134">Preencha os valores conforme mostrado no exemplo abaixo e selecione **criar**.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-134">Fill in the values as shown in the example below and select **Create**.</span></span> 
<span data-ttu-id="8d8ca-135">![custom_details. png](media/custom_details.png)</span><span class="sxs-lookup"><span data-stu-id="8d8ca-135">![custom_details.png](media/custom_details.png)</span></span>
- <span data-ttu-id="8d8ca-136">**Título** – nome de exibição da lista de reprodução</span><span class="sxs-lookup"><span data-stu-id="8d8ca-136">**Title** - Display name of the playlist</span></span>
- <span data-ttu-id="8d8ca-137">**Descrição** -informações sobre o que será aprendido</span><span class="sxs-lookup"><span data-stu-id="8d8ca-137">**Description** - Information about what will be learned</span></span>
- <span data-ttu-id="8d8ca-138">**Categoria** : selecionada com base na seleção inicial</span><span class="sxs-lookup"><span data-stu-id="8d8ca-138">**Category** - Preselected based on your initial selection</span></span>
- <span data-ttu-id="8d8ca-139">**Subcategoria** -selecionada com base na seleção inicial</span><span class="sxs-lookup"><span data-stu-id="8d8ca-139">**Sub Category** - Preselected based on your intial selection</span></span>
- <span data-ttu-id="8d8ca-140">**Tecnologia** -selecione conforme aplicável</span><span class="sxs-lookup"><span data-stu-id="8d8ca-140">**Technology** - Select as applicable</span></span>
- <span data-ttu-id="8d8ca-141">**Level** -iniciante, intermidate ou avançado</span><span class="sxs-lookup"><span data-stu-id="8d8ca-141">**Level** - Beginner, Intermidate or Advanced</span></span>
- <span data-ttu-id="8d8ca-142">**Público** -alvo-permite direcionar o conteúdo com base em uma lista predefinida de funções fornecidas pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-142">**Audience** - This allows you to target content based on a pre-defined list of roles provided by Microsoft.</span></span>

6. <span data-ttu-id="8d8ca-143">Clique em **salvar detalhe**</span><span class="sxs-lookup"><span data-stu-id="8d8ca-143">Click **Save Detail**</span></span>

> [!TIP]
> <span data-ttu-id="8d8ca-144">Você pode personalizar a imagem do ícone da sua lista de reprodução.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-144">You can customize the icon image for your playlist.</span></span>  <span data-ttu-id="8d8ca-145">Clique no ícone de imagem e insira uma URL de uma imagem previamente carregada.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-145">Click the image icon and insert an URL of a previously uploaded image.</span></span>  <span data-ttu-id="8d8ca-146">Verifique se a imagem está localizada dentro do conjunto de sites de aprendizado personalizado ou em outro local em que todos os usuários terão acesso ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-146">Make sure the image is located within the Custom Learning site collection or in another location that all users will have access to the file.</span></span>  
<span data-ttu-id="8d8ca-147">![custom_image. png](media/custom_image.png)</span><span class="sxs-lookup"><span data-stu-id="8d8ca-147">![custom_image.png](media/custom_image.png)</span></span>

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="8d8ca-148">Etapa 3: Adicionar ativos à lista de reprodução</span><span class="sxs-lookup"><span data-stu-id="8d8ca-148">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="8d8ca-149">Nesta etapa, você adicionará ativos existentes da Microsoft e da página do SharePoint que você criou na lista de reprodução.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-149">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1. <span data-ttu-id="8d8ca-150">Depois de salvar os detalhes da sua lista de reprodução, você poderá usar a pesquisa de ativos existentes.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-150">Once you have saved the details for your Playlist you can use the Search for Existing Assets.</span></span>
1. <span data-ttu-id="8d8ca-151">**Insira em qualquer termo de pesquisa** para ver uma lista de ativos predefinidos que estão disponíveis a partir de outras listas de reprodução.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-151">**Enter in any search term** to see a list of predefined assets that are available from other playlists.</span></span> <span data-ttu-id="8d8ca-152">**Clique no nome** de um ativo para incluí-lo em sua nova lista de reprodução.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-152">**Click on the name** of an asset to include it in your new playlist.</span></span>
<span data-ttu-id="8d8ca-153">![custom_slist. png](media/custom_slist.png)</span><span class="sxs-lookup"><span data-stu-id="8d8ca-153">![custom_slist.png](media/custom_slist.png)</span></span>

<span data-ttu-id="8d8ca-154">Você também pode adicionar a página do SharePoint que você criou anteriormente ou criar uma desde o início da experiência.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-154">You can also add the SharePoint page you created earlier or create one from scratch in the experience.</span></span>

1. <span data-ttu-id="8d8ca-155">Clique na opção **novo ativo** da caixa de diálogo ativos da playlist</span><span class="sxs-lookup"><span data-stu-id="8d8ca-155">Click on the **New Asset** option in the Playlist Assets dialog</span></span>
1. <span data-ttu-id="8d8ca-156">Dê um **título**ao seu ativo.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-156">Give your asset a **Title**.</span></span> <span data-ttu-id="8d8ca-157">Depois de inseridas, as opções ![adicionais exibirão custom_newpage. png](media/custom_newpage.png)</span><span class="sxs-lookup"><span data-stu-id="8d8ca-157">Once entered, additional options will display ![custom_newpage.png](media/custom_newpage.png)</span></span>
1. <span data-ttu-id="8d8ca-158">Agora você pode criar uma nova página de ativo no SharePoint Online ou inserir a URL de uma página existente para adicioná-la à sua lista de reprodução personalizada.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-158">You can now create a new asset page in SharePoint Online or enter in the URL of an existing page to add it to your custom playlist.</span></span> 
1. <span data-ttu-id="8d8ca-159">Os campos **categoria**, subcategoria e **tecnologia** serão preenchidos previamente com base em suas seleções anteriores para esta lista de reprodução. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="8d8ca-159">**Category**, **Sub Category** and **Technology** fields will be pre-populated based on your previous selections for this playlist.</span></span>
1. <span data-ttu-id="8d8ca-160">Faça as seleções apropriadas para o nível e o público-alvo desse ativo individual.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-160">Make the appropriate selections for Level and Audience for this individual asset.</span></span>  
1. <span data-ttu-id="8d8ca-161">Clique em **salvar ativo** para adicioná-lo à playlist personalizada</span><span class="sxs-lookup"><span data-stu-id="8d8ca-161">Click **Save Asset** to add it to the custom playlist</span></span>
1. <span data-ttu-id="8d8ca-162">Repita essas etapas, pesquisando ou adicionando páginas individuais até que a lista de reprodução esteja concluída.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-162">Repeat these steps, either searching or adding individual pages, until your playlist is complete.</span></span> 
1. <span data-ttu-id="8d8ca-163">Clique em **fechar playlist** para salvar</span><span class="sxs-lookup"><span data-stu-id="8d8ca-163">Click **Close Playlist** to save</span></span>

<span data-ttu-id="8d8ca-164">A sua lista de reprodução com esse conteúdo estará disponível em qualquer lugar em que você instalou/incorporou a Web Part de aprendizado personalizada.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-164">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

> [!NOTE]
> <span data-ttu-id="8d8ca-165">Se você cometer um erro depois de fechar a lista de reprodução, você pode excluí-la da categoria clicando no X ao lado do nome da lista de reprodução.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-165">If you make a mistake once you have closed the playlist, you can delete it from the category by clicking the X next to the playlist name.</span></span>  

#### <a name="things-to-think-about"></a><span data-ttu-id="8d8ca-166">Coisas a considerar</span><span class="sxs-lookup"><span data-stu-id="8d8ca-166">Things to Think About</span></span>

<span data-ttu-id="8d8ca-167">As listas de reprodução personalizadas podem ser usadas para ajudar os usuários finais em várias tarefas.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-167">Custom playlists can be used to assist your end users in a variety of tasks.</span></span>  <span data-ttu-id="8d8ca-168">Você tem um formulário de solicitação de folga?</span><span class="sxs-lookup"><span data-stu-id="8d8ca-168">Do you have a time off request form?</span></span>  <span data-ttu-id="8d8ca-169">Um formulário para solicitar equipamento de hardware?</span><span class="sxs-lookup"><span data-stu-id="8d8ca-169">A form to request hardware equipment?</span></span>  <span data-ttu-id="8d8ca-170">Qualquer ativo de treinamento existente pode ser programado para a experiência.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-170">Any existing training assets can be programmed into the experience.</span></span>  

## <a name="share-playlists"></a><span data-ttu-id="8d8ca-171">Compartilhar listas de reprodução</span><span class="sxs-lookup"><span data-stu-id="8d8ca-171">Share Playlists</span></span>

1. <span data-ttu-id="8d8ca-172">Navegar para qualquer lista de reprodução dentro da Web Part ou experiência do site</span><span class="sxs-lookup"><span data-stu-id="8d8ca-172">Navigate to any playlist within the webpart or site experience</span></span>
1. <span data-ttu-id="8d8ca-173">No canto superior esquerdo, você verá três ícones</span><span class="sxs-lookup"><span data-stu-id="8d8ca-173">In the upper left hand corner you will see three icons</span></span>
1. <span data-ttu-id="8d8ca-174">Clique no ícone que representa um link</span><span class="sxs-lookup"><span data-stu-id="8d8ca-174">Click on the icon representing a link</span></span>
1. <span data-ttu-id="8d8ca-175">Copiar a URL para a lista de reprodução</span><span class="sxs-lookup"><span data-stu-id="8d8ca-175">Copy the URL to the playlist</span></span>

<span data-ttu-id="8d8ca-176">![share. png](media/share.png) essa URL agora pode ser inserida na sua navegação no site ou utilizada em outras comunicações para levar seus funcionários diretamente para essa lista de reprodução.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-176">![share.png](media/share.png) This URL can now be inserted in your site navigation or utilized in other communications to take your employees directly to that playlist.</span></span> 

### <a name="next-steps---drive-adoptiondriveadoptionmd"></a><span data-ttu-id="8d8ca-177">Próximas etapas- [adoção](driveadoption.md) de drives</span><span class="sxs-lookup"><span data-stu-id="8d8ca-177">Next Steps - [Drive Adoption](driveadoption.md)</span></span>
