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
# <a name="frequently-asked-questions"></a><span data-ttu-id="a2eb0-103">Perguntas Frequentes</span><span class="sxs-lookup"><span data-stu-id="a2eb0-103">Frequently Asked Questions</span></span>

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a><span data-ttu-id="a2eb0-104">1. quais são os requisitos para instalar o aprendizado personalizado para o Office 365 em meu ambiente de locatário?</span><span class="sxs-lookup"><span data-stu-id="a2eb0-104">1. What are the requirements for installing Custom Learning for Office 365 into my tenant environment?</span></span>

- <span data-ttu-id="a2eb0-105">SharePoint Online e sites de comunicação habilitados.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-105">SharePoint Online and Communication Sites enabled.</span></span>
- <span data-ttu-id="a2eb0-106">O indivíduo que será o provisionamento de CLO365 deve ser o administrador de locatários do locatário de destino para a instalação.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-106">The individual that will be provisioning CLO365 must be the tenant administrator of the target tenant for install.</span></span>
- <span data-ttu-id="a2eb0-107">Um "catálogo de aplicativos" do locatário deve estar disponível na opção "aplicativos" do centro de administração do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-107">A tenant 'App Catalog' must be available within the 'Apps' option of the SharePoint Admin Center.</span></span>
- <span data-ttu-id="a2eb0-108">O indivíduo que será o provisionamento de CLO365 deve ser um administrador de conjunto de sites do catálogo de aplicativos no locatário de destino para a instalação.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-108">The individual that will be provisioning CLO365 must be a site collection administrator of the app catalog in the target tenant for install.</span></span>

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a><span data-ttu-id="a2eb0-109">2. quais idiomas são aprendizagem personalizada para o Office 365 disponível no?</span><span class="sxs-lookup"><span data-stu-id="a2eb0-109">2. What languages is Custom Learning for Office 365 available in?</span></span>

<span data-ttu-id="a2eb0-110">O aprendizado personalizado para o Office 365 só está disponível no momento em inglês.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-110">Custom Learning for Office 365 is currently available only in English.</span></span> <span data-ttu-id="a2eb0-111">O provisionamento automático de ponta a ponta funciona apenas com locatários em inglês.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-111">Automatic end-to-end provisioning only works with English tenants.</span></span> <span data-ttu-id="a2eb0-112">Idiomas adicionais podem ser adicionados em versões futuras.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-112">Additional languages may be added at in future releases.</span></span>

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a><span data-ttu-id="a2eb0-113">3. quanto tempo levará para instalar o site em nosso ambiente de locatário?</span><span class="sxs-lookup"><span data-stu-id="a2eb0-113">3. How long will it take to install the site in our tenant environment?</span></span>

<span data-ttu-id="a2eb0-114">Com base em nosso teste da instalação, deve levar menos de 15 minutos.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-114">Based on our testing of the installation, it should take less than 15 minutes.</span></span> <span data-ttu-id="a2eb0-115">Isso não inclui o tempo necessário para personalizar o site para seus requisitos.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-115">This does not include time required to customize the site to your requirements.</span></span>

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a><span data-ttu-id="a2eb0-116">4. podemos fazer o aprendizado personalizado para o Office 365 um subsite de nosso conjunto de sites principal do SharePoint?</span><span class="sxs-lookup"><span data-stu-id="a2eb0-116">4. Can we make the Custom learning for Office 365 a subsite of our primary SharePoint site collection?</span></span>

<span data-ttu-id="a2eb0-117">Não.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-117">No.</span></span> <span data-ttu-id="a2eb0-118">O site é baseado em um modelo de site de comunicação, que sempre é destinado a ser um conjunto de sites raiz.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-118">The site is based on a communication site template, which is always meant to be a root site collection.</span></span>

> [!NOTE]
> <span data-ttu-id="a2eb0-119">É importante considerar as permissões que os usuários finais precisarão acessar o site.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-119">It is important to consider the permissions your end users will need to access the site.</span></span> <span data-ttu-id="a2eb0-120">A maioria das organizações definiu grupos de segurança ou de usuários.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-120">Most organizations have defined security or user groups.</span></span> <span data-ttu-id="a2eb0-121">Você deve adicionar os grupos de segurança apropriados ao seu novo portal de treinamento quando estiver pronto para iniciá-lo na sua comunidade de funcionários.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-121">You must add the appropriate security groups to your new training portal once you are ready to launch it to your employee community.</span></span>

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a><span data-ttu-id="a2eb0-122">5. preciso reinstalar o site; o que devo fazer?</span><span class="sxs-lookup"><span data-stu-id="a2eb0-122">5. I need to reinstall the site; what should I do?</span></span>

<span data-ttu-id="a2eb0-123">Siga as instruções de instalação publicadas [aqui](custom_provision.md).</span><span class="sxs-lookup"><span data-stu-id="a2eb0-123">Follow the installation instructions published [here](custom_provision.md).</span></span>

> [!NOTE]
> <span data-ttu-id="a2eb0-124">Se você desabilitou a telemetria em sua instalação anterior e deseja continuar com a telemetria desabilitada, será necessário seguir as instruções para desabilitar a telemetria aqui.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-124">If you had disabled telemetry in your prior installation and would like to continue with telemetry disabled, you will need to follow the instructions for disabling the telemetry here.</span></span>

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a><span data-ttu-id="a2eb0-125">6. fizemos atualizações para nossa implementação de aprendizado personalizado para o Office 365.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-125">6. We made updates to our implementation of Custom Learning for Office 365.</span></span> <span data-ttu-id="a2eb0-126">Perderá essas atualizações (feitas no modelo de site, nas listas de reprodução) se reinstalarmos o site?</span><span class="sxs-lookup"><span data-stu-id="a2eb0-126">Will we lose these updates (made to site template, playlists) if we reinstall the site?</span></span>

<span data-ttu-id="a2eb0-127">As personalizações para páginas individuais e listas de reprodução personalizadas serão perdidas se você reinstalar o site sobre sua instalação atual.</span><span class="sxs-lookup"><span data-stu-id="a2eb0-127">Customizations to individual pages and custom playlists will be lost if you reinstall the site over your current installation.</span></span>  