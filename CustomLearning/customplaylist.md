---
author: karuanag
ms.author: karuanag
manager: alexb
title: Personalizar e compartilhar playlists
ms.date: 02/10/2019
description: Criar playlists personalizadas de conteúdo existente ou páginas SharePoint novas
ms.service: sharepoint-online
audience: itpro
ms.topic: article
ms.openlocfilehash: 31310a6737543a3006f810ffc6b9522d6c9583da
ms.sourcegitcommit: a93cae8ea6e3c1141d7266d04131b69f2c2498cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2021
ms.locfileid: "59485332"
---
# <a name="customize-and-share-playlists"></a>Personalizar e compartilhar playlists

## <a name="create-a-playlist"></a>Criar uma playlist

Uma playlist é uma compilação de "assets". Um "ativo" é uma página SharePoint ou item existente do conteúdo de treinamento da Microsoft. Ao criar uma playlist, você seleciona ativos que se juntam para criar um caminho de aprendizado para o usuário.  

O benefício de adicionar SharePoint páginas é que você pode criar páginas SharePoint com vídeos ou vídeos do YouTube hospedados em sua organização. Você também pode criar páginas com Formulários ou outros Office 365 conteúdo.  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a>Etapa 1: Criar uma página SharePoint para sua playlist
Neste exemplo, primeiro criaremos uma página SharePoint para adicionar à playlist. Criaremos uma página com uma Web Part de vídeo do YouTube e Uma Web Part text.  Estas instruções pressuem que você está usando o serviço SharePoint Online. 

#### <a name="create-a-new-page"></a>Criar uma página
1.  Selecione o Configurações menu > Conteúdo do Site > Páginas do Site > Página > Site Novo.
2.  Na área título, digite Usar a caixa de Teams comando
3.  Selecione a seção Adicionar uma nova e selecione Duas Colunas.

    ![adicionar duas colunas](media/clo365addtwocolumn.png)

4.  Na caixa à esquerda, selecione Adicionar uma nova Web Part e selecione Incorporar. 
5.  Em um navegador da Web, vá até essa URL e receba o código https://youtu.be/wYrRCRphrp0 de incorporar do vídeo. 
6.  Na web part SharePoint, selecione Adicionar código incorporar e, em seguida, colar-o na caixa Incorporar. 
7.  Na caixa à direita, selecione Adicionar uma nova Web Part e selecione Texto. 
8.  Em um navegador da Web, acesse esta URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b e copie o Try it! Instruções da página e colar-as na Web Part texto. Sua página deve ter a seguinte aparência. 
   ![Página incorporar](media/clo365teamscommandbox.png)
9.  Clique **em** Publicar e, em seguida, copie a URL da página e a colar em Bloco de notas

#### <a name="step-2-create-the-playlist"></a>Etapa 2: Criar a playlist

1. Navegue até **a página Administração Learning personalizado** em sua experiência de site.
   ![Administrador personalizado](media/custom_admin.png)
1. Certifique-se **de que Category** está selecionado 
1. Clique na categoria na qual você gostaria que sua nova playlist fosse exibida
1. Ao lado do nome da categoria, clique no símbolo de adição ![ Lista de reprodução personalizada](media/custom_addplay.png)

1. Preencha os valores conforme mostrado no exemplo abaixo e selecione **Criar**. 
  ![Detalhes personalizados da lista de reprodução](media/custom_details.png)
- **Título** - Nome de exibição da playlist
- **Descrição** - Informações sobre o que será aprendido
- **Categoria** - Pré-selecionado com base em sua seleção inicial
- **Sub Category** - Pré-selecionado com base em sua seleção inicial
- **Tecnologia** - Selecione conforme aplicável
- **Nível** - Iniciante, Intermediário ou Avançado
- **Público-** Isso permite direcionar conteúdo com base em uma lista pré-definida de funções fornecidas pela Microsoft.

6. Clique **em Salvar Detalhes**

> [!TIP]
> Você pode personalizar a imagem do ícone da sua playlist.  Clique no ícone da imagem e insira uma URL de uma imagem carregada anteriormente.  Certifique-se de que a imagem está localizada no conjunto Learning site personalizado ou em outro local que todos os usuários terão acesso ao arquivo.  
![Imagem personalizada](media/custom_image.png)

#### <a name="step-3-add-assets-to-the-playlist"></a>Etapa 3: Adicionar ativos à playlist
Nesta etapa, você adicionará ativos existentes da Microsoft e a página SharePoint que você criou à playlist. 

1. Depois de salvar os detalhes da playlist, você pode usar a Pesquisa de Ativos Existentes.
1. **Insira em qualquer termo de pesquisa** para ver uma lista de ativos predefinidos que estão disponíveis em outras listas de reprodução. **Clique no nome de** um ativo para incluí-lo em sua nova playlist.

    ![Playlist de pesquisa personalizada](media/custom_slist.png)

Você também pode adicionar a página SharePoint criada anteriormente ou criar uma do zero na experiência.

1. Clique na opção **Novo Ativo** na caixa de diálogo Ativos de Playlist
1. Dê a seu ativo um **Título**. Depois de inserido, opções adicionais exibirão ![ Página nova personalizada](media/custom_newpage.png)
1. Agora você pode criar uma nova página de ativos no SharePoint Online ou inserir a URL de uma página existente para adicioná-la à sua playlist personalizada. 
1. **Os** campos Categoria **, Sub** Categoria e **Tecnologia** serão pré-preenchidos com base em suas seleções anteriores para esta playlist.
1. Faça as seleções apropriadas para Nível e Audiência para esse ativo individual.  
1. Clique **em Salvar Ativo** para adicioná-lo à playlist personalizada
1. Repita estas etapas, pesquisando ou adicionando páginas individuais, até que sua playlist seja concluída. 
1. Clique **em Fechar Playlist** para salvar

Sua playlist com esse conteúdo agora estará disponível em qualquer lugar em que você instalou/insiou a Web Part Learning Custom. 

> [!NOTE]
> Se você cometer um erro depois de fechar a playlist, poderá excluí-la da categoria clicando no X ao lado do nome da playlist.  

#### <a name="things-to-think-about"></a>Coisas para pensar

Listas de reprodução personalizadas podem ser usadas para ajudar os usuários finais em várias tarefas.  Você tem um formulário de solicitação de tempo de folga?  Um formulário para solicitar equipamento de hardware?  Todos os ativos de treinamento existentes podem ser programados na experiência.  

## <a name="share-playlists"></a>Compartilhar Playlists

1. Navegue até qualquer playlist dentro da web part ou experiência do site
1. No canto superior esquerdo, você verá três ícones
1. Clique no ícone que representa um link
1. Copie a URL para a playlist

   ![Compartilhar playlist Essa URL agora pode ser inserida na navegação do site ou usada em outras comunicações para levar seus funcionários ](media/share.png) diretamente para essa playlist. 

### <a name="next-steps---drive-adoption"></a>Próximas etapas - [Impulsionar a adoção](driveadoption.md)
