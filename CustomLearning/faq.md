---
title: Microsoft 365 perguntas frequentes sobre caminhos de aprendizagem
author: karuanag
ms.author: karuanag
manager: alexb
ms.date: 02/10/2019
description: Informações de perguntas frequentes para Microsoft 365 de aprendizado
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: 82a7e777490e13fde6fef5add40beee417050027
ms.sourcegitcommit: d05381fc4a58cf2949773d73877bacc5ef3a7ca6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2021
ms.locfileid: "60048718"
---
# <a name="frequently-asked-questions"></a>Perguntas frequentes

## <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>Quais são os requisitos para instalar Microsoft 365 de aprendizado no meu ambiente de locatário?

- Os sites do SharePoint Online e Sites de Comunicação precisam estar habilitados.
- O indivíduo que estará provisionando Microsoft 365 de aprendizado deve ser o administrador de locatário do locatário de destino para instalação.
- Um locatário 'Catálogo de Aplicativos' deve estar disponível na opção 'Aplicativos' do Centro SharePoint Administrador.
- Se um novo Catálogo de Aplicativos for criado, será necessário um tempo de espera de 30 minutos ou mais para que o Catálogo de Aplicativos seja totalmente provisionado. A tentativa de provisionar Microsoft 365 de aprendizado diretamente após a criação do Catálogo de Aplicativos do locatário resultará em um erro de provisionamento da solução de caminhos de aprendizado.
- O indivíduo que estará provisionando Microsoft 365 de aprendizado deve ser um administrador do conjunto de sites do catálogo de aplicativos no locatário de destino para instalação.

## <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>Por que a Microsoft está solicitando permissões de locatário ao instalar Microsoft 365 de aprendizado?

O serviço SharePoint Provisionamento Online usa as permissões para provisionar o site SharePoint do Learning, criar as páginas do site e instalar o aplicativo de caminhos de aprendizagem Microsoft 365 no locatário. Esse é o único motivo pelo qual solicitamos as permissões. Sem as permissões solicitadas, o SharePoint provisionamento não pode executar os comandos que instalam automaticamente o modelo de site e a Web Part de caminhos de aprendizado.
![Captura de tela da solicitação de permissões](media/faqs-permissions-request-screenshot.png "Solicitação de permissões") Se você ainda tiver preocupações com esse nível de acesso, poderá conceder as permissões e implantar os modelos de site em que estiver interessado e remover imediatamente as permissões concedidas para o aplicativo no armazenamento de aplicativos [do Azure.](https://myapps.microsoft.com)

## <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>Quanto tempo levará para instalar o site em nosso ambiente de locatário?

Deve levar menos de 15 minutos. Isso não inclui o tempo necessário para personalizar o site para suas necessidades.

## <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Os Microsoft 365 de aprendizado são uma solução de código aberto e quais são as implicações?

Microsoft 365 de aprendizado é uma solução de software de código aberto (OSS) e, como tal, carrega um conjunto de benefícios e considerações para o OSS:

### <a name="benefits"></a>Benefícios 

- **Microsoft 365 de aprendizado é uma solução gratuita:** Os clientes podem instalar a solução em seu locatário, personalizá-la e torná-la disponível para os usuários finais.
- **O OSS habilita o desenvolvimento rápido e a colaboração:** Todas as soluções de código aberto estão disponíveis para uma ampla comunidade de colaboradores. A Microsoft está comprometida com esse método de impulsionar a inovação. Para garantir que estamos entregando uma experiência que beneficia o conjunto mais amplo de nossos clientes, nossa equipe principal de gerenciamento de serviços reserva o direito de determinar quais contribuições são mescladas em nossa com build oficial.  
- **O OSS habilita a colaboração com parceiros:** A Microsoft está trabalhando com vários parceiros de aprendizagem para dar suporte aos seus esforços para extensões futuras e contribuições para Microsoft 365 de aprendizado. Forneceremos mais informações à medida que esses planos são finalizados.

### <a name="implications"></a>Implicações

- **OSS não é um produto comercialmente disponível:** Os produtos comerciais incluem atualização e correção e estão incluídos em contratos de suporte baseados em taxas. Embora a Microsoft ofereça atualmente documentação, atualização e correção para Microsoft 365 de aprendizado, ela se baseia no nosso compromisso de melhorar esse cenário de negócios específico. Embora nossos planos sejam continuar investindo em caminhos de aprendizado, esteja ciente de que nossa equipe de gerenciamento de serviços pode alterar estratégias no futuro. Quaisquer alterações futuras Microsoft 365 de aprendizado serão comunicadas antes de entrar em vigor.
- **Como OSS,** Microsoft 365 de aprendizado é suportado por meio de uma lista de problemas online no GitHub : Microsoft 365 de aprendizado não é coberto por qualquer contrato de suporte da Microsoft existente. Os problemas enviados são triaged por Microsoft 365 proprietários de serviços de caminhos de aprendizagem e a comunidade. Os níveis de serviço de resolução de problemas NÃO estão no mesmo nível de um contrato de suporte pago da Microsoft.  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-sub-site-of-our-primary-sharepoint-site-collection"></a>Podemos tornar os caminhos Microsoft 365 de aprendizado um sub-site do nosso conjunto SharePoint site principal?

Não. O site é baseado em um modelo de site de comunicação, que sempre deve ser um conjunto de sites raiz.

> [!NOTE]
> É importante considerar as permissões que seus usuários finais precisarão para acessar o site. A maioria das organizações definiu grupos de usuários ou segurança. Você deve adicionar os grupos de segurança apropriados ao seu novo portal de treinamento quando estiver pronto para iniciar na sua comunidade de funcionários.

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>Preciso reinstalar o site; O que devo fazer?

Siga as instruções de instalação [publicadas aqui](custom_provision.md).

> [!NOTE]
> Se você desabilitou a telemetria em sua instalação anterior e gostaria de continuar com a telemetria desabilitada, você precisará seguir as instruções para desabilitar a telemetria [aqui](https://github.com/pnp/custom-learning-office-365/blob/a7168c97a76e0b4122e3ddfc530f6a10c724c3e1/installation/README.md).

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>Fizemos atualizações para nossa implementação de Microsoft 365 de aprendizado. Vamos perder essas atualizações (feitas em modelo de site, playlists) se reinstalarmos o site?

As personalizações para páginas individuais e listas de reprodução personalizadas serão perdidas se você reinstalar o site em sua instalação atual.  
