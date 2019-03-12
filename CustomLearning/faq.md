---
author: karuanag
ms.author: karuanag
title: Perguntas frequentes sobre o aprendizado personalizado para as soluções do Office 365
ms.date: 02/10/2019
description: Perguntas frequentes sobre o aprendizado personalizado para o Office 365
ms.openlocfilehash: 7da1f3da197fc298c83eac89e3455312cba7a851
ms.sourcegitcommit: c60ca83b784f36b6f41b56ac193f7d58c750984e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2019
ms.locfileid: "30543761"
---
# <a name="frequently-asked-questions"></a>Perguntas Frequentes

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a>1. quais são os requisitos para instalar o aprendizado personalizado para o Office 365 em meu ambiente de locatário?

- SharePoint Online e sites de comunicação habilitados.
- O indivíduo que será o provisionamento de CLO365 deve ser o administrador de locatários do locatário de destino para a instalação.
- Um "catálogo de aplicativos" do locatário deve estar disponível na opção "aplicativos" do centro de administração do SharePoint.
- O indivíduo que será o provisionamento de CLO365 deve ser um administrador de conjunto de sites do catálogo de aplicativos no locatário de destino para a instalação.

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a>2. quais idiomas são aprendizagem personalizada para o Office 365 disponível no?

O aprendizado personalizado para o Office 365 só está disponível no momento em inglês. O provisionamento automático de ponta a ponta funciona apenas com locatários em inglês. Idiomas adicionais podem ser adicionados em versões futuras.

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>3. quanto tempo levará para instalar o site em nosso ambiente de locatário?

Com base em nosso teste da instalação, deve levar menos de 15 minutos. Isso não inclui o tempo necessário para personalizar o site para seus requisitos.

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a>4. podemos fazer o aprendizado personalizado para o Office 365 um subsite de nosso conjunto de sites principal do SharePoint?

Não. O site é baseado em um modelo de site de comunicação, que sempre é destinado a ser um conjunto de sites raiz.

> [!NOTE]
> É importante considerar as permissões que os usuários finais precisarão acessar o site. A maioria das organizações definiu grupos de segurança ou de usuários. Você deve adicionar os grupos de segurança apropriados ao seu novo portal de treinamento quando estiver pronto para iniciá-lo na sua comunidade de funcionários.

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a>5. preciso reinstalar o site; o que devo fazer?

Siga as instruções de instalação publicadas [aqui](custom_provision.md).

> [!NOTE]
> Se você desabilitou a telemetria em sua instalação anterior e deseja continuar com a telemetria desabilitada, será necessário seguir as instruções para desabilitar a telemetria aqui.

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>6. fizemos atualizações para nossa implementação de aprendizado personalizado para o Office 365. Perderá essas atualizações (feitas no modelo de site, nas listas de reprodução) se reinstalarmos o site?

As personalizações para páginas individuais e listas de reprodução personalizadas serão perdidas se você reinstalar o site sobre sua instalação atual.  