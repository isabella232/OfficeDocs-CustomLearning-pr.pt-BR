---
author: karuanag
ms.author: karuanag
title: Perguntas frequentes sobre os caminhos de aprendizado do Microsoft 365
ms.date: 02/10/2019
description: Informações de perguntas frequentes para os caminhos de aprendizado do Microsoft 365
ms.openlocfilehash: 5b90971ef6e411b4bd8d0cece2d8211f6fd5db23
ms.sourcegitcommit: 86cfa176d50b324c964b1a8609270cc73a2468b3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068812"
---
# <a name="frequently-asked-questions"></a>Perguntas Frequentes

### <a name="i-recently-saw-a-blog-post-that-custom-learning-for-office-365-is-being-renamed-to-microsoft-365-learning-pathways-are-there-other-changes-being-added-to-the-solution-as-part-of-the-renaming-effort-should-i-update-the-solution-in-my-organization"></a>Recentemente, vi uma postagem de blog que o aprendizado personalizado para o Office 365 está sendo renomeado para os caminhos de aprendizado da Microsoft 365. Há outras alterações que estão sendo adicionadas à solução como parte do esforço de renomeação? Devo atualizar a solução em minha organização?

O lançamento dos cursores de aprendizado da Microsoft 365 é um esforço de remarcação dedicado à alteração do nome da solução para alinhar-se com a identidade visual 365 da Microsoft. Se você tiver o aprendizado personalizado do Office 365 atualmente em execução com êxito em sua organização, não será necessário atualizar a solução no momento.  

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>Quais são os requisitos para instalar os caminhos de aprendizado do Microsoft 365 em meu ambiente de locatários?

- SharePoint Online e sites de comunicação habilitados.
- O indivíduo que será o provisionamento de CLO365 deve ser o administrador de locatários do locatário de destino para a instalação.
- Um "catálogo de aplicativos" do locatário deve estar disponível na opção "aplicativos" do centro de administração do SharePoint.
- Se um novo catálogo de aplicativos for criado, um tempo de espera de 30 minutos ou mais é necessário para que o catálogo de aplicativos seja totalmente provisionado. Tentar provisionar os caminhos de aprendizado do Microsoft 365 diretamente após a criação do catálogo de aplicativos do locatário resultará em um erro de provisionamento da solução de cursores de aprendizado. 
- O indivíduo que será o provisionamento de CLO365 deve ser um administrador de conjunto de sites do catálogo de aplicativos no locatário de destino para a instalação.

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>Por que a Microsoft está solicitando permissões de locatário ao instalar os caminhos de aprendizado do Microsoft 365 

- O serviço de provisionamento do SharePoint Online usa as permissões para provisionar o site de cursores de aprendizado do SharePoint, criar as páginas do site e instalar o aplicativo de caminhos de aprendizado do Microsoft 365 em seus locatários. Essa é a única razão pela qual nos solicitamos as permissões. Sem as permissões solicitadas, o serviço de provisionamento do SharePoint não pode executar os comandos que instalam automaticamente o modelo de site de cursores de aprendizado e a Web Part. 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>Quais são as implicações dos caminhos de aprendizado da Microsoft 365 em uma versão beta prévia? 

Os caminhos de aprendizado do Microsoft 365 estão atualmente na visualização beta. Considere o seguinte ao avaliar, planejar e implementar os caminhos de aprendizado da Microsoft 365:

- Como em qualquer solução beta, nossa equipe de gerenciamento de serviços reserva-se o direito de fazer alterações no serviço e seus componentes. À medida que estamos resolvendo erros e problemas de experiência do UX, provavelmente você precisaria atualizar a Web Part.
- Para atualizar a Web Part, você precisará baixá-la em nosso repositório do GitHub e carregá-la no catálogo de aplicativos do locatário. Consulte a seção "Atualizando a solução" do arquivo [Leiame](https://github.com/pnp/custom-learning-office-365/blob/master/README.md) dos caminhos de aprendizado do Microsoft 365. 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>Quais idiomas são os caminhos de aprendizado da Microsoft 365 disponíveis no?

Os caminhos de aprendizado do Microsoft 365 estão atualmente disponíveis somente em inglês. O provisionamento automático de ponta a ponta funciona apenas com locatários em inglês. Planejamos implantar o suporte multilíngue para esses nove idiomas no primeiro trimestre de 2020. 

- Chinês (simplificado) 
- Holandês (Países Baixos) 
- Francês  
- Alemão 
- Italiano (Itália) 
- Japonês (Japão)  
- Português (Brasil) 
- Russo (russo)  
- Espanhol 

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>Quanto tempo levará para instalar o site em nosso ambiente de locatário?

Com base em nosso teste da instalação, deve levar menos de 15 minutos. Isso não inclui o tempo necessário para personalizar o site para seus requisitos.

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>O Microsoft 365 Learning é o caminho de uma solução de Open Source e quais são as implicações?

Os caminhos de aprendizado da Microsoft 365 são uma solução de software de código aberto (OSS) e, como tal, realiza um conjunto de benefícios e considerações em alemão para o OSS:

#### <a name="benefits"></a>Benefícios 
- Os **caminhos de aprendizado da Microsoft 365 são uma solução gratuita:** Os clientes podem instalar a solução em seus locatários, personalizá-la e torná-la disponível para os usuários finais
- O **OSS permite desenvolvimento e colaboração rápidos:**  Todas as soluções de código aberto estão disponíveis para uma ampla comunidade de colaboradores.  A Microsoft está comprometida com esse método de condução de inovação.  Para garantir que estamos fornecendo uma experiência que beneficia o conjunto mais amplo de nossos clientes, nossa equipe de gerenciamento de serviços principais irá reservar o direito de determinar quais contribuições serão mescladas em nossa compilação oficial.  
- O **OSS permite a colaboração com parceiros:** A Microsoft está trabalhando com vários parceiros de aprendizado para dar suporte aos esforços para futuras extensões e contribuições para os caminhos de aprendizado da Microsoft 365. Forneceremos mais informações, pois esses planos serão finalizados. 
    
#### <a name="implications"></a>Implica
- **O OSS não é um produto disponível comercialmente:** Os produtos comerciais incluem atualização e patch e incluídos em contratos de suporte baseados em taxas. Embora a Microsoft oferece atualmente documentação, atualização e correção para os cursores de aprendizagem do Microsoft 365, ela se baseia em nosso compromisso de melhorar esse cenário comercial específico. Nossos planos são continuar investindo em caminhos de aprendizado, mas os clientes devem estar cientes de que nossa equipe de gerenciamento de serviços pode mudar de estratégia no futuro. As alterações futuras feitas nos caminhos de aprendizado do Microsoft 365 serão comunicadas com antecedência. 
- **Como SOS, os caminhos de aprendizado da microsoft 365 são suportados por meio de uma lista de problemas online no GitHub**: os caminhos de aprendizado da Microsoft 365 não estão cobertos por nenhum contrato de suporte da Microsoft existente. Problemas enviados são classificados por proprietários de serviço de cursores de aprendizado da Microsoft 365 e da Comunidade. Os níveis de serviço de resolução de problemas não estão no mesmo nível que um contrato de suporte da Microsoft pago.  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>Podemos fazer com que o Microsoft 365 Learning decursos seja um subsite de nosso conjunto de sites principal do SharePoint?

Não. O site é baseado em um modelo de site de comunicação, que sempre é destinado a ser um conjunto de sites raiz.

> [!NOTE]
> É importante considerar as permissões que os usuários finais precisarão acessar o site. A maioria das organizações definiu grupos de segurança ou de usuários. Você deve adicionar os grupos de segurança apropriados ao seu novo portal de treinamento quando estiver pronto para iniciá-lo na sua comunidade de funcionários.

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>Preciso reinstalar o site; o que devo fazer?

Siga as instruções de instalação publicadas [aqui](custom_provision.md).

> [!NOTE]
> Se você desabilitou a telemetria em sua instalação anterior e deseja continuar com a telemetria desabilitada, será necessário seguir as instruções para desabilitar a telemetria aqui.

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>Fizemos atualizações em nossa implementação de caminhos de aprendizado do Microsoft 365. Perderá essas atualizações (feitas no modelo de site, nas listas de reprodução) se reinstalarmos o site?

As personalizações para páginas individuais e listas de reprodução personalizadas serão perdidas se você reinstalar o site sobre sua instalação atual.  