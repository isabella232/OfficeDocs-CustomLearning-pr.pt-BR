---
author: pkrebs
ms.author: pkrebs
title: Visão geral
ms.date: 02/18/2019
description: Visão geral do aprendizado personalizado para o Office 365 para administradores
ms.openlocfilehash: 6aee3a93a5109b37e43a7118bd98ca31e8b9ac1f
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055618"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="deee9-103">Personalizar a experiência de aprendizagem</span><span class="sxs-lookup"><span data-stu-id="deee9-103">Customize the Learning Experience</span></span>

<span data-ttu-id="deee9-104">Apresentando o aprendizado personalizado para o Office 365, uma nova solução da Microsoft projetada para acelerar o uso e a adoção do Office 365 dentro de uma organização.</span><span class="sxs-lookup"><span data-stu-id="deee9-104">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization.</span></span> <span data-ttu-id="deee9-105">Com o aprendizado personalizado, você pode:</span><span class="sxs-lookup"><span data-stu-id="deee9-105">With Custom Learning, you can:</span></span>
- <span data-ttu-id="deee9-106">Ajustar o conteúdo de aprendizado e adoção do Office 365 para seu ambiente</span><span class="sxs-lookup"><span data-stu-id="deee9-106">Tailor Office 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="deee9-107">Ocultar ou Mostrar conteúdo para refletir os serviços ou recursos compatíveis com a sua organização</span><span class="sxs-lookup"><span data-stu-id="deee9-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="deee9-108">Manter o conteúdo e os usuários atualizados com um feed atualizado de conteúdo de aprendizado da Microsoft</span><span class="sxs-lookup"><span data-stu-id="deee9-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="deee9-109">Criar listas de reprodução e categorias personalizadas criadas especificamente para as necessidades do usuário</span><span class="sxs-lookup"><span data-stu-id="deee9-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![CG-Introducing. png](media/cg-introducing.png)

## <a name="how-does-custom-learning-work"></a><span data-ttu-id="deee9-111">Como funciona o aprendizado personalizado?</span><span class="sxs-lookup"><span data-stu-id="deee9-111">How does Custom Learning work?</span></span>

<span data-ttu-id="deee9-112">O aprendizado personalizado para o Office 365 (aprendizado personalizado para curto) consiste em três partes:</span><span class="sxs-lookup"><span data-stu-id="deee9-112">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
1. <span data-ttu-id="deee9-113">um feed ativo de conteúdo de um catálogo do Microsoft Online</span><span class="sxs-lookup"><span data-stu-id="deee9-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="deee9-114">um site de comunicação do SharePoint</span><span class="sxs-lookup"><span data-stu-id="deee9-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="deee9-115">uma Web Part do SharePoint</span><span class="sxs-lookup"><span data-stu-id="deee9-115">a SharePoint web part</span></span> 

![CG-howitworks. png](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="deee9-117">Requisitos e permissões</span><span class="sxs-lookup"><span data-stu-id="deee9-117">Requirements and Permissions</span></span>

<span data-ttu-id="deee9-118">Antes de começar a usar este guia, verifique se a aprendizagem personalizada foi configurada pelo administrador de locatários do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="deee9-118">Before getting started with this guide, ensure that Custom Learning has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="deee9-119">Se você não tiver certeza sobre a configuração, entre em contato com o administrador de locatários do SharePoint para verificar se o aprendizado personalizado foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="deee9-119">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that Custom Learning has been provisioned.</span></span> <span data-ttu-id="deee9-120">Além disso, certifique-se de obter a URL do site do SharePoint de aprendizado personalizado.</span><span class="sxs-lookup"><span data-stu-id="deee9-120">Also be sure to get the URL of the Custom Learning SharePoint site.</span></span> <span data-ttu-id="deee9-121">Se você for o administrador de locatários e o aprendizado personalizado não foram provisionados, consulte proVisionar o [aprendizado personalizado](custom_provision.md).</span><span class="sxs-lookup"><span data-stu-id="deee9-121">If you are the Tenant Administrator and Custom Learning has not been provisioned, see [Provision Custom Learning](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-custom-learning"></a><span data-ttu-id="deee9-122">Permissões para provisionar o aprendizado personalizado</span><span class="sxs-lookup"><span data-stu-id="deee9-122">Permissions to provision Custom Learning</span></span>

- <span data-ttu-id="deee9-123">Administrador de locatários, também conhecido como administrador global do Office 365</span><span class="sxs-lookup"><span data-stu-id="deee9-123">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="deee9-124">Administrador do conjunto de sites do SharePoint com permissões de proprietário no site</span><span class="sxs-lookup"><span data-stu-id="deee9-124">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-custom-learning-administration-features"></a><span data-ttu-id="deee9-125">Permissões para usar recursos personalizados de administração de aprendizado</span><span class="sxs-lookup"><span data-stu-id="deee9-125">Permissions to use Custom Learning Administration features</span></span>

- <span data-ttu-id="deee9-126">Administrador de Conjunto de Sites</span><span class="sxs-lookup"><span data-stu-id="deee9-126">Site Collection Administrator</span></span>
- <span data-ttu-id="deee9-127">Proprietário do SharePoint ou permissões de membro</span><span class="sxs-lookup"><span data-stu-id="deee9-127">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-custom-learning-site-as-a-user"></a><span data-ttu-id="deee9-128">Permissões para usar o site de aprendizado personalizado como usuário</span><span class="sxs-lookup"><span data-stu-id="deee9-128">Permissions to use the Custom Learning site as a user</span></span>

- <span data-ttu-id="deee9-129">Office 365 permissões de usuário/permissões de visitante de site do SharePoint ou mais</span><span class="sxs-lookup"><span data-stu-id="deee9-129">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="deee9-130">Introdução à personalização</span><span class="sxs-lookup"><span data-stu-id="deee9-130">Get started with customization</span></span>
<span data-ttu-id="deee9-131">Quando tiver certeza de que tem as permissões necessárias para personalizar o site e a Web Part, é hora de começar a usar o processo de personalização.</span><span class="sxs-lookup"><span data-stu-id="deee9-131">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="deee9-132">Para começar, consulte [vá para o site de aprendizado personalizado](custom_goto.md).</span><span class="sxs-lookup"><span data-stu-id="deee9-132">To get started, see [Go to the Custom Learning Site](custom_goto.md).</span></span>