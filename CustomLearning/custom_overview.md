---
author: pkrebs
ms.author: pkrebs
title: Personalizar os caminhos de aprendizado
ms.date: 02/18/2019
description: Personalizar os caminhos de aprendizado
ms.openlocfilehash: 15d782455204cf043937bec03041a85abc9e4ee3
ms.sourcegitcommit: 3b8896c81ad2adbcfdbda658482847af5fccb264
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/30/2019
ms.locfileid: "37886634"
---
# <a name="customize-learning-pathways"></a><span data-ttu-id="cfacb-103">Personalizar os caminhos de aprendizado</span><span class="sxs-lookup"><span data-stu-id="cfacb-103">Customize learning pathways</span></span>

<span data-ttu-id="cfacb-104">Os caminhos de aprendizado do Microsoft 365 oferecem várias maneiras de personalizar o conteúdo da sua organização.</span><span class="sxs-lookup"><span data-stu-id="cfacb-104">Microsoft 365 learning pathways provides a variety of ways that you can customize content for your organization.</span></span> <span data-ttu-id="cfacb-105">Por exemplo, você pode:</span><span class="sxs-lookup"><span data-stu-id="cfacb-105">For example, you can:</span></span>  
- <span data-ttu-id="cfacb-106">Modificar o site de cursores de aprendizado do SharePoint-altere o nome, o logotipo e os itens do site.</span><span class="sxs-lookup"><span data-stu-id="cfacb-106">Modify the learning pathways SharePoint site - Change the site name, logo, and them.</span></span> <span data-ttu-id="cfacb-107">Modificar a página fazer perguntas e obter ajuda para criar seu próprio centro de ajuda.</span><span class="sxs-lookup"><span data-stu-id="cfacb-107">Modify the Ask Questions and Get Help page to create your own Help Center.</span></span> 
- <span data-ttu-id="cfacb-108">Ocultar ou Mostrar conteúdo para refletir os serviços ou recursos compatíveis com a sua organização</span><span class="sxs-lookup"><span data-stu-id="cfacb-108">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="cfacb-109">Criar listas de reprodução e subcategorias personalizadas criadas especificamente para as necessidades do usuário</span><span class="sxs-lookup"><span data-stu-id="cfacb-109">Build custom playlists and subcategories crafted specifically for your user's needs</span></span>
- <span data-ttu-id="cfacb-110">Criar páginas de aterrissagem com conteúdo filtrado para dar suporte a resultados comerciais, como conduzir a adoção do Microsoft Teams, Outlook Mobile ou trabalhar de forma mais colaborativa com o Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cfacb-110">Build landing pages with content filtered to support business outcomes, such as driving the adoption of Microsoft Teams, Outlook mobile, or working more collaboratively with Microsoft 365.</span></span>

![CG-Introducing. png](media/cg-introducing.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="cfacb-112">Requisitos e permissões</span><span class="sxs-lookup"><span data-stu-id="cfacb-112">Requirements and Permissions</span></span>

<span data-ttu-id="cfacb-113">Antes de começar a usar a orientação personalizar cursores de aprendizado, verifique se os caminhos de aprendizado foram configurados pelo administrador de locatários do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cfacb-113">Before getting started with the Customize learning pathways guidance, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="cfacb-114">Se você não tiver certeza sobre a configuração, entre em contato com o administrador de locatários do SharePoint para verificar se os caminhos de aprendizado foram provisionados.</span><span class="sxs-lookup"><span data-stu-id="cfacb-114">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="cfacb-115">Além disso, certifique-se de obter a URL do site do SharePoint cursores de aprendizado.</span><span class="sxs-lookup"><span data-stu-id="cfacb-115">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="cfacb-116">Se você for o administrador de locatários e os caminhos de aprendizado não foram provisionados, confira [provisionar cursores de aprendizado](custom_provision.md).</span><span class="sxs-lookup"><span data-stu-id="cfacb-116">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="cfacb-117">Permissões para provisionar os caminhos de aprendizado</span><span class="sxs-lookup"><span data-stu-id="cfacb-117">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="cfacb-118">Administrador de locatários, também conhecido como administrador global do Office 365</span><span class="sxs-lookup"><span data-stu-id="cfacb-118">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="cfacb-119">Administrador do conjunto de sites do SharePoint com permissões de proprietário no site</span><span class="sxs-lookup"><span data-stu-id="cfacb-119">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="cfacb-120">Permissões para usar recursos de administração de caminhos de aprendizado</span><span class="sxs-lookup"><span data-stu-id="cfacb-120">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="cfacb-121">Administrador de Conjunto de Sites</span><span class="sxs-lookup"><span data-stu-id="cfacb-121">Site Collection Administrator</span></span>
- <span data-ttu-id="cfacb-122">Proprietário do SharePoint ou permissões de membro</span><span class="sxs-lookup"><span data-stu-id="cfacb-122">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="cfacb-123">Permissões para usar o site de cursores de aprendizado como um usuário</span><span class="sxs-lookup"><span data-stu-id="cfacb-123">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="cfacb-124">Office 365 permissões de usuário/permissões de visitante de site do SharePoint ou mais</span><span class="sxs-lookup"><span data-stu-id="cfacb-124">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="cfacb-125">Introdução à personalização</span><span class="sxs-lookup"><span data-stu-id="cfacb-125">Get started with customization</span></span>
<span data-ttu-id="cfacb-126">Quando tiver certeza de que tem as permissões necessárias para personalizar o site e a Web Part, é hora de começar a usar o processo de personalização.</span><span class="sxs-lookup"><span data-stu-id="cfacb-126">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="cfacb-127">Para começar, consulte [ir para o site de cursores de aprendizado](custom_goto.md).</span><span class="sxs-lookup"><span data-stu-id="cfacb-127">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>