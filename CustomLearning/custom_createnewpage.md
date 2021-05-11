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
# <a name="create-sharepoint-pages-for-custom-playlists"></a>Criar SharePoint páginas para playlists personalizadas

Um dos recursos exclusivos dos caminhos de aprendizado é a capacidade de criar listas de reprodução que são montadas a partir de ativos da Microsoft e SharePoint ativos que você cria. Neste exemplo, criaremos uma página SharePoint antes de criar uma playlist. A capacidade de criar playlists SharePoint páginas oferece várias oportunidades para criar páginas usando as Web Parts disponíveis da Microsoft ou da sua organização. Por exemplo, uma playlist pode incluir uma página de SharePoint com vídeos incorporados do YouTube ou um formulário criado a partir do Office 365 Forms ou um relatório Power BI incorporado. Neste exemplo, mostraremos como criar uma página com a Web Part Incorporar e a Web Part Texto.  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a>Criar uma SharePoint para uma playlist personalizada

1. Clique no SharePoint **de** engrenagem e clique **em Adicionar uma página.**
2. Clique **em Adicionar uma nova seção (+)** no lado esquerdo da página e clique em Duas **Colunas** para o layout da seção.
3. Na coluna esquerda, clique em + e clique na Web Part **Incorporar.** 
4. Na coluna direita, clique em +e clique na Web Part **Texto.** Sua página deve ter esta aparência.

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a>Adicionar um vídeo e texto do YouTube

1. No navegador, vá para o YouTube. Para este exemplo, pesquise "O que é Office 365 – os melhores aplicativos de produtividade da Microsoft".
2. Clique no vídeo para reproduzi-lo, pause-o e clique com o botão direito do mouse nele. 
3. Clique **em Copiar código de incorporar** e retorne à página SharePoint. 
4. Clique **em Adicionar código de** incorporar na Web Part Incorporar e, em seguida, adicione o código do vídeo do YouTube. 
5. Volte para a página do YouTube e copie o texto **Descrição** do vídeo. 
6. Volte para a página SharePoint, selecione a Web Part **Texto** e copie o texto do vídeo do YouTube.
7. Selecione o **ícone editar web part** na área Título da página SharePoint e, em seguida, nomee a página "Introdução personalizada da playlist". 
8. Para **Layout,** selecione **Plain**, em seguida, feche o painel de propriedades **da** Região de Título. A página agora deve ter uma aparência parecida com a seguinte. 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a>Publicar a página

- Selecione o **botão Publicar.** Agora você está pronto para adicionar essa página SharePoint à sua playlist personalizada. 