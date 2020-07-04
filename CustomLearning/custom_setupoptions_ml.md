---
author: pkrebs
ms.author: pkrebs
title: Opções de configuração para caminhos de aprendizado multilíngues
ms.date: 07/6/2020
description: Opções de configuração para caminhos de aprendizado multilíngues
ROBOTS: NOINDEX, NOFOLLOW
ms.openlocfilehash: 2e2e7a765a7d24ef83a04f0ca3ef6d049cc658e3
ms.sourcegitcommit: 1e6e31d2bd43971b62322c7d2db352961c554d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/04/2020
ms.locfileid: "45037213"
---
# <a name="setup-options-for-multilingual-learning-pathways"></a>Opções de configuração para caminhos de aprendizado multilíngues
Com o lançamento de recursos multilíngues para sites de comunicação do SharePoint Online, os caminhos de aprendizado agora oferecem suporte para vários idiomas. Você pode configurar os caminhos de aprendizado em diferentes tipos de formas para atender às necessidades da sua organização. Para ajudá-lo a decidir o melhor caminho para sua organização, descrevemos as opções de instalação. 

## <a name="new-install-scenarios"></a>Novos cenários de instalação
Os "novos cenários de instalação" explicam as opções para instalar uma nova instância dos caminhos de aprendizado usando o serviço de provisionamento do SharePoint, agora disponível no livro de aparência do SharePoint.

### <a name="scenario-1-we-have-not-installed-learning-pathways-and-need-learning-pathways-multilingual-support"></a>Cenário 1: não foram instalados os caminhos de aprendizado e precisam de cursores de aprendizado suporte multilíngue 
Se você não tiver instalado os caminhos de aprendizado e precisar de vários idiomas, poderá usar o serviço de provisionamento do SharePoint para instalar uma nova solução de cursores de aprendizado com suporte para nove idiomas. Inglês será o idioma padrão e não poderá ser alterado. 
- Para provisionar uma nova solução de cursores de aprendizado com o inglês como o idioma padrão do site, confira [provisionar uma nova solução de cursores de aprendizado](custom_provision_ml.md).

### <a name="scenario-2-we-installed-learning-pathways-but-arent-currently-using-it-andor-havent-made-any-customization-to-the-site-or-playlists"></a>Cenário 2: instalamos os caminhos de aprendizado, mas não o utilizam atualmente e/ou não fizeram nenhuma personalização no site ou nas listas de reprodução 
Se você instalou os cursores de aprendizado, mas não o usar ativamente ou se não tiver feito nenhuma personalização no site ou nas listas de reprodução, poderá usar o serviço de provisionamento do SharePoint para instalar uma nova solução com suporte para nove idiomas. Inglês será o idioma padrão e não poderá ser alterado. 
- Para provisionar uma nova solução de cursores de aprendizado com o inglês como o idioma padrão do site, confira [provisionar uma nova solução de cursores de aprendizado](custom_provision_ml.md).

### <a name="scenario-3-we-havent-installed-learning-pathways-and-dont-need-multilingual-support"></a>Cenário 3: não instalamos os caminhos de aprendizado e não precisam de suporte multilíngue 
Se você não tiver instalado os caminhos de aprendizado e não precisar de suporte multilíngue, você poderá instalá-lo a partir do serviço de provisionamento do SharePoint. Inglês será o idioma padrão. Após a instalação, você precisa desativar o suporte multilíngue. 
- Para provisionar uma nova solução de cursores de aprendizado sem suporte multilíngue, confira [provisionar uma nova solução de cursores de aprendizado](custom_provision_ml.md).

## <a name="update-learning-pathways-with-a-web-part-upload-scenarios"></a>Cenários de atualização de cursores de aprendizado (com um carregamento de Web Part)
Se você tiver uma versão existente dos caminhos de aprendizado instalados, você poderá carregar a Web Part de caminhos de aprendizado para o catálogo de aplicativos do SharePoint para habilitar o suporte multilíngue. 

### <a name="scenario-1-we-need-to-upgrade-an-existing-version-of-learning-pathways-but-dont-need-multilingual-support"></a>Cenário 1: precisamos atualizar uma versão existente dos caminhos de aprendizado, mas não é necessário suporte multilíngue
Você pode atualizar os caminhos de aprendizado versão 4,0 sem suporte multilíngue. Com a atualização, você obtém alguns novos recursos, incluindo um seletor de imagem para listas de reprodução e subcategorias personalizadas. 

- Para atualizar uma solução de cursores de aprendizado existente sem suporte multilíngue, consulte [Atualizar caminhos de aprendizado para suporte multilíngue](custom_update_ml.md). O processo de atualização para nenhum suporte multilíngue é o mesmo que o suporte multilíngue, mas com menos etapas. 

### <a name="scenario-2-we-need-to-upgrade-to-multilingual-support-and-the-default-language-of-the-site-collection-is-our-default-language"></a>Cenário 2: precisamos atualizar para o suporte multilíngue e o idioma padrão do conjunto de sites é nosso idioma padrão
Cursores de aprendizado versão 4. O oferecerá suporte a páginas multilíngues no seu conjunto de sites. Além do suporte multilíngue, você obtém alguns novos recursos, incluindo um seletor de imagem para listas de reprodução e subcategorias personalizadas. 
- Para atualizar um site de cursores de aprendizado existente suporte multilíngue, confira [Atualizar caminhos de aprendizado para suporte multilíngue](custom_update_ml.md). 

## <a name="update-learning-pathways-for-multilingual-support-with-manual-install"></a>Atualizar os caminhos de aprendizado para suporte multilíngue com instalação manual 
O exemplo a seguir descreve os cenários para atualização de uma instância existente da solução de cursores de aprendizado para a versão 4,0 multilíngue, instalando manualmente a Web Part de caminhos de aprendizado. 

### <a name="scenario-1-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--no-custom-content"></a>Cenário 1: precisamos de suporte multilíngue e o idioma padrão do conjunto de sites não é nosso idioma padrão, sem conteúdo personalizado 
Os caminhos de aprendizado versão 4,0 oferecerão suporte a esse cenário. No entanto, esse cenário pressupõe que você não tenha conteúdo personalizado ou listas de reprodução no site existente. Para este cenário, você pode criar um novo site de comunicação do SharePoint Online com o idioma padrão, carregar a Web Part e, em seguida, configurar manualmente os caminhos de aprendizado com um script do PowerShell. 
- Para configurar os caminhos de aprendizado para suporte multilíngue com seu idioma padrão, confira [instalação manual dos caminhos de aprendizado para suporte multilíngue](custom_manualsetup_ml.md).

### <a name="scenario-2-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--plus-we-have-custom-content"></a>Cenário 2: precisamos de suporte multilíngue e o idioma padrão do conjunto de sites não é nosso idioma padrão – além disso, temos conteúdo personalizado 
Para este cenário, você pode criar um novo site de comunicação do SharePoint Online com o idioma padrão, carregar a Web Part e, em seguida, configurar manualmente os caminhos de aprendizado com um script do PowerShell. 

Após restabelecer o site de cursores de aprendizado seguindo as etapas acima, você precisará mover o conteúdo de sua lista do **CustomPlaylists** e sua lista do **CustomAssets** . Você também pode, opcionalmente, mover as páginas personalizadas reais que compõem seus ativos personalizados se residirem no site de cursores de aprendizado existentes e sua intenção é excluí-lo. A tarefa pode ser difícil porque para todos os itens na lista **CustomPlaylists** , a ID do item de lista na lista **CustomAssets** é incluída no campo JSONData de cada item de lista de playlist. Portanto, simplesmente mover o conteúdo da lista **CustomPlaylists** de um site para outro não será suficiente. Além disso, a lista **CustomAssets** contém a URL absoluta para a página do ativo personalizado no campo JSONData do item de lista. Se os ativos não forem movidos e o site não for renomeado (alterando, assim, a URL absoluta para a página do ativo), o **CustomAssets** poderá permanecer. Mas será necessário corrigir manualmente as entradas. Dada a complexidade desse tipo de migração sugerimos que você considere a lista de um dos nossos cursores de aprendizado para ajudá-lo a fazer essa transição.
- Para configurar os caminhos de aprendizado para suporte multilíngue com seu idioma padrão, confira [instalação manual dos caminhos de aprendizado para suporte multilíngue](custom_manualsetup_ml.md).

