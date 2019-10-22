---
author: pkrebs
ms.author: pkrebs
title: Visão geral
ms.date: 02/18/2019
description: Visão geral dos caminhos de aprendizado do Microsoft 365
ms.openlocfilehash: 74fac090177ad8009155e21a977b05ee2b742b3b
ms.sourcegitcommit: f5a7079d56598c14aef2f4b886c025a59ba89276
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2019
ms.locfileid: "34247836"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="583c7-103">Personalizar a experiência de aprendizagem</span><span class="sxs-lookup"><span data-stu-id="583c7-103">Customize the learning experience</span></span>

<span data-ttu-id="583c7-104">Apresentando os caminhos de aprendizado da Microsoft 365, uma nova solução da Microsoft projetada para acelerar o uso e a adoção do Office 365 dentro de uma organização.</span><span class="sxs-lookup"><span data-stu-id="583c7-104">Introducing Microsoft 365 learning pathways, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization.</span></span> <span data-ttu-id="583c7-105">Com o Learning pathwyas, você pode:</span><span class="sxs-lookup"><span data-stu-id="583c7-105">With learning pathwyas, you can:</span></span>
- <span data-ttu-id="583c7-106">Ajuste o conteúdo de treinamento e adoção do Microsoft 365 para seu ambiente</span><span class="sxs-lookup"><span data-stu-id="583c7-106">Tailor Microsoft 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="583c7-107">Ocultar ou Mostrar conteúdo para refletir os serviços ou recursos compatíveis com a sua organização</span><span class="sxs-lookup"><span data-stu-id="583c7-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="583c7-108">Manter o conteúdo e os usuários atualizados com um feed atualizado de conteúdo de aprendizado da Microsoft</span><span class="sxs-lookup"><span data-stu-id="583c7-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="583c7-109">Criar listas de reprodução e categorias personalizadas criadas especificamente para as necessidades do usuário</span><span class="sxs-lookup"><span data-stu-id="583c7-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![CG-Introducing. png](media/cg-introducing.png)

## <a name="how-does-learning-pathways-work"></a><span data-ttu-id="583c7-111">Como funciona o cursores de aprendizado?</span><span class="sxs-lookup"><span data-stu-id="583c7-111">How does learning pathways work?</span></span>

<span data-ttu-id="583c7-112">os caminhos de aprendizado do Office 365 (caminhos de aprendizado para curto) consistem em três partes:</span><span class="sxs-lookup"><span data-stu-id="583c7-112">learning pathways for Office 365 (learning pathways for short) consists of three parts:</span></span> 
1. <span data-ttu-id="583c7-113">um feed ativo de conteúdo de um catálogo do Microsoft Online</span><span class="sxs-lookup"><span data-stu-id="583c7-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="583c7-114">um site de comunicação do SharePoint</span><span class="sxs-lookup"><span data-stu-id="583c7-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="583c7-115">uma Web Part do SharePoint</span><span class="sxs-lookup"><span data-stu-id="583c7-115">a SharePoint web part</span></span> 

![CG-howitworks. png](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="583c7-117">Requisitos e permissões</span><span class="sxs-lookup"><span data-stu-id="583c7-117">Requirements and Permissions</span></span>

<span data-ttu-id="583c7-118">Antes de começar a usar este guia, verifique se os caminhos de aprendizado foram configurados pelo administrador de locatários do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="583c7-118">Before getting started with this guide, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="583c7-119">Se você não tiver certeza sobre a configuração, entre em contato com o administrador de locatários do SharePoint para verificar se os caminhos de aprendizado foram provisionados.</span><span class="sxs-lookup"><span data-stu-id="583c7-119">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="583c7-120">Além disso, certifique-se de obter a URL do site do SharePoint cursores de aprendizado.</span><span class="sxs-lookup"><span data-stu-id="583c7-120">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="583c7-121">Se você for o administrador de locatários e os caminhos de aprendizado não foram provisionados, confira [provisionar cursores de aprendizado](custom_provision.md).</span><span class="sxs-lookup"><span data-stu-id="583c7-121">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="583c7-122">Permissões para provisionar os caminhos de aprendizado</span><span class="sxs-lookup"><span data-stu-id="583c7-122">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="583c7-123">Administrador de locatários, também conhecido como administrador global do Office 365</span><span class="sxs-lookup"><span data-stu-id="583c7-123">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="583c7-124">Administrador do conjunto de sites do SharePoint com permissões de proprietário no site</span><span class="sxs-lookup"><span data-stu-id="583c7-124">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="583c7-125">Permissões para usar recursos de administração de caminhos de aprendizado</span><span class="sxs-lookup"><span data-stu-id="583c7-125">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="583c7-126">Administrador de Conjunto de Sites</span><span class="sxs-lookup"><span data-stu-id="583c7-126">Site Collection Administrator</span></span>
- <span data-ttu-id="583c7-127">Proprietário do SharePoint ou permissões de membro</span><span class="sxs-lookup"><span data-stu-id="583c7-127">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="583c7-128">Permissões para usar o site de cursores de aprendizado como um usuário</span><span class="sxs-lookup"><span data-stu-id="583c7-128">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="583c7-129">Office 365 permissões de usuário/permissões de visitante de site do SharePoint ou mais</span><span class="sxs-lookup"><span data-stu-id="583c7-129">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="583c7-130">Introdução à personalização</span><span class="sxs-lookup"><span data-stu-id="583c7-130">Get started with customization</span></span>
<span data-ttu-id="583c7-131">Quando tiver certeza de que tem as permissões necessárias para personalizar o site e a Web Part, é hora de começar a usar o processo de personalização.</span><span class="sxs-lookup"><span data-stu-id="583c7-131">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="583c7-132">Para começar, consulte [ir para o site de cursores de aprendizado](custom_goto.md).</span><span class="sxs-lookup"><span data-stu-id="583c7-132">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>