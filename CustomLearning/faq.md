---
title: Microsoft 365 perguntas frequentes sobre caminhos de aprendizagem
author: karuanag
ms.author: karuanag
manager: alexb
ms.date: 02/10/2019
description: Informações de perguntas frequentes para Microsoft 365 de aprendizado
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: f24f16455ba41724d300d038a01dc04c2170dc4a
ms.sourcegitcommit: 33acfc2149de89e8375b064b2223cae505d2a102
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52575916"
---
# <a name="frequently-asked-questions"></a>Perguntas frequentes

### <a name="i-recently-saw-a-blog-post-that-custom-learning-for-office-365-is-being-renamed-to-microsoft-365-learning-pathways-are-there-other-changes-being-added-to-the-solution-as-part-of-the-renaming-effort-should-i-update-the-solution-in-my-organization"></a>Recentemente, vi uma postagem de blog em que o Custom Learning for Office 365 está sendo renomeado para Microsoft 365 de aprendizado. Há outras alterações sendo adicionadas à solução como parte do esforço de renomeação? Devo atualizar a solução na minha organização?

A Microsoft 365 de aprendizado é um esforço de renomeação dedicado a alterar o nome da solução para se alinhar Microsoft 365 identidade visual. Se você tiver o Custom Learning para Office 365 executando com êxito em sua organização, não é necessário atualizar a solução no momento.  

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>Quais são os requisitos para instalar Microsoft 365 de aprendizado no meu ambiente de locatário?

- Os sites do SharePoint Online e Sites de Comunicação precisam estar habilitados.
- O indivíduo que estará provisionando o CLO365 deve ser o administrador de locatário do locatário de destino para instalação.
- Um locatário 'Catálogo de Aplicativos' deve estar disponível na opção 'Aplicativos' do Centro SharePoint Administrador.
- Se um novo Catálogo de Aplicativos for criado, será necessário um tempo de espera de 30 minutos ou mais para que o Catálogo de Aplicativos seja totalmente provisionado. A tentativa de provisionar Microsoft 365 de aprendizado diretamente após a criação do Catálogo de Aplicativos do locatário resultará em um erro de provisionamento da solução de caminhos de aprendizado. 
- O indivíduo que estará provisionando o CLO365 deve ser um administrador do conjunto de sites do catálogo de aplicativos no locatário de destino para instalação.

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>Por que a Microsoft está solicitando permissões de locatário ao instalar Microsoft 365 de aprendizado 

- O SharePoint de Provisionamento Online usa as permissões para provisionar o site SharePoint learning Pathways, criar as páginas do site e instalar o aplicativo de caminhos de Microsoft 365 de aprendizagem em seu locatário. Esse é o único motivo pelo qual solicitamos as permissões. Sem as permissões solicitadas, o SharePoint provisionamento não pode executar os comandos que instalam automaticamente o modelo de site e a Web Part de caminhos de aprendizado. 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>Quais são as implicações de Microsoft 365 de aprendizado em uma Visualização Beta? 

Microsoft 365 de aprendizado está atualmente em Beta Preview. Considere o seguinte conforme você avalia, planeja e implementa Microsoft 365 de aprendizado:

- Assim como em qualquer solução Beta, nossa equipe de gerenciamento de serviços reserva o direito de fazer alterações no serviço e em seus componentes. Como você está resolvendo ativamente bugs e problemas de UX, provavelmente precisará atualizar o WebPart.
- Para atualizar a Web Part, você precisará baixá-la de nosso repositório GitHub e carregue-a no catálogo de aplicativos de locatário. Consulte a seção "Atualizando a solução" do arquivo [readme](https://github.com/pnp/custom-learning-office-365/blob/master/README.md) Microsoft 365 de aprendizado. 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>Em quais idiomas Microsoft 365 caminhos de aprendizado disponíveis?

Microsoft 365 de aprendizado está disponível apenas em inglês. O provisionamento automático de ponta a ponta só funciona com locatários em inglês. Planejamos a implantação de suporte multilíngue para os idiomas a seguir no segundo trimestre de 2020. 

- Chinês (simplificado) 
- Francês  
- Alemão 
- Italiano (Itália) 
- Japonês (Japão)  
- Português (Brasil) 
- Russo (russo)  
- Espanhol 

> O suporte para o idioma holandês não será incluído na próxima versão do suporte a vários idiomas para caminhos de aprendizado. Continuaremos avaliando novas opções de idioma no futuro.

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>Quanto tempo levará para instalar o site em nosso ambiente de locatário?

Com base no nosso teste da instalação, deve levar menos de 15 minutos. Isso não inclui o tempo necessário para personalizar o site para suas necessidades.

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Os Microsoft 365 de aprendizado são uma solução de código aberto e quais são as implicações?

Microsoft 365 de aprendizado é uma solução de software de código aberto (OSS) e, como tal, carrega um conjunto de benefícios e considerações para o OSS:

#### <a name="benefits"></a>Benefícios 
- **Microsoft 365 de aprendizado é uma solução gratuita:** Os clientes podem instalar a solução em seu locatário, personalizá-la e torná-la disponível para os usuários finais
- **O OSS habilita o desenvolvimento rápido e a colaboração:**  Todas as soluções de código aberto estão disponíveis para uma ampla comunidade de colaboradores.  A Microsoft está comprometida com esse método de impulsionar a inovação.  Para garantir que estamos entregando uma experiência que beneficia o conjunto mais amplo de nossos clientes, nossa equipe principal de gerenciamento de serviços reserva o direito de determinar quais contribuições são mescladas em nossa com build oficial.  
- **O OSS habilita a colaboração com parceiros:** A Microsoft está trabalhando com vários parceiros de aprendizagem para dar suporte aos seus esforços para extensões futuras e contribuições para Microsoft 365 de aprendizado. Forneceremos mais informações à medida que esses planos são finalizados. 
    
#### <a name="implications"></a>Implicações
- **OSS não é um produto comercialmente disponível:** Os produtos comerciais incluem atualização e correção e estão incluídos em contratos de suporte baseados em taxas. Embora a Microsoft ofereça atualmente documentação, atualização e correção para Microsoft 365 de aprendizado, ela se baseia no nosso compromisso de melhorar esse cenário de negócios específico. Nossos planos são continuar investindo em caminhos de aprendizado, esteja ciente de que nossa equipe de gerenciamento de serviços pode mudar estratégias no futuro. Quaisquer alterações futuras Microsoft 365 de aprendizado serão comunicadas antes de entrar em vigor. 
- **Como OSS,** Microsoft 365 de aprendizado é suportado por meio de uma lista de problemas online no GitHub : Microsoft 365 de aprendizado não é coberto por qualquer contrato de suporte da Microsoft existente. Os problemas enviados são triaged por Microsoft 365 proprietários de serviços de caminhos de aprendizagem e a comunidade. Os níveis de serviço de resolução de problemas NÃO estão no mesmo nível de um contrato de suporte pago da Microsoft.  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>Podemos tornar os caminhos Microsoft 365 de aprendizado um subsite do nosso conjunto SharePoint site principal?

Não. O site é baseado em um modelo de site de comunicação, que sempre deve ser um conjunto de sites raiz.

> [!NOTE]
> É importante considerar as permissões que seus usuários finais precisarão para acessar o site. A maioria das organizações definiu grupos de usuários ou segurança. Você deve adicionar os grupos de segurança apropriados ao seu novo portal de treinamento quando estiver pronto para iniciar na sua comunidade de funcionários.

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>Preciso reinstalar o site; O que devo fazer?

Siga as instruções de instalação [publicadas aqui](custom_provision.md).

> [!NOTE]
> Se você desabilitou a telemetria em sua instalação anterior e gostaria de continuar com a telemetria desabilitada, você precisará seguir as instruções para desabilitar a telemetria aqui.

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>Fizemos atualizações para nossa implementação de Microsoft 365 de aprendizado. Vamos perder essas atualizações (feitas em modelo de site, playlists) se reinstalarmos o site?

As personalizações para páginas individuais e listas de reprodução personalizadas serão perdidas se você reinstalar o site em sua instalação atual.  
