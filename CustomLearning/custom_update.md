---
author: pkrebs
ms.author: pkrebs
title: Atualizar caminhos de aprendizagem do Microsoft 365
ms.date: 07/06/2020
description: Atualizar caminhos de aprendizagem do Microsoft 365
ms.openlocfilehash: 6880e49f925f18b961790ec9eff2fbca55a741b7
ms.sourcegitcommit: a34d166d01e0a0a0f7d36593ad69b93e923d778b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/26/2020
ms.locfileid: "46895579"
---
# <a name="update-learning-pathways"></a>Atualizar os caminhos de aprendizagem
Se você tiver um site de cursores de aprendizado existente, poderá atualizá-lo para suporte multilíngue. Para atualizar os caminhos de aprendizado para a versão 4,0 multilíngue, você carrega o pacote de Web Parts, customlearning. sppkg, para o catálogo de aplicativos de locatários do SharePoint. Ao atualizar os caminhos de aprendizado:  

- Todas as playlists e ativos personalizados criados anteriormente são mantidos
- As configurações para ocultar ou Mostrar conteúdo são mantidas
- O modelo de cursores de aprendizado do SharePoint permanece inalterado
- As páginas do site de cursores de aprendizado não são traduzidas. Esse trabalho deve ser feito manualmente

## <a name="read-the-learning-pathways-multilingual-overview"></a>Ler os caminhos de aprendizado visão geral multilíngue
Para saber mais sobre como o suporte multilíngue funciona para os caminhos de aprendizado, leia a [visão geral multilíngue dos caminhos de aprendizado](custom_overview.md). 

## <a name="prerequisites-to-update"></a>Pré-requisitos para atualizar
Antes de atualizar os caminhos de aprendizado, o seguinte pré-requisito deve ser atendido:
- A pessoa que está atualizando os caminhos de aprendizado deve ser um proprietário do conjunto de sites do catálogo de aplicativos do locatário. Se os caminhos de aprendizado de provisionamento de pessoa não forem proprietários de conjunto de sites do catálogo de aplicativos, [conclua estas instruções](addappadmin.md) e continue. 

## <a name="set-language-settings"></a>Definir configurações de idioma 
Antes de atualizar os caminhos de aprendizado, defina as configurações de idioma do site. Para habilitar o suporte multilíngue para o site de cursores de aprendizado, você pode definir as **páginas habilitadas e as notícias a serem traduzidas em vários idiomas** **e, em seguida, adicionar**os idiomas que você deseja dar suporte ao site.
1.  No site de cursores de aprendizado, selecione **configurações** no canto superior direito e, em seguida, selecione **informações do site**.
2.  Na parte inferior do painel de informações do site, selecione **Exibir todas as configurações do site**.
3.  Em **Administração do site**, selecione **configurações de idioma**.
4.  Em **habilitar páginas e notícias a serem traduzidas em vários idiomas**, defina a opção Alternar. 
- Para um site do multiligual, deslize o botão para **Ativar**e, em seguida, prossiga para a seção Adicionar idiomas. 
- Para um site somente em inglês, deslize a alternância para **desativar**.

### <a name="add-languages"></a>Adicionar idiomas
Os caminhos de aprendizado dão suporte a nove idiomas, você deve adicionar somente os idiomas necessários. Nos exemplos usados nesta documentação, o italiano será adicionado. 
- Em **Adicionar ou remover idiomas do site**, comece a digitar o nome de um idioma em **selecionar ou digite um idioma**ou escolha um idioma na lista suspensa. Você pode repetir essa etapa para adicionar vários idiomas. Você pode adicionar ou remover idiomas do seu site a qualquer momento, voltando para esta página.
 
### <a name="assign-translators"></a>Atribuir tradutores
Ao definir as configurações de idioma para os caminhos de aprendizado, você pode atribuir tradutores. Os tradutores devem ter um perfil de idioma estrangeiro configurado. Para obter mais informações sobre perfis de idioma estrangeiros, consulte [criar sites de comunicação multilíngue, páginas e notícias](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).  
- Para obter um idioma com suporte, clique em **selecionar ou digite um tradutor** e selecione um conversor. 

## <a name="update-the-learning-pathways-web-part-package"></a>Atualizar o pacote de Web Part de cursores de aprendizado
Nesta etapa, você carrega a Web Part caminhos de aprendizado 4,0 para o catálogo de aplicativos do SharePoint e, em seguida, navega até a página de administração de caminhos de aprendizado para iniciar o processo de atualização.

### <a name="upload-the-web-part-package"></a>Carregar o pacote de Web Part
1.  Vá para o [repositório de aprendizado personalizado do GitHub](https://github.com/pnp/custom-learning-office-365/tree/master/webpart), selecione **customlearning. sppkg** e baixe-o para uma unidade local em seu computador.
2.  Se você ainda não tiver entrado, entre em seu locatário com uma conta de administrador de locatário ou de administrador de conjunto de sites. 
3.  Clique em **Administração**  >  **Mostrar todos os**  >  **recursos do SharePoint**  >  **More Features**. 
4.  Em **aplicativos**, clique em **abrir**. 
5.  Clique em **Catálogo**  >  **de aplicativos distribuir aplicativos para SharePoint**. 
6.  Clique em **carregar**  >  **escolher arquivos**. 
7.  Selecione o arquivo **customlearning. sppkg** que você baixou, clique em **OK**  >  **implantar**. 

### <a name="complete-the-update"></a>Concluir a atualização
1.  No site de cursores de aprendizado, selecione **Administração de cursores de aprendizado** no menu **página inicial** . 
2.  Você verá um prompt perguntando se você deseja atualizar. 
![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)
3.  Clique em **Iniciar**. 
4. Quando a atualização for concluída, clique em **fechar**. 

### <a name="next-steps"></a>Próximas etapas
- Explore o [conteúdo padrão](custom_exploresite.md) fornecido no site e na Web Part.
- Para obter mais informações sobre a tradução de páginas de sites, consulte [traduzir páginas de sites](custom_translate_page_ml.md). 

