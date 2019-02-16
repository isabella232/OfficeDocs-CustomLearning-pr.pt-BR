---
author: pkrebs
ms.author: pkrebs
title: Visão geral
ms.date: 02/15/2019
description: Visão geral do aprendizado personalizado para o Office 365 para administradores
ms.openlocfilehash: c4b9679ae5a7158306bfd53e345f8e892ab206bc
ms.sourcegitcommit: afb5502604d271f49f6d1133db9dfc499f710eec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2019
ms.locfileid: "30064981"
---
# <a name="overview-of-custom-learning"></a><span data-ttu-id="545cb-103">Visão geral da aprendizagem personalizada</span><span class="sxs-lookup"><span data-stu-id="545cb-103">Overview of Custom Learning</span></span>
<span data-ttu-id="545cb-p101">Apresentando o aprendizado personalizado para o Office 365, uma nova solução da Microsoft projetada para acelerar o uso e a adoção do Office 365 dentro de uma organização. Com o aprendizado personalizado, você pode:</span><span class="sxs-lookup"><span data-stu-id="545cb-p101">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization. With Custom Learning, you can:</span></span>

- <span data-ttu-id="545cb-p102">Personalizar o aprendizado personalizado para o Office 365 em seu ambiente. Modifique as páginas do site com sua marca e logotipo, eventos de treinamento e informações de suporte. Ocultar e mostrar o conteúdo de serviços ou recursos que não têm suporte em sua organização.</span><span class="sxs-lookup"><span data-stu-id="545cb-p102">Tailor Custom Learning for Office 365 to your environment. Modify site pages with your brand and logo, training events, and support info. Hide and show content for services or features that are not supported in your organization.</span></span> 
- <span data-ttu-id="545cb-109">Deixe a Microsoft manter seu conteúdo e seus usuários atualizados – o aprendizado personalizado oferece uma alimentação dinâmica de conteúdo de aprendizado que a Microsoft mantém atualizada.</span><span class="sxs-lookup"><span data-stu-id="545cb-109">Let Microsoft keep your content and users up-to-date – Custom Learning provides a dynamic feed of learning content that Microsoft keeps up-to-date.</span></span> 
- <span data-ttu-id="545cb-110">Criar categorias e listas de reprodução personalizadas que refletem as políticas, os procedimentos e a cultura da sua organização, permitindo que os usuários criem habilidades com conteúdo de aprendizado criado especificamente para suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="545cb-110">Build categories and custom playlists reflecting your organization’s policies, procedures, and culture, enabling users to build skills with learning content crafted specifically to their needs.</span></span>

![cg_introducing. png](media/cg_introducing.png)

## <a name="how-does-custom-learning-word"></a><span data-ttu-id="545cb-112">Como o Word de aprendizado personalizado?</span><span class="sxs-lookup"><span data-stu-id="545cb-112">How does Custom Learning word?</span></span>
<span data-ttu-id="545cb-113">O aprendizado personalizado para o Office 365 (aprendizado personalizado para curto) consiste em três partes:</span><span class="sxs-lookup"><span data-stu-id="545cb-113">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
- <span data-ttu-id="545cb-114">um site de comunicação do SharePoint</span><span class="sxs-lookup"><span data-stu-id="545cb-114">a SharePoint communication site</span></span>
- <span data-ttu-id="545cb-115">uma Web Part do SharePoint</span><span class="sxs-lookup"><span data-stu-id="545cb-115">a SharePoint web part</span></span>
- <span data-ttu-id="545cb-116">um feed ativo de conteúdo de um catálogo do Microsoft Online</span><span class="sxs-lookup"><span data-stu-id="545cb-116">a live feed of content from a Microsoft online catalog</span></span>

![cg_howitworks. png](media/cg_howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="545cb-118">Requisitos e permissões</span><span class="sxs-lookup"><span data-stu-id="545cb-118">Requirements and Permissions</span></span>
<span data-ttu-id="545cb-p103">O aprendizado personalizado para o Office 365 deve ser instalado pelo administrador de locatários da sua organização-alguém que tenha permissão de administrador de locatários. Antes de começar a usar esses procedimentos de personalização abordados neste guia, verifique se o aprendizado personalizado foi configurado por um administrador de locatários do SharePoint. Se você não tiver certeza, entre em contato com o administrador de locatários do SharePoint para verificar se o aprendizado personalizado foi instalado. Além disso, certifique-se de obter a URL do site do SharePoint de aprendizado personalizado. Se você for o administrador de locatários e o aprendizado personalizado não tiverem sido instalados, consulte o guia de instalação do aprendizado personalizado do Office 365.</span><span class="sxs-lookup"><span data-stu-id="545cb-p103">Custom Learning for Office 365 must be installed by your organization’s tenant administrator - someone who has Tenant Administrator permission. Before getting started with this customization procedures covered in this guide, ensure that Custom Learning has been set up by a SharePoint tenant administrator. If you’re not sure, contact your SharePoint tenant administrator to verify that Custom Learning has been installed. Also be sure to get the URL of the Custom Learning SharePoint site. If you are the Tenant Administrator and Custom Learning has not been installed, see the Custom Learning for Office 365 Installation Guide.</span></span> 

### <a name="permissions-required-for-custom-learning"></a><span data-ttu-id="545cb-124">Permissões necessárias para o aprendizado personalizado</span><span class="sxs-lookup"><span data-stu-id="545cb-124">Permissions required for Custom Learning</span></span> 
<span data-ttu-id="545cb-125">Aqui está uma divisão das permissões necessárias para instalar, personalizar e usar o aprendizado personalizado.</span><span class="sxs-lookup"><span data-stu-id="545cb-125">Here’s a breakdown of the permissions required for installing, customizing, and using Custom Learning.</span></span> 

<span data-ttu-id="545cb-126">**Permissões para instalar o aprendizado personalizado**</span><span class="sxs-lookup"><span data-stu-id="545cb-126">**Permissions to install Custom Learning**</span></span>
- <span data-ttu-id="545cb-127">Administrador global do Office 365</span><span class="sxs-lookup"><span data-stu-id="545cb-127">Office 365 Global Administrator</span></span>
- <span data-ttu-id="545cb-128">Administrador do SharePoint</span><span class="sxs-lookup"><span data-stu-id="545cb-128">SharePoint Administrator</span></span>

<span data-ttu-id="545cb-129">**Permissões para usar recursos personalizados de administração de aprendizado**</span><span class="sxs-lookup"><span data-stu-id="545cb-129">**Permissions to use Custom Learning Administration features**</span></span>
- <span data-ttu-id="545cb-130">Office 365 SharePoint Administrator/permissões de proprietário de site do SharePoint</span><span class="sxs-lookup"><span data-stu-id="545cb-130">Office 365 SharePoint Administrator/SharePoint Site Owner Permissions</span></span>
- <span data-ttu-id="545cb-131">Administrador do conjunto de sites do SharePoint/permissões de proprietário do site do SharePoint</span><span class="sxs-lookup"><span data-stu-id="545cb-131">SharePoint Site Collection Administrator/SharePoint Site Owner Permissions</span></span>

<span data-ttu-id="545cb-132">**Para usar o site de aprendizado personalizado como usuário**</span><span class="sxs-lookup"><span data-stu-id="545cb-132">**To use the Custom Learning site as a user**</span></span>
- <span data-ttu-id="545cb-133">Office 365 permissões de usuário/permissões de visitante de site do SharePoint ou mais</span><span class="sxs-lookup"><span data-stu-id="545cb-133">Office 365 user permissions/SharePoint Site Visitor Permissions or higher</span></span>
- <span data-ttu-id="545cb-134">Se você não tiver certeza se recebeu as permissões necessárias, contate o administrador de locatários do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="545cb-134">If you’re not sure if you’ve been granted the necessary permissions, contact your SharePoint Tenant Administrator.</span></span>

### <a name="next-steps"></a><span data-ttu-id="545cb-135">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="545cb-135">Next Steps</span></span>

- [<span data-ttu-id="545cb-136">Personalizar e compartilhar listas de reprodução</span><span class="sxs-lookup"><span data-stu-id="545cb-136">Customize and Share Playlists</span></span>](customplaylist.md)
- [<span data-ttu-id="545cb-137">Adoção de drive</span><span class="sxs-lookup"><span data-stu-id="545cb-137">Drive Adoption</span></span>](driveadoption.md) 