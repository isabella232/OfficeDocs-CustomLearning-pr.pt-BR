# <a name="installing-the-custom-learning-solution-webpart"></a><span data-ttu-id="a8d78-101">Instalando o sinalizador Webpart de solução de aprendizagem</span><span class="sxs-lookup"><span data-stu-id="a8d78-101">Installing the Custom Learning Solution Webpart</span></span>

## <a name="prerequisites-for-a-tenant-wide-installation"></a><span data-ttu-id="a8d78-102">Pré-requisitos para uma instalação de todo o locatário</span><span class="sxs-lookup"><span data-stu-id="a8d78-102">Prerequisites for a tenant-wide installation</span></span>

- <span data-ttu-id="a8d78-p101">Para instalar a Web Part de aprendizado personalizado para seu locatário inteiro, você precisará ter permissões administrativas do Office 365.  Se você não tiver essas permissões, você pode trabalhar com o administrador do Office 365 ou instale a Web Part para um conjunto de sites individuais.</span><span class="sxs-lookup"><span data-stu-id="a8d78-p101">To install the Custom Learning webpart for your entire tenant you will need to have Office 365 Administrative permissions.  If you do not have these permissions you can either work with your Office 365 Administrator or install the webpart for an individual site collection.</span></span>
- <span data-ttu-id="a8d78-105">Você ou o administrador do Office 365 deve ter a instalação e configurado um locatário todo o [Catálogo de aplicativos](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) ou um [Catálogo de aplicativos do conjunto de sites](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)para receber a Web Part.]</span><span class="sxs-lookup"><span data-stu-id="a8d78-105">You or your Office 365 Administrator must have setup and configured a tenant-wide [App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) or a [Site Collection App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)to receive the webpart.]</span></span>
- <span data-ttu-id="a8d78-p102">Oferecemos suporte para SharePoint Online somente. A web part não é o suporte para instalação em qualquer versão do SharePoint no local.</span><span class="sxs-lookup"><span data-stu-id="a8d78-p102">We support SharePoint Online only. The web part is not support for installation on any version of SharePoint on premises.</span></span>

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a><span data-ttu-id="a8d78-108">Adicionar a Web Part de aprendizado personalizado ao seu locatário</span><span class="sxs-lookup"><span data-stu-id="a8d78-108">Add the Custom Learning webpart to your tenant</span></span> 

1. <span data-ttu-id="a8d78-p103">Baixe a Web Part de aprendizado personalizado e salve-o em sua unidade local.  Esse arquivo é chamado "ms-custom-learning.sppkg".  Não altere o nome ou o sufixo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="a8d78-p103">Download the Custom Learning webpart and save it to your local drive.  This file is named "ms-custom-learning.sppkg".  Do not change the name or suffix of the file.</span></span> 
2. <span data-ttu-id="a8d78-112">Navegue até o [portal de administração do Office 365](https://admin.microsoft.com/AdminPortal/Home#/homepage) para seu locatário</span><span class="sxs-lookup"><span data-stu-id="a8d78-112">Navigate to the [Office 365 Admin portal](https://admin.microsoft.com/AdminPortal/Home#/homepage) for your tenant</span></span>
3. <span data-ttu-id="a8d78-p104">No painel de navegação esquerdo selecione centros do administrador do SharePoint. Isso será aberto em uma nova guia, aplicativos de select no SharePoint Admin Center, catálogo de aplicativos, aplicativos para SharePoint</span><span class="sxs-lookup"><span data-stu-id="a8d78-p104">From the left navigation select Admin Centers, SharePoint. This will open in a new tab. , In the SharePoint Admin Center select Apps, App Catalog, Apps for SharePoint</span></span> 
4. <span data-ttu-id="a8d78-115">Selecione carregar a Web Part e escolha o arquivo "ms-custom-learning.sppkg" que você baixou</span><span class="sxs-lookup"><span data-stu-id="a8d78-115">Select upload the webpart and choose the "ms-custom-learning.sppkg" file you downloaded</span></span>
5. <span data-ttu-id="a8d78-116">Para essa verificação de instalação de locatário toda a caixa ao lado de "Fica tornar essa solução disponível a todos na organização."</span><span class="sxs-lookup"><span data-stu-id="a8d78-116">For this tenant-wide installation check the box next to "Make this solution available to all sits in the organization."</span></span>  

![Implantar solução](media/trustapp_sm.png)


## <a name="add-the-customer-learning-webpart-to-a-sharepoint-online-page"></a><span data-ttu-id="a8d78-118">Adicionar a Web Part de aprendizagem do cliente para uma página do SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a8d78-118">Add the Customer Learning webpart to a SharePoint Online Page</span></span>

<span data-ttu-id="a8d78-p105">Depois de aprendizado personalizado está instalado no seu locatário, você pode adicionar a Web part a uma página do SharePoint. Quando você fizer isso, repentinamente treinamento do Office 365 está disponível para você.</span><span class="sxs-lookup"><span data-stu-id="a8d78-p105">After Custom Learning is installed in your tenant you can add the Web part to a SharePoint page. When you do, suddenly Office 365 training is available to you.</span></span> 

1. <span data-ttu-id="a8d78-121">Adicione a Web Part de aprendizado personalizado em um layout de colunas de largura total:</span><span class="sxs-lookup"><span data-stu-id="a8d78-121">Add the Custom Learning webpart in a full width column layout:</span></span>

![Layout de página do SharePoint](media/clo365fullcolumnwidth.png)

2. <span data-ttu-id="a8d78-p106">Na página do SharePoint, selecione seção Adicionar e, em seguida, selecione a coluna de largura total.  Você verá o seguinte aviso:</span><span class="sxs-lookup"><span data-stu-id="a8d78-p106">In the SharePoint page, select Add section and then select full width column.  You'll see the following prompt:</span></span>

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. <span data-ttu-id="a8d78-p107">Selecione Microsoft Learning.  Você verá o seguinte:</span><span class="sxs-lookup"><span data-stu-id="a8d78-p107">Select Microsoft Learning.  You should now see the following:</span></span> 

![Sinalizador de Web Part de aprendizagem](media/clo365addwebpart.png)

 <span data-ttu-id="a8d78-129">Agora, você pode clicar nas peças para explorar o conteúdo padrão incluído na solução.</span><span class="sxs-lookup"><span data-stu-id="a8d78-129">You can now click on the tiles to explore the default content included in the solution.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="a8d78-130">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a8d78-130">Next Steps</span></span>
- <span data-ttu-id="a8d78-131">Explore o [conteúdo padrão](webpartcontent.md) incluído na Web Part de.</span><span class="sxs-lookup"><span data-stu-id="a8d78-131">Explore the [default content](webpartcontent.md) included in the webpart.</span></span>
- <span data-ttu-id="a8d78-132">[Personalizar](customization.md) a experiência de treinamento para sua organização.</span><span class="sxs-lookup"><span data-stu-id="a8d78-132">[Customize](customization.md) the training experience for your organization.</span></span>
- <span data-ttu-id="a8d78-133">[Direcionar a adoção](driveadoption.md) da sua solução de treinamento.</span><span class="sxs-lookup"><span data-stu-id="a8d78-133">[Drive adoption](driveadoption.md) of your training solution.</span></span>

