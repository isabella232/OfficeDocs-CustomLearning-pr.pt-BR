---
author: karuanag
ms.author: karuanag
title: Perguntas frequentes para o aprendizado de sinalizador para soluções do Office 365
ms.date: 02/10/2019
description: Perguntas frequentes informações de perguntas para o aprendizado personalizado para o Office 365
ms.openlocfilehash: d8b5104e8feeaa4e70296f61594233b27363481b
ms.sourcegitcommit: f93a6a691331515ba10f4d43b491928ec268f0ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29952585"
---
# <a name="frequently-asked-questions"></a>Perguntas Frequentes

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a>1. quais são os requisitos para instalar o aprendizado personalizado para o Office 365 em meu ambiente locatário?

- SharePoint Online e os Sites de comunicação habilitados.
- O indivíduo que vai ser provisionamento CLO365 deve ser o administrador de locatário do inquilino destino para a instalação.
- Um locatário 'App Catalog' deve estar disponível na opção 'Apps' do Centro de administração do SharePoint.
- O indivíduo que vai ser provisionamento CLO365 deve ser um administrador de conjunto de sites do catálogo de aplicativos no locatário destino para a instalação.

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a>2. quais idiomas está disponível na aprendizagem personalizado para o Office 365?

Sinalizador de aprendizagem do Office 365 está atualmente disponível apenas em inglês. O provisionamento automático de ponta a ponta funciona somente com locatários em inglês. Idiomas adicionais podem ser adicionados em futuras versões.

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>3. quanto tempo levará para instalar o site em nosso ambiente de locatário?

Com base em nossos testes da instalação, ele deve levar menos de 15 minutos. Isso não incluir o tempo necessário para personalizar o site às suas necessidades.

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a>4. podemos tornar o sinalizador de aprendizagem do Office 365 um subsite de nosso principal conjunto de sites do SharePoint?

Não. O site baseia-se em um modelo de site de comunicação, que sempre deve ser um conjunto de sites raiz.

> [!NOTE]
> É importante considerar as permissões que os usuários finais precisará acessar o site. A maioria das organizações definiu a grupos de segurança ou de usuário. Você deve adicionar grupos de segurança apropriados para seu novo portal de treinamento, quando você estiver pronto para iniciá-lo à sua comunidade de funcionário.

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a>5. eu preciso reinstalar o site; o que deve fazer?

Execute a instalação instruções publicado [aqui](installsitepackage.md).

> [!NOTE]
> Se você tiver desabilitado a telemetria na sua instalação anterior e gostaria de continuar com a telemetria desabilitada, você precisará siga as instruções para desabilitar a telemetria aqui.

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>6. que fizemos atualizações à nossa implementação de aprendizado personalizado para o Office 365. Podemos perderá essas atualizações (feitas ao modelo de sites, listas de reprodução) se podemos reinstalar o site?

Personalizações páginas individuais e listas de reprodução personalizadas serão perdidas se você reinstalar o site sobre sua instalação atual.  