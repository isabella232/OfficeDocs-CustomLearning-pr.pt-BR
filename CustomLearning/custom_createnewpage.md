---
author: pkrebs
ms.author: pkrebs
title: Criar páginas do SharePoint para playlists
ms.date: 02/10/2019
description: Criar páginas do SharePoint para playlists
ms.service: sharepoint-online
ms.openlocfilehash: 40c249fbd5b0fdaefd555f23bf20ac23240ea954
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999082"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a>Criar páginas do SharePoint para playlists personalizadas

Um dos recursos exclusivos dos caminhos de aprendizado é a capacidade de criar listas de reprodução que são montadas a partir de ativos da Microsoft e dos ativos do SharePoint que você cria. Neste exemplo, criaremos uma página do SharePoint antes de criar uma playlist. A capacidade de criar playlists a partir de páginas do SharePoint oferece várias oportunidades para criar páginas usando as Web Parts disponíveis da Microsoft ou da sua organização. Por exemplo, uma playlist pode incluir uma página do SharePoint com vídeos incorporados do YouTube ou um formulário criado a partir do Office 365 Forms ou um relatório do Power BI incorporado. Neste exemplo, mostraremos como criar uma página com a Web Part Incorporar e a Web Part Texto.  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a>Criar uma página do SharePoint para uma playlist personalizada

1. Clique no ícone **engrenagem** do SharePoint e clique **em Adicionar uma página**.
2. Clique **em Adicionar uma nova seção (+)** no lado esquerdo da página e clique em Duas **Colunas** para o layout da seção.
3. Na coluna esquerda, clique em + e clique na Web Part **Incorporar.** 
4. Na coluna direita, clique em +e clique na Web Part **Texto.** Sua página deve ter esta aparência.

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a>Adicionar um vídeo e texto do YouTube

1. No navegador, vá para o YouTube. Para este exemplo, pesquise "O que é o Office 365 – os melhores aplicativos de produtividade da Microsoft".
2. Clique no vídeo para reproduzi-lo, pause-o e clique com o botão direito do mouse nele. 
3. Clique **em Copiar código de incorporar** e, em seguida, retorne à página do SharePoint. 
4. Clique **em Adicionar código de** incorporar na Web Part Incorporar e, em seguida, adicione o código do vídeo do YouTube. 
5. Volte para a página do YouTube e copie o texto **Descrição** do vídeo. 
6. Retorne à página do SharePoint, selecione a Web Part **Texto** e copie o texto do vídeo do YouTube.
7. Selecione o **ícone editar web part** na área Título da página do SharePoint e, em seguida, nomee a página "Introdução personalizada da playlist". 
8. Para **Layout,** selecione **Plain**, em seguida, feche o painel de propriedades **da** Região de Título. A página agora deve ter uma aparência parecida com a seguinte. 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a>Publicar a página

- Selecione o **botão Publicar.** Agora você está pronto para adicionar essa página do SharePoint à sua playlist personalizada. 