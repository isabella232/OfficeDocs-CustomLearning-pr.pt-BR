---
author: pkrebs
ms.author: pkrebs
title: Opções de configuração para caminhos de aprendizado multilíngues
ms.date: 07/6/2020
description: Opções de configuração para caminhos de aprendizado multilíngues
ROBOTS: NOINDEX, NOFOLLOW
ms.openlocfilehash: e9e2c74f366dedf8e0010a01797aedb3c3316fa4
ms.sourcegitcommit: 1f080ed4cf3687f922907304db3fd7a06aa9d501
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2020
ms.locfileid: "45031687"
---
# <a name="setup-options-for-multilingual-learning-pathways"></a>Opções de configuração para caminhos de aprendizado multilíngues
Com o lançamento de recursos multilíngues para sites de comunicação do SharePoint Online, os caminhos de aprendizado agora oferecem suporte para vários idiomas. A maneira como você configura os caminhos de aprendizado para o suporte multilíngue depende das necessidades da sua organização. Para ajudá-lo a decidir o melhor caminho para sua organização, descrevemos os possíveis cenários.

## <a name="new-install-scenarios"></a>Novos cenários de instalação
O exemplo a seguir descreve os cenários de instalação de uma nova instância da solução de cursores de aprendizado usando o serviço de provisionamento do SharePoint, agora disponível no livro de aparência do SharePoint.

### <a name="scenario-1-we-have-not-installed-learning-pathways-and-need-learning-pathways-multilingual-support"></a>Cenário 1: não foram instalados os caminhos de aprendizado e precisam de cursores de aprendizado suporte multilíngue 
Se você não tiver instalado os caminhos de aprendizado e precisar de vários idiomas, poderá usar o serviço de provisionamento do SharePoint para criar um novo site de caminhos de aprendizado em nove idiomas. Inglês será o idioma padrão e não poderá ser alterado. 
- Para provisionar uma nova solução de cursores de aprendizado com o inglês como o idioma padrão do site, confira [provisionar uma nova solução de cursores de aprendizado](custom_provision_ml.md).

### <a name="scenario-2-we-installed-learning-pathways-but-arent-currently-using-it-andor-havent-made-any-customization-to-the-site-or-playlists"></a>Cenário 2: instalamos os caminhos de aprendizado, mas não o utilizam atualmente e/ou não fizeram nenhuma personalização no site ou nas listas de reprodução 
Se você tiver instalado os caminhos de aprendizado, mas não o usar ativamente ou se não tiver feito nenhuma personalização no site ou nas listas de reprodução, poderá usar o serviço de provisionamento do SharePoint para criar um novo site em nove idiomas. Inglês será o idioma padrão e não poderá ser alterado. 
- Para provisionar uma nova solução de cursores de aprendizado com o inglês como o idioma padrão do site, confira [provisionar uma nova solução de cursores de aprendizado](custom_provision_ml.md).

### <a name="scenario-3-we-have-not-installed-learning-pathways-and-dont-need-multilingual-support"></a>Cenário 3: não foi instalado o cursores de aprendizado e não é necessário suporte multilíngue 
Se você não tiver instalado os caminhos de aprendizado anteriormente e não precisar de suporte multilíngue, poderá provisionar os caminhos de aprendizado do serviço de provisionamento do SharePoint. Inglês será o idioma padrão. Após a instalação, será necessário desativar o suporte multilíngue. 
- Para provisionar uma nova solução de cursores de aprendizado sem suporte multilíngue, confira [provisionar uma nova solução de cursores de aprendizado](custom_provision_ml.md).

## <a name="update-learning-pathways-with-web-part-upload-scenarios"></a>Atualizar os caminhos de aprendizado com cenários de carregamento de Web Part
O seguinte descreve os cenários para atualizar uma instância existente da solução de cursores de aprendizado para a versão 4,0 multilíngue. Com esse cenário, você carrega a Web Part de cursores de aprendizado no catálogo de aplicativos do SharePoint.

### <a name="scenario-1-we-need-to-upgrade-an-existing-version-of-learning-pathways-but-do-not-need-multilingual-support"></a>Cenário 1: precisamos atualizar uma versão existente dos caminhos de aprendizado, mas não precisam de suporte multilíngue
Você pode atualizar para o cursores de aprendizado versão 4,0 sem suporte multilíngue. Com a atualização, você obtém alguns novos recursos que podem ser úteis para você, incluindo um seletor de imagem para escolher a imagem de uma lista de reprodução personalizada e uma subcategoria personalizada. 

- Para atualizar um site de cursores de aprendizado existente sem suporte multilíngue, consulte [Atualizar caminhos de aprendizado para suporte multilíngue](custom_update_ml.md). O processo de atualização para nenhum suporte multilíngue é o mesmo que o suporte multilíngue, mas com menos etapas. 

### <a name="scenario-2-we-need-to-upgrade-to-multilingual-support-and-the-default-language-of-the-site-collection-is-our-default-language"></a>Cenário 2: precisamos atualizar para o suporte multilíngue e o idioma padrão do conjunto de sites é nosso idioma padrão
Caminhos de aprendizado versão 4. O oferecerá suporte ao recurso de páginas multilíngues no seu conjunto de sites. Além do suporte multilíngue, você obtém algumas atualizações que podem ser úteis para uma interface do usuário de seletor de imagem para escolher a imagem de uma lista de reprodução personalizada e a adição de uma interface do usuário para alterar a imagem padrão para uma subcategoria personalizada. 
- Para atualizar um site de cursores de aprendizado existente suporte multilíngue, confira [Atualizar caminhos de aprendizado para suporte multilíngue](custom_update_ml.md). 

## <a name="update-learning-pathways-for-multilingual-support-with-manual-install"></a>Atualizar os caminhos de aprendizado para suporte multilíngue com instalação manual 
O exemplo a seguir descreve os cenários para atualização de uma instância existente da solução de cursores de aprendizado para a versão 4,0 multilíngue, instalando manualmente a Web Part de caminhos de aprendizado. 

### <a name="scenario-1-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--no-custom-content"></a>Cenário 1: precisamos de suporte multilíngue e o idioma padrão do conjunto de sites não é nosso idioma padrão, sem conteúdo personalizado 
Os caminhos de aprendizado versão 4,0 oferecerão suporte a esse cenário. No entanto, esse cenário pressupõe que você não tenha conteúdo personalizado ou listas de reprodução no site existente. Para este cenário, você pode criar um novo site de comunicação do SharePoint Online com o idioma padrão, carregar a Web Part e, em seguida, configurar manualmente os caminhos de aprendizado com um script do PowerShell. 
- Para atualizar os caminhos de aprendizado para suporte multilíngue com seu idioma padrão, confira **instalação manual de caminhos de aprendizado para suporte multilíngue**.

### <a name="scenario-2-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--plus-we-have-custom-content"></a>Cenário 2: precisamos de suporte multilíngue e o idioma padrão do conjunto de sites não é nosso idioma padrão – além disso, temos conteúdo personalizado 
Para este cenário, você pode criar um novo site de comunicação do SharePoint Online com o idioma padrão, carregar a Web Part e, em seguida, configurar manualmente os caminhos de aprendizado com um script do PowerShell. Após restabelecer o site de cursores de aprendizado seguindo as etapas acima, você precisará mover o conteúdo de sua lista do **CustomPlaylists** e sua lista do **CustomAssets** . Você também pode, opcionalmente, mover as páginas personalizadas reais que compõem seus ativos personalizados se residirem no site de cursores de aprendizado existentes e sua intenção é excluí-lo. A tarefa pode ser difícil porque para todos os itens na lista **CustomPlaylists** , a ID do item de lista na lista **CustomAssets** é incluída no campo JSONData de cada item de lista de playlist. Portanto, simplesmente mover o conteúdo da lista **CustomPlaylists** de um site para outro não será suficiente. Além disso, a lista **CustomAssets** contém a URL absoluta para a página do ativo personalizado no campo JSONData do item de lista. Se os ativos não forem movidos e o site não for renomeado (alterando, assim, a URL absoluta para a página do ativo), o **CustomAssets** poderá permanecer. Mas será necessário corrigir manualmente as entradas. Dada a complexidade desse tipo de migração sugerimos que você considere a lista de um dos nossos cursores de aprendizado para ajudá-lo a fazer essa transição.
- Para atualizar os caminhos de aprendizado para suporte multilíngue com seu idioma padrão, confira **instalação manual de caminhos de aprendizado para suporte multilíngue**.

