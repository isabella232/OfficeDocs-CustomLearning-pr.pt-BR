---
author: pkrebs
ms.author: pkrebs
title: Personalizar os caminhos de aprendizagem
ms.date: 02/18/2019
manager: bpardi
audience: admin
ms.topic: article
description: Personalizar os caminhos de aprendizagem
ms.service: sharepoint-online
ms.openlocfilehash: a5087096ec3bd7c1194aab9dd089276fc196a736
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999497"
---
# <a name="customize-learning-pathways"></a><span data-ttu-id="03f29-103">Personalizar os caminhos de aprendizagem</span><span class="sxs-lookup"><span data-stu-id="03f29-103">Customize learning pathways</span></span>

<span data-ttu-id="03f29-104">Os caminhos de aprendizado do Microsoft 365 fornece várias maneiras de personalizar o conteúdo para sua organização.</span><span class="sxs-lookup"><span data-stu-id="03f29-104">Microsoft 365 learning pathways provides a variety of ways that you can customize content for your organization.</span></span> <span data-ttu-id="03f29-105">Por exemplo, você pode:</span><span class="sxs-lookup"><span data-stu-id="03f29-105">For example, you can:</span></span>  
- <span data-ttu-id="03f29-106">Modificar os caminhos de aprendizado do site do SharePoint - Alterar o nome do site, o logotipo e eles.</span><span class="sxs-lookup"><span data-stu-id="03f29-106">Modify the learning pathways SharePoint site - Change the site name, logo, and them.</span></span> <span data-ttu-id="03f29-107">Modifique a página Fazer Perguntas e Obter Ajuda para criar sua própria Central de Ajuda.</span><span class="sxs-lookup"><span data-stu-id="03f29-107">Modify the Ask Questions and Get Help page to create your own Help Center.</span></span> 
- <span data-ttu-id="03f29-108">Ocultar ou mostrar conteúdo para refletir os serviços ou recursos suportados em sua organização</span><span class="sxs-lookup"><span data-stu-id="03f29-108">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="03f29-109">Criar playlists personalizadas e subcategorias criadas especificamente para as necessidades do usuário</span><span class="sxs-lookup"><span data-stu-id="03f29-109">Build custom playlists and subcategories crafted specifically for your user's needs</span></span>
- <span data-ttu-id="03f29-110">Crie páginas de aterrissagem com conteúdo filtrado para dar suporte a resultados de negócios, como impulsionar a adoção do Microsoft Teams, outlook mobile ou trabalhar de forma mais colaborativa com o Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="03f29-110">Build landing pages with content filtered to support business outcomes, such as driving the adoption of Microsoft Teams, Outlook mobile, or working more collaboratively with Microsoft 365.</span></span>

![Coleção de fotos de caminhos de aprendizado geral da Microsoft.](media/cg-introducing.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="03f29-112">Requisitos e Permissões</span><span class="sxs-lookup"><span data-stu-id="03f29-112">Requirements and Permissions</span></span>

<span data-ttu-id="03f29-113">Antes de começar com as diretrizes Personalizar caminhos de aprendizado, verifique se os caminhos de aprendizado foram definidos pelo administrador de locatários do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="03f29-113">Before getting started with the Customize learning pathways guidance, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="03f29-114">Se você não tiver certeza se foi configurada, entre em contato com o administrador de locatários do SharePoint para verificar se os caminhos de aprendizado foram provisionados.</span><span class="sxs-lookup"><span data-stu-id="03f29-114">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="03f29-115">Também certifique-se de obter a URL do site do SharePoint de caminhos de aprendizado.</span><span class="sxs-lookup"><span data-stu-id="03f29-115">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="03f29-116">Se você for o Administrador de Locatários e os caminhos de aprendizado não foram provisionados, consulte [Provision learning pathways](custom_provision.md).</span><span class="sxs-lookup"><span data-stu-id="03f29-116">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="03f29-117">Permissões para provisionar caminhos de aprendizado</span><span class="sxs-lookup"><span data-stu-id="03f29-117">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="03f29-118">Administrador de Locatários, também conhecido como Administrador Global do Office 365</span><span class="sxs-lookup"><span data-stu-id="03f29-118">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="03f29-119">Administrador de Conjunto de Sites do SharePoint com Permissões de proprietário no site</span><span class="sxs-lookup"><span data-stu-id="03f29-119">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="03f29-120">Permissões para usar os recursos de administração de caminhos de aprendizado</span><span class="sxs-lookup"><span data-stu-id="03f29-120">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="03f29-121">Administrador de Conjunto de Sites</span><span class="sxs-lookup"><span data-stu-id="03f29-121">Site Collection Administrator</span></span>
- <span data-ttu-id="03f29-122">Permissões de proprietário ou membro do SharePoint</span><span class="sxs-lookup"><span data-stu-id="03f29-122">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="03f29-123">Permissões para usar o site de caminhos de aprendizado como usuário</span><span class="sxs-lookup"><span data-stu-id="03f29-123">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="03f29-124">Permissões de usuário do Office 365, permissões de visitante do Site do SharePoint ou superior.</span><span class="sxs-lookup"><span data-stu-id="03f29-124">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="03f29-125">Começar a usar a personalização</span><span class="sxs-lookup"><span data-stu-id="03f29-125">Get started with customization</span></span>
<span data-ttu-id="03f29-126">Depois de garantir que você tem as permissões necessárias para personalizar o site e a Web Part, é hora de começar o processo de personalização.</span><span class="sxs-lookup"><span data-stu-id="03f29-126">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="03f29-127">Para começar, consulte [Ir para o site de caminhos de aprendizagem.](custom_goto.md)</span><span class="sxs-lookup"><span data-stu-id="03f29-127">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>