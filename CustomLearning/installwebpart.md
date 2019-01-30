# <a name="installing-the-custom-learning-solution-webpart"></a>Instalando o sinalizador Webpart de solução de aprendizagem

## <a name="prerequisites-for-a-tenant-wide-installation"></a>Pré-requisitos para uma instalação de todo o locatário

- Para instalar a Web Part de aprendizado personalizado para seu locatário inteiro, você precisará ter permissões administrativas do Office 365.  Se você não tiver essas permissões, você pode trabalhar com o administrador do Office 365 ou instale a Web Part para um conjunto de sites individuais.
- Você ou o administrador do Office 365 deve ter a instalação e configurado um locatário todo o [Catálogo de aplicativos](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) ou um [Catálogo de aplicativos do conjunto de sites](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)para receber a Web Part.]
- Oferecemos suporte para SharePoint Online somente. A web part não é o suporte para instalação em qualquer versão do SharePoint no local.

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a>Adicionar a Web Part de aprendizado personalizado ao seu locatário 

1. Baixe a Web Part de aprendizado personalizado e salve-o em sua unidade local.  Esse arquivo é chamado "ms-custom-learning.sppkg".  Não altere o nome ou o sufixo do arquivo. 
2. Navegue até o [portal de administração do Office 365](https://admin.microsoft.com/AdminPortal/Home#/homepage) para seu locatário
3. No painel de navegação esquerdo selecione centros do administrador do SharePoint. Isso será aberto em uma nova guia, aplicativos de select no SharePoint Admin Center, catálogo de aplicativos, aplicativos para SharePoint 
4. Selecione carregar a Web Part e escolha o arquivo "ms-custom-learning.sppkg" que você baixou
5. Para essa verificação de instalação de locatário toda a caixa ao lado de "Fica tornar essa solução disponível a todos na organização."  

![Implantar solução](media/trustapp_sm.png)


## <a name="add-the-customer-learning-webpart-to-a-sharepoint-online-page"></a>Adicionar a Web Part de aprendizagem do cliente para uma página do SharePoint Online

Depois de aprendizado personalizado está instalado no seu locatário, você pode adicionar a Web part a uma página do SharePoint. Quando você fizer isso, repentinamente treinamento do Office 365 está disponível para você. 

1. Adicione a Web Part de aprendizado personalizado em um layout de colunas de largura total:

![Layout de página do SharePoint](media/clo365fullcolumnwidth.png)

2. Na página do SharePoint, selecione seção Adicionar e, em seguida, selecione a coluna de largura total.  Você verá o seguinte aviso:

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. Selecione Microsoft Learning.  Você verá o seguinte: 

![Sinalizador de Web Part de aprendizagem](media/clo365addwebpart.png)

 Agora, você pode clicar nas peças para explorar o conteúdo padrão incluído na solução.  

## <a name="next-steps"></a>Próximas etapas
- Explore o [conteúdo padrão](webpartcontent.md) incluído na Web Part de.
- [Personalizar](customization.md) a experiência de treinamento para sua organização.
- [Direcionar a adoção](driveadoption.md) da sua solução de treinamento.

