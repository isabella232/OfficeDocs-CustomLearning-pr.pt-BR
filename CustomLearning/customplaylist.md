# <a name="customize-the-services-and-playlists"></a><span data-ttu-id="3a914-101">Personalizar os serviços e as listas de reprodução</span><span class="sxs-lookup"><span data-stu-id="3a914-101">Customize the Services and Playlists</span></span>

<span data-ttu-id="3a914-p101">Por padrão a experiência de site e a Web Part de incluem conteúdo para todos os serviços do Office 365.  Se apenas a todos ou alguns desses serviços estão disponíveis na sua empresa, você pode ajustar o conteúdo que está disponível para os usuários.  Neste artigo, nós irá personalizar o conteúdo de Web Part.</span><span class="sxs-lookup"><span data-stu-id="3a914-p101">By default both the site experience and the webpart include content for all Office 365 services.  If only all or some of these services are available in your company you can adjust what content is available to your users.  In this article we will customize the webpart content.</span></span>  

## <a name="customizing-the-webpart-content"></a><span data-ttu-id="3a914-105">Personalizando o conteúdo de Web Part</span><span class="sxs-lookup"><span data-stu-id="3a914-105">Customizing the webpart content</span></span>

<span data-ttu-id="3a914-106">A Web Part de aprendizado personalizado oferece dois recursos cruciais:</span><span class="sxs-lookup"><span data-stu-id="3a914-106">The Custom Learning webpart provides two key features:</span></span>
- <span data-ttu-id="3a914-107">Mostrar/ocultar tecnologias</span><span class="sxs-lookup"><span data-stu-id="3a914-107">Hide/Show Technologies</span></span>
- <span data-ttu-id="3a914-108">Criar uma lista de reprodução</span><span class="sxs-lookup"><span data-stu-id="3a914-108">Create a Playlist</span></span>

### <a name="hide-or-show-technology-categories"></a><span data-ttu-id="3a914-109">Ocultar ou Mostrar categorias de tecnologia</span><span class="sxs-lookup"><span data-stu-id="3a914-109">Hide or Show Technology Categories</span></span>

<span data-ttu-id="3a914-110">Para ocultar e Mostrar conteúdo na Web part:</span><span class="sxs-lookup"><span data-stu-id="3a914-110">To hide and show content in the Web part:</span></span> 
1.  <span data-ttu-id="3a914-111">Clique no menu suspenso em que a Web Part e clique em Mostrar/ocultar tecnologias</span><span class="sxs-lookup"><span data-stu-id="3a914-111">Click the dropdown menu on the webpart, then click Hide/Show Technologies</span></span>

![Opção de menu](media/clohideshow.png)

2. <span data-ttu-id="3a914-113">Selecione um checkox para ocultar ou mostrar uma tecnologia e selecione **Aplicar**.</span><span class="sxs-lookup"><span data-stu-id="3a914-113">Select a checkox to hide or show a technology and select **Apply**.</span></span>

![Opções de tecnologia](media/clohideshow1.png)

### <a name="create-a-playlist"></a><span data-ttu-id="3a914-115">Criar uma lista de reprodução</span><span class="sxs-lookup"><span data-stu-id="3a914-115">Create a Playlist</span></span>

<span data-ttu-id="3a914-p102">Uma lista de reprodução é um compliation de "ativos". Um "ativo" é uma página do SharePoint ou o item existente do conteúdo de treinamento do Microsoft. Quando você cria uma lista de reprodução você selecionar ativos que vá juntos para criar um plano de aprendizado para o usuário.</span><span class="sxs-lookup"><span data-stu-id="3a914-p102">A playlist is a compliation of "assets". An "asset" is a SharePoint page or existing item of Microsoft training content. When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="3a914-p103">O benefício da adição de páginas do SharePoint é que você pode criar páginas do SharePoint com um YouTube vídeos ou vídeos hospedados em sua organização. Você também pode criar páginas com formulários ou outros conteúdos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="3a914-p103">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization. You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="3a914-121">Etapa 1: Criar uma página do SharePoint para sua lista de reprodução</span><span class="sxs-lookup"><span data-stu-id="3a914-121">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="3a914-p104">Neste exemplo, vamos primeiro criar uma página do SharePoint para adicionar à lista de reprodução. Criaremos uma página com um YouTube vídeo de web part e a web part de texto.  Estas instruções pressupõem que você estiver usando o serviço do SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="3a914-p104">In this example, we’ll first create a SharePoint page to add to the playlist. We’ll create a page with a YouTube video web part and Text web part.  These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="3a914-125">Criar uma nova página</span><span class="sxs-lookup"><span data-stu-id="3a914-125">Create a new page</span></span>
1.  <span data-ttu-id="3a914-126">Selecione as configurações menu gt _ conteúdos do Site gt _ páginas do Site gt _ Novo gt _ página do Site.</span><span class="sxs-lookup"><span data-stu-id="3a914-126">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="3a914-127">Na área de título, digite Use a caixa de comando de equipes</span><span class="sxs-lookup"><span data-stu-id="3a914-127">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="3a914-128">Selecione Adicionar uma nova seção e, em seguida, selecione duas colunas.</span><span class="sxs-lookup"><span data-stu-id="3a914-128">Select the Add a new section, and then select Two Columns.</span></span>

![adicionar duas colunas](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="3a914-130">Na caixa à esquerda, selecione Adicionar uma nova web part e selecione Embed.</span><span class="sxs-lookup"><span data-stu-id="3a914-130">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="3a914-131">Em um navegador da Web, vá para essa URL https://youtu.be/wYrRCRphrp0 e obtenha o código de inserção para o vídeo.</span><span class="sxs-lookup"><span data-stu-id="3a914-131">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="3a914-132">Na parte da Web do SharePoint, selecione Adicionar incorporar código e cole-o na caixa Embed.</span><span class="sxs-lookup"><span data-stu-id="3a914-132">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="3a914-133">Na caixa direita, selecione Adicionar uma nova web part e, em seguida, selecione o texto.</span><span class="sxs-lookup"><span data-stu-id="3a914-133">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="3a914-p105">Em um navegador da Web, vá para esta URL: https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b e copie o bloco Try-lo! As instruções da página e colá-los em texto Web part. Sua página deve se parecer com o seguinte.</span><span class="sxs-lookup"><span data-stu-id="3a914-p105">In a Web browser, go to this URL: https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it! Instructions from the page and paste them into the Text Web part. Your page should look like the following.</span></span> 

![Incorporar página](media/clo365teamscommandbox.png)

9.  <span data-ttu-id="3a914-138">Clique em Publicar e, em seguida, copie a URL da página e cole-o no bloco de notas</span><span class="sxs-lookup"><span data-stu-id="3a914-138">Click Publish, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="3a914-139">Etapa 2: Criar a lista de reprodução</span><span class="sxs-lookup"><span data-stu-id="3a914-139">Step 2: Create the Playlist</span></span>
1.  <span data-ttu-id="3a914-p106">Navegue até onde você instalou a Web Part de aprendizado personalizado. Na experiência completa do site está hospedado na página de treinamento do Office 365.</span><span class="sxs-lookup"><span data-stu-id="3a914-p106">Navigate to where you have installed the Custom Learning webpart. In the full site experience it is hosted on the Office 365 training page.</span></span> 
2.  <span data-ttu-id="3a914-142">No menu suspenso, selecione Criar nova lista de reprodução.</span><span class="sxs-lookup"><span data-stu-id="3a914-142">From the dropdown menu select Create New Playlist.</span></span> 

![Criar lista de reprodução personalizada](media/clo365createplaylist.png)

3.  <span data-ttu-id="3a914-144">Preencha os valores, conforme mostrado no exemplo a seguir e selecione **criar**.</span><span class="sxs-lookup"><span data-stu-id="3a914-144">Fill in the values as shown in the example below and select **Create**.</span></span> 

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="3a914-145">Etapa 3: Adicionar ativos à lista de reprodução</span><span class="sxs-lookup"><span data-stu-id="3a914-145">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="3a914-146">Nesta etapa, você adicionará ativos existentes da Microsoft e a página do SharePoint que você criou na lista de reprodução.</span><span class="sxs-lookup"><span data-stu-id="3a914-146">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1.  <span data-ttu-id="3a914-147">Clique no botão menu, clique em Adicionar ativo existente.</span><span class="sxs-lookup"><span data-stu-id="3a914-147">Click the menu button, then click Add Existing Asset.</span></span>

![Adicionar ativo](media/clo365addasset.png)

2.  <span data-ttu-id="3a914-149">Filtrar treinamento do Office 365 Apps gt _ equipes da Microsoft</span><span class="sxs-lookup"><span data-stu-id="3a914-149">Filter on Office 365 Apps > Microsoft Teams Training</span></span>
3.  <span data-ttu-id="3a914-150">Adicionar bem-vindo ao Microsoft Teams, obter sua equipe em funcionamento e iniciar bate-papos e fazer chamadas.</span><span class="sxs-lookup"><span data-stu-id="3a914-150">Add Welcome to Microsoft Teams, Get your team up and running, and Start chats and make calls.</span></span>
4.  <span data-ttu-id="3a914-151">Selecione o de botão gt menu _ criar ativos.</span><span class="sxs-lookup"><span data-stu-id="3a914-151">Select the menu button > Create Asset.</span></span>
5.  <span data-ttu-id="3a914-152">Tipo Use a caixa de comando de equipes na caixa Título ativos.</span><span class="sxs-lookup"><span data-stu-id="3a914-152">Type Use the Teams command box in the Asset title box.</span></span> 
6.  <span data-ttu-id="3a914-153">Cole o uso do SharePoint a URL da página equipes comando caixa você copiou no campo conteúdo ativo.</span><span class="sxs-lookup"><span data-stu-id="3a914-153">Paste the SharePoint Use the Teams command box page URL you copied in the Asset content field.</span></span> 
7.  <span data-ttu-id="3a914-p107">Agora navegue de volta para gt _ a Home Page gt _ listas de reprodução de sinalizador seu primeiro dias com gt _ de equipes usam a caixa de comando de equipes. Sua página deve se parecer com o seguinte.</span><span class="sxs-lookup"><span data-stu-id="3a914-p107">Now navigate back to the Home Page > Custom Playlists > Your first days with Teams > Use the Teams command box. Your page should look like the following.</span></span> 

![página criada](media/clo365createplaylist2.png)

<span data-ttu-id="3a914-157">Sua lista de reprodução com esse conteúdo agora estará disponível em qualquer lugar você tiver instalado / incorporada a Web Part de aprendizado personalizado.</span><span class="sxs-lookup"><span data-stu-id="3a914-157">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

#### <a name="things-to-think-about"></a><span data-ttu-id="3a914-158">Coisas a pense sobre</span><span class="sxs-lookup"><span data-stu-id="3a914-158">Things to Think About</span></span>

<span data-ttu-id="3a914-p108">Listas de reprodução personalizadas podem ser usadas para ajudar seus usuários finais em um vareity de tarefas.  Você tem uma formulário de solicitação de folga?  Um formulário para solicitar o equipamento de hardware?  Qualquer ativos de treinamento existentes podem ser programados para a experiência.</span><span class="sxs-lookup"><span data-stu-id="3a914-p108">Custom playlists can be used to assist your end users in a vareity of tasks.  Do you have a time off request form?  A form to request hardware equipment?  Any existing training assets can be programmed into the experience.</span></span>  
