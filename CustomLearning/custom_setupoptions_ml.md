---
author: pkrebs
ms.author: pkrebs
title: Opções de instalação para caminhos de aprendizado multilíngues
ms.date: 07/6/2020
description: Opções de instalação para caminhos de aprendizado multilíngues
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 1384885adc1d7119658bf968e18e8859c784ef37
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999307"
---
# <a name="setup-options-for-multilingual-learning-pathways"></a>Opções de instalação para caminhos de aprendizado multilíngues
Com a versão de recursos multilíngues para sites de comunicação do SharePoint Online, os caminhos de aprendizado agora oferecem suporte para vários idiomas. Você pode configurar caminhos de aprendizado de diferentes tipos de maneiras para atender às necessidades da sua organização. Para ajudá-lo a decidir o melhor caminho para sua organização, descrevemos as opções de instalação. 

## <a name="new-install-scenarios"></a>Novos cenários de instalação
Os "novos cenários de instalação" explicam as opções para instalar uma nova instância dos caminhos de aprendizado usando o Serviço de Provisionamento do SharePoint, agora disponível no look book do SharePoint.

### <a name="scenario-1-we-have-not-installed-learning-pathways-and-need-learning-pathways-multilingual-support"></a>Cenário 1: não instalamos caminhos de aprendizado e precisamos de suporte multilíngue de caminhos de aprendizagem 
Se você não tiver instalado os caminhos de aprendizado e precisar dele em vários idiomas, poderá usar o Serviço de Provisionamento do SharePoint para instalar uma nova solução de caminhos de aprendizado com suporte para nove idiomas. O inglês será o idioma padrão e não poderá ser alterado. 
- Para provisionar uma nova solução de caminhos de aprendizado com o inglês como idioma padrão para o site, consulte [Provisionar uma nova solução](custom_provision_ml.md)de caminhos de aprendizado.

### <a name="scenario-2-we-installed-learning-pathways-but-arent-currently-using-it-andor-havent-made-any-customization-to-the-site-or-playlists"></a>Cenário 2: Instalamos caminhos de aprendizado, mas não estamos usando-o no momento e/ou não fizemos nenhuma personalização para o site ou playlists 
Se você instalou caminhos de aprendizado, mas não está usando ativamente ou não fez nenhuma personalização para o site ou listas de reprodução, você pode usar o Serviço de Provisionamento do SharePoint para instalar uma nova solução com suporte para nove idiomas. O inglês será o idioma padrão e não poderá ser alterado. 
- Para provisionar uma nova solução de caminhos de aprendizado com o inglês como idioma padrão para o site, consulte [Provisionar uma nova solução](custom_provision_ml.md)de caminhos de aprendizado.

### <a name="scenario-3-we-havent-installed-learning-pathways-and-dont-need-multilingual-support"></a>Cenário 3: não instalamos caminhos de aprendizado e não precisamos de suporte multilíngue 
Se você não tiver instalado os caminhos de aprendizado e não precisar de suporte multilíngue, poderá instalá-lo do Serviço de Provisionamento do SharePoint. O inglês será o idioma padrão. Após a instalação, você precisa desativar o suporte multilíngue. 
- Para provisionar uma nova solução de caminhos de aprendizado sem suporte multilíngue, consulte [Provisionar uma nova solução de caminhos de aprendizado.](custom_provision_ml.md)

## <a name="update-learning-pathways-with-a-web-part-upload-scenarios"></a>Atualizar os caminhos de aprendizado (com um carregamento de Web Part) cenários
Se você tiver uma versão existente dos caminhos de aprendizado instalados, poderá carregar a Web Part de caminhos de aprendizado para o Catálogo de Aplicativos do SharePoint para habilitar o suporte multilíngue. 

### <a name="scenario-1-we-need-to-upgrade-an-existing-version-of-learning-pathways-but-dont-need-multilingual-support"></a>Cenário 1: precisamos atualizar uma versão existente dos caminhos de aprendizado, mas não precisamos de suporte multilíngue
Você pode atualizar os caminhos de aprendizado versão 4.0 sem suporte multilíngue. Com a atualização, você recebe alguns novos recursos, incluindo um seletor de imagem para playlists personalizadas e subcategorias. 

- Para atualizar uma solução de caminhos de aprendizado existentes sem suporte multilíngue, consulte [Update learning pathways for multilingual support](custom_update_ml.md). O processo de atualização para nenhum suporte multilíngue é o mesmo que com o suporte multilíngue, mas com menos etapas. 

### <a name="scenario-2-we-need-to-upgrade-to-multilingual-support-and-the-default-language-of-the-site-collection-is-our-default-language"></a>Cenário 2: precisamos atualizar para o suporte multilíngue e o idioma padrão do conjunto de sites é nosso idioma padrão
Os caminhos de aprendizado versão 4.O darão suporte a páginas multilíngues em seu conjunto de sites. Além do suporte multilíngue, você recebe alguns novos recursos, incluindo um seletor de imagens para playlists personalizadas e subcategorias. 
- Para atualizar um suporte multilíngue de caminhos de aprendizado existentes, consulte Atualizar caminhos de aprendizado para suporte [multilíngue.](custom_update_ml.md) 

## <a name="update-learning-pathways-for-multilingual-support-with-manual-install"></a>Atualizar caminhos de aprendizado para suporte multilíngue com instalação manual 
Os seguintes descreve os cenários para atualizar uma instância existente da solução de caminhos de aprendizagem para a versão 4.0 multilíngue instalando manualmente a Web Part de caminhos de aprendizado. 

### <a name="scenario-1-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--no-custom-content"></a>Cenário 1: precisamos de suporte multilíngue e o idioma padrão do conjunto de sites não é nosso idioma padrão – nenhum conteúdo personalizado 
Os caminhos de aprendizado versão 4.0 darão suporte a esse cenário. No entanto, esse cenário supõe que você não tenha conteúdo personalizado ou playlists no site existente. Para esse cenário, você pode criar um novo site de comunicação do SharePoint Online com seu idioma padrão, carregar a Web Part e configurar manualmente os caminhos de aprendizado com um Script do PowerShell. 
- Para configurar caminhos de aprendizado para suporte multilíngue com seu idioma padrão, consulte Instalação Manual de Caminhos de Aprendizagem para suporte [multilíngue.](custom_manualsetup_ml.md)

### <a name="scenario-2-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--plus-we-have-custom-content"></a>Cenário 2: precisamos de suporte multilíngue e o idioma padrão do conjunto de sites não é nosso idioma padrão , além disso, temos conteúdo personalizado 
Para esse cenário, você pode criar um novo site de comunicação do SharePoint Online com seu idioma padrão, carregar a Web Part e configurar manualmente os caminhos de aprendizado com um Script do PowerShell. 

Depois de restabelecer seu site de caminhos de aprendizado seguindo as etapas acima, você precisará mover o conteúdo da sua lista **CustomPlaylists** e sua **lista CustomAssets.** Você também pode, opcionalmente, mover as páginas personalizadas reais que comem seus ativos personalizados se elas morarem no site de caminhos de aprendizado existentes, e sua intenção é excluí-la. A tarefa pode ser difícil porque, para todos os itens na lista **CustomPlaylists,** a ID do item de lista na lista **CustomAssets** é sepultada no campo JSONData de cada item de lista de playlist. Portanto, simplesmente mover o conteúdo da lista **CustomPlaylists** de um site para o outro não será suficiente. Além disso, **a lista CustomAssets** contém a URL absoluta para a página do ativo personalizado no campo JSONData do item de lista. Se os ativos não são movidos e o site não é renomeado (alterando a URL absoluta para a página do ativo), **CustomAssets** poderá permanecer. Mas você precisará corrigir manualmente as entradas. Dada a complexidade desse tipo de migração, sugerimos que você considere inscrever um de nossos parceiros de caminhos de aprendizado para ajudá-lo a fazer essa transição.
- Para configurar caminhos de aprendizado para suporte multilíngue com seu idioma padrão, consulte Instalação Manual de Caminhos de Aprendizagem para suporte [multilíngue.](custom_manualsetup_ml.md)

