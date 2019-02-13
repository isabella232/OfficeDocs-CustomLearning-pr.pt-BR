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
# <a name="frequently-asked-questions"></a><span data-ttu-id="0340c-103">Perguntas Frequentes</span><span class="sxs-lookup"><span data-stu-id="0340c-103">Frequently Asked Questions</span></span>

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a><span data-ttu-id="0340c-104">1. quais são os requisitos para instalar o aprendizado personalizado para o Office 365 em meu ambiente locatário?</span><span class="sxs-lookup"><span data-stu-id="0340c-104">1. What are the requirements for installing Custom Learning for Office 365 into my tenant environment?</span></span>

- <span data-ttu-id="0340c-105">SharePoint Online e os Sites de comunicação habilitados.</span><span class="sxs-lookup"><span data-stu-id="0340c-105">SharePoint Online and Communication Sites enabled.</span></span>
- <span data-ttu-id="0340c-106">O indivíduo que vai ser provisionamento CLO365 deve ser o administrador de locatário do inquilino destino para a instalação.</span><span class="sxs-lookup"><span data-stu-id="0340c-106">The individual that will be provisioning CLO365 must be the tenant administrator of the target tenant for install.</span></span>
- <span data-ttu-id="0340c-107">Um locatário 'App Catalog' deve estar disponível na opção 'Apps' do Centro de administração do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0340c-107">A tenant 'App Catalog' must be available within the 'Apps' option of the SharePoint Admin Center.</span></span>
- <span data-ttu-id="0340c-108">O indivíduo que vai ser provisionamento CLO365 deve ser um administrador de conjunto de sites do catálogo de aplicativos no locatário destino para a instalação.</span><span class="sxs-lookup"><span data-stu-id="0340c-108">The individual that will be provisioning CLO365 must be a site collection administrator of the app catalog in the target tenant for install.</span></span>

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a><span data-ttu-id="0340c-109">2. quais idiomas está disponível na aprendizagem personalizado para o Office 365?</span><span class="sxs-lookup"><span data-stu-id="0340c-109">2. What languages is Custom Learning for Office 365 available in?</span></span>

<span data-ttu-id="0340c-p101">Sinalizador de aprendizagem do Office 365 está atualmente disponível apenas em inglês. O provisionamento automático de ponta a ponta funciona somente com locatários em inglês. Idiomas adicionais podem ser adicionados em futuras versões.</span><span class="sxs-lookup"><span data-stu-id="0340c-p101">Custom Learning for Office 365 is currently available only in English. Automatic end-to-end provisioning only works with English tenants. Additional languages may be added at in future releases.</span></span>

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a><span data-ttu-id="0340c-113">3. quanto tempo levará para instalar o site em nosso ambiente de locatário?</span><span class="sxs-lookup"><span data-stu-id="0340c-113">3. How long will it take to install the site in our tenant environment?</span></span>

<span data-ttu-id="0340c-p102">Com base em nossos testes da instalação, ele deve levar menos de 15 minutos. Isso não incluir o tempo necessário para personalizar o site às suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="0340c-p102">Based on our testing of the installation, it should take less than 15 minutes. This does not include time required to customize the site to your requirements.</span></span>

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a><span data-ttu-id="0340c-116">4. podemos tornar o sinalizador de aprendizagem do Office 365 um subsite de nosso principal conjunto de sites do SharePoint?</span><span class="sxs-lookup"><span data-stu-id="0340c-116">4. Can we make the Custom learning for Office 365 a subsite of our primary SharePoint site collection?</span></span>

<span data-ttu-id="0340c-p103">Não. O site baseia-se em um modelo de site de comunicação, que sempre deve ser um conjunto de sites raiz.</span><span class="sxs-lookup"><span data-stu-id="0340c-p103">No. The site is based on a communication site template, which is always meant to be a root site collection.</span></span>

> [!NOTE]
> <span data-ttu-id="0340c-p104">É importante considerar as permissões que os usuários finais precisará acessar o site. A maioria das organizações definiu a grupos de segurança ou de usuário. Você deve adicionar grupos de segurança apropriados para seu novo portal de treinamento, quando você estiver pronto para iniciá-lo à sua comunidade de funcionário.</span><span class="sxs-lookup"><span data-stu-id="0340c-p104">It is important to consider the permissions your end users will need to access the site. Most organizations have defined security or user groups. You must add the appropriate security groups to your new training portal once you are ready to launch it to your employee community.</span></span>

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a><span data-ttu-id="0340c-122">5. eu preciso reinstalar o site; o que deve fazer?</span><span class="sxs-lookup"><span data-stu-id="0340c-122">5. I need to reinstall the site; what should I do?</span></span>

<span data-ttu-id="0340c-123">Execute a instalação instruções publicado [aqui](installsitepackage.md).</span><span class="sxs-lookup"><span data-stu-id="0340c-123">Follow the installation instructions published [here](installsitepackage.md).</span></span>

> [!NOTE]
> <span data-ttu-id="0340c-124">Se você tiver desabilitado a telemetria na sua instalação anterior e gostaria de continuar com a telemetria desabilitada, você precisará siga as instruções para desabilitar a telemetria aqui.</span><span class="sxs-lookup"><span data-stu-id="0340c-124">If you had disabled telemetry in your prior installation and would like to continue with telemetry disabled, you will need to follow the instructions for disabling the telemetry here.</span></span>

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a><span data-ttu-id="0340c-p105">6. que fizemos atualizações à nossa implementação de aprendizado personalizado para o Office 365. Podemos perderá essas atualizações (feitas ao modelo de sites, listas de reprodução) se podemos reinstalar o site?</span><span class="sxs-lookup"><span data-stu-id="0340c-p105">6. We made updates to our implementation of Custom Learning for Office 365. Will we lose these updates (made to site template, playlists) if we reinstall the site?</span></span>

<span data-ttu-id="0340c-127">Personalizações páginas individuais e listas de reprodução personalizadas serão perdidas se você reinstalar o site sobre sua instalação atual.</span><span class="sxs-lookup"><span data-stu-id="0340c-127">Customizations to individual pages and custom playlists will be lost if you reinstall the site over your current installation.</span></span>  