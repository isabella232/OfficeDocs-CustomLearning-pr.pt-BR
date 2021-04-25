---
title: Perguntas frequentes sobre caminhos de aprendizagem do Microsoft 365
author: karuanag
ms.author: karuanag
ms.date: 02/10/2019
description: Informações de perguntas frequentes sobre os caminhos de aprendizado do Microsoft 365
ms.service: sharepoint-online
ms.openlocfilehash: d91c2710315b393eb8be3645c4fa94b32d353aa7
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000077"
---
# <a name="frequently-asked-questions"></a>Perguntas frequentes

### <a name="i-recently-saw-a-blog-post-that-custom-learning-for-office-365-is-being-renamed-to-microsoft-365-learning-pathways-are-there-other-changes-being-added-to-the-solution-as-part-of-the-renaming-effort-should-i-update-the-solution-in-my-organization"></a>Recentemente, vi uma postagem de blog em que o Custom Learning para o Office 365 está sendo renomeado para caminhos de aprendizado do Microsoft 365. Há outras alterações sendo adicionadas à solução como parte do esforço de renomeação? Devo atualizar a solução na minha organização?

A versão de caminhos de aprendizado do Microsoft 365 é um esforço de rebranding dedicado a alterar o nome da solução para se alinhar à identidade visual do Microsoft 365. Se você tiver o Custom Learning para o Office 365 executando com êxito em sua organização, não é necessário atualizar a solução no momento.  

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>Quais são os requisitos para instalar os caminhos de aprendizado do Microsoft 365 no meu ambiente de locatário?

- Os sites do SharePoint Online e Sites de Comunicação precisam estar habilitados.
- O indivíduo que estará provisionando o CLO365 deve ser o administrador de locatário do locatário de destino para instalação.
- Um locatário 'Catálogo de Aplicativos' deve estar disponível na opção 'Aplicativos' do Centro de Administração do SharePoint.
- Se um novo Catálogo de Aplicativos for criado, será necessário um tempo de espera de 30 minutos ou mais para que o Catálogo de Aplicativos seja totalmente provisionado. A tentativa de provisionar os caminhos de aprendizado do Microsoft 365 diretamente após a criação do Catálogo de Aplicativos do locatário resultará em um erro de provisionamento da solução de caminhos de aprendizado. 
- O indivíduo que estará provisionando o CLO365 deve ser um administrador do conjunto de sites do catálogo de aplicativos no locatário de destino para instalação.

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>Por que a Microsoft está solicitando permissões de locatário ao instalar os caminhos de aprendizado do Microsoft 365 

- O serviço de Provisionamento do SharePoint Online usa as permissões para provisionar o site do SharePoint Caminhos de Aprendizagem, criar as páginas do site e instalar o aplicativo de caminhos de aprendizado do Microsoft 365 em seu locatário. Esse é o único motivo pelo qual solicitamos as permissões. Sem as permissões solicitadas, o Serviço de Provisionamento do SharePoint não pode executar os comandos que instalam automaticamente o modelo de site e a Web Part de caminhos de aprendizado. 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>Quais são as implicações dos caminhos de aprendizado do Microsoft 365 em uma Visualização Beta? 

Os caminhos de aprendizado do Microsoft 365 estão atualmente no Beta Preview. Considere o seguinte conforme você avalia, planeja e implementa os caminhos de aprendizado do Microsoft 365:

- Assim como em qualquer solução Beta, nossa equipe de gerenciamento de serviços reserva o direito de fazer alterações no serviço e em seus componentes. Como você está resolvendo ativamente bugs e problemas de UX, provavelmente precisará atualizar o WebPart.
- Para atualizar a Web Part, você precisará baixá-la do repositório do GitHub e carregar no catálogo de aplicativos do locatário. Consulte a seção "Atualizando a solução" do arquivo [Readme](https://github.com/pnp/custom-learning-office-365/blob/master/README.md) dos caminhos de aprendizado do Microsoft 365. 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>Em quais idiomas estão disponíveis os caminhos de aprendizado do Microsoft 365?

Os caminhos de aprendizado do Microsoft 365 estão disponíveis apenas em inglês. O provisionamento automático de ponta a ponta só funciona com locatários em inglês. Planejamos a implantação de suporte multilíngue para os idiomas a seguir no segundo trimestre de 2020. 

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

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Os caminhos de aprendizado do Microsoft 365 são uma solução de código aberto e quais são as implicações?

Os caminhos de aprendizado do Microsoft 365 são uma solução de software de código aberto (OSS) e, como tal, carregam um conjunto de benefícios e considerações para o OSS:

#### <a name="benefits"></a>Benefícios 
- Os caminhos de aprendizado do **Microsoft 365 são uma solução gratuita:** Os clientes podem instalar a solução em seu locatário, personalizá-la e torná-la disponível para os usuários finais
- **O OSS habilita o desenvolvimento rápido e a colaboração:**  Todas as soluções de código aberto estão disponíveis para uma ampla comunidade de colaboradores.  A Microsoft está comprometida com esse método de impulsionar a inovação.  Para garantir que estamos entregando uma experiência que beneficia o conjunto mais amplo de nossos clientes, nossa equipe principal de gerenciamento de serviços reserva o direito de determinar quais contribuições são mescladas em nossa com build oficial.  
- **O OSS habilita a colaboração com parceiros:** A Microsoft está trabalhando com vários parceiros de aprendizagem para dar suporte aos seus esforços para extensões futuras e contribuições para os caminhos de aprendizado do Microsoft 365. Forneceremos mais informações à medida que esses planos são finalizados. 
    
#### <a name="implications"></a>Implicações
- **OSS não é um produto comercialmente disponível:** Os produtos comerciais incluem atualização e correção e estão incluídos em contratos de suporte baseados em taxas. Embora a Microsoft ofereça atualmente documentação, atualização e correção para os caminhos de aprendizado do Microsoft 365, ela se baseia no nosso compromisso de melhorar esse cenário de negócios específico. Nossos planos são continuar investindo em caminhos de aprendizado, esteja ciente de que nossa equipe de gerenciamento de serviços pode mudar estratégias no futuro. Quaisquer alterações futuras nos caminhos de aprendizado do Microsoft 365 serão comunicadas antes de entrar em vigor. 
- Como OSS, os caminhos de aprendizado do **Microsoft 365** são suportados por meio de uma lista de problemas online no GitHub : os caminhos de aprendizado do Microsoft 365 não são cobertos por qualquer contrato de suporte da Microsoft existente. Os problemas enviados são triaged pelos proprietários do serviço de caminhos de aprendizado do Microsoft 365 e pela comunidade. Os níveis de serviço de resolução de problemas NÃO estão no mesmo nível de um contrato de suporte pago da Microsoft.  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>Podemos tornar os caminhos de aprendizado do Microsoft 365 um subsite do nosso conjunto de sites principal do SharePoint?

Não. O site é baseado em um modelo de site de comunicação, que sempre deve ser um conjunto de sites raiz.

> [!NOTE]
> É importante considerar as permissões que seus usuários finais precisarão para acessar o site. A maioria das organizações definiu grupos de usuários ou segurança. Você deve adicionar os grupos de segurança apropriados ao seu novo portal de treinamento quando estiver pronto para iniciar na sua comunidade de funcionários.

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>Preciso reinstalar o site; O que devo fazer?

Siga as instruções de instalação [publicadas aqui](custom_provision.md).

> [!NOTE]
> Se você desabilitou a telemetria em sua instalação anterior e gostaria de continuar com a telemetria desabilitada, você precisará seguir as instruções para desabilitar a telemetria aqui.

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>Fizemos atualizações para a implementação dos caminhos de aprendizado do Microsoft 365. Vamos perder essas atualizações (feitas em modelo de site, playlists) se reinstalarmos o site?

As personalizações para páginas individuais e listas de reprodução personalizadas serão perdidas se você reinstalar o site em sua instalação atual.  
