---
author: pkrebs
ms.author: pkrebs
title: ProVisionar o site de aprendizado personalizado
ms.date: 02/10/2019
description: ProVisionar o aprendizado personalizado para o site do Office 365 por meio do mecanismo de provisionamento do SharePoint
ms.openlocfilehash: 868708f9f096c84d5ebc5f9bc4e21e558da84d2b
ms.sourcegitcommit: 5ea8d7fdc255ef7de06f41b3c794bc40551cf5bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30577857"
---
# <a name="provision-custom-learning"></a>ProVisionar aprendizado personalizado 

Com o serviço de provisionamento do SharePoint Online, um administrador de locatários do Office 365 pode iniciar o processo de provisionamento com alguns cliques simples. O serviço de provisionamento é a maneira recomendada de provisionar o aprendizado personalizado. É rápido, fácil e leva apenas alguns minutos para iniciar o processo. Antes de começar a usar o serviço de provisionamento, no entanto, verifique se você atendeu aos pré-requisitos de provisionamento.

## <a name="prerequisites"></a>Pré-requisitos
 
Para configurar com êxito a aprendizagem personalizada com o serviço de provisionamento, a pessoa que está fazendo o provisionamento deve atender aos seguintes pré-requisitos: 
 
- O aprendizado personalizado de provisionamento de pessoa deve ser um administrador de locatários do locatário onde o aprendizado personalizado será provisionado.  
- Um catálogo de aplicativos do locatário deve estar disponível na opção aplicativos do centro de administração do SharePoint. Se sua organização não tiver um catálogo de aplicativos de locatário do SharePoint, consulte a [documentação do SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) para criar um.  
- O aprendizado personalizado de provisionamento de pessoa deve ser um proprietário de conjunto de sites do catálogo de aplicativos do locatário. Se a pessoa que estiver Provisionando o aprendizado personalizado não for um proprietário do conjunto de sites do catálogo de aplicativos, [Complete estas instruções](addappadmin.md) e continue. 

### <a name="to-provision-custom-learning"></a>Para provisionar o aprendizado personalizado

1. Vá para http://provisioning.sharepointpnp.com e **entre** no canto superior direito da Home Page.  Entre com as credenciais do locatário de destino no qual você planeja instalar o modelo de site.

![pnphome. png](media/inst_signin.png)

2. DesMarque o **consentimento em nome da sua organização** e selecione **aceitar**.

![no](media/inst_perms.png)

3. Role para baixo na página, selecione a guia **soluções** e, em seguida, selecione **aprendizado personalizado para o Office 365**. 

![no](media/inst_select.png)

4. Selecione **Adicionar ao seu locatário**

![inst_select. png](media/inst_add.png)

5. Preencha os campos da página informações de provisionamento, conforme apropriado para sua instalação. No mínimo, insira o endereço de email para o qual você deseja obter notificações sobre o processo de provisionamento e a URL de destino do seu site a ser provisionado.  
> [!NOTE]
> Torne a URL de destino do seu site um tanto amigável para seus funcionários, como "/sites/MyTraining" ou "/teams/LearnOffice365".

![inst_options. png](media/inst_options.png)

6. Selecione **** provisionar quando estiver pronto para instalar o aprendizado personalizado no seu ambiente de locatário.  O processo de provisionamento levará até 15 minutos. Você será notificado por email (para o endereço de email de notificação que você inseriu na página de provisionamento) quando o site estiver pronto para o Access. 

> [!IMPORTANT]
> O administrador de locatários que provisiona o site de aprendizado personalizado deve ir para o site e, em seguida, abrir **CustomLearningAdmin. aspx** para inicializar as propriedades personalizadas de administração de aprendizado. No momento, o administrador de locatários também deve atribuir proprietários ao site. 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Validar o êxito do provisionamento e inicializar a lista CustomConfig

Quando o provisionamento é concluído, o administrador de locatários que provisionou o site recebe um email do serviço de provisionamento PnP. O email contém um link para o site. Neste ponto, o administrador de locatário deve ir para o site usando o link fornecido no email e configurar o site para o primeiro uso:

- Acesse `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`. Abrir **CustomLearningAdmin. aspx** Inicializa o item de lista **CustomConfig** que configura o aprendizado personalizado para o primeiro uso. Você verá uma página parecida com esta:

![CG-adminapppage. png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Adicionar proprietários ao site
Como administrador de locatários, é improvável que você seja a pessoa que personaliza o site, portanto, você precisará atribuir alguns proprietários ao site. Os proprietários têm privilégios administrativos no site para que eles possam modificar as páginas do site e remarcar o site. Eles também podem ocultar e mostrar o conteúdo fornecido por meio da Web Part de aprendizado personalizado. Além disso, eles terão a capacidade de criar uma lista de reprodução personalizada e atribuí-las às subcategorias personalizadas.  

1. No menu **configurações** do SharePoint, clique em **permissões do site**.
2. Clique em **configurações de permissão avançadas**.
3. Clique em **aprendizagem personalizada para proprietários do Office 365**.
4. Clique em **novo** > **Adicionar usuários a este grupo**e adicione as pessoas que você deseja que sejam proprietários. 
5. Adicione um link para [explorar o site](custom_exploresite.md) na mensagem de compartilhamento e clique em **compartilhar**.

### <a name="next-steps"></a>Próximos passos
- Explore o [conteúdo padrão](custom_exploresite.md) fornecido no site e na Web Part.
