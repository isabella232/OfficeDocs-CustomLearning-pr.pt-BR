---
author: pkrebs
ms.author: pkrebs
title: Provisionar o site de aprendizado personalizado
ms.date: 02/10/2019
description: Provisionar o aprendizado personalizado para o site do Office 365 por meio do mecanismo de provisionamento do SharePoint
ms.service: sharepoint online
ms.openlocfilehash: feebef7f351aab4cd1efe7f87596dad98dba7536
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233753"
---
# <a name="provision-custom-learning"></a>Provisionar aprendizado personalizado

Com o serviço de provisionamento do SharePoint Online, um administrador de locatários do Office 365 pode iniciar o processo de provisionamento com alguns cliques simples. O serviço de provisionamento é a maneira recomendada de provisionar o aprendizado personalizado. É rápido, fácil e leva apenas alguns minutos para iniciar o processo. Antes de começar a usar o serviço de provisionamento, no entanto, verifique se você atendeu aos pré-requisitos de provisionamento.

## <a name="prerequisites"></a>Pré-requisitos
 
Para configurar com êxito o aprendizado personalizado com o serviço de provisionamento do serviço de [provisionamento do SharePoint Online](https://provisioning.sharepointpnp.com), a pessoa que está fazendo o provisionamento deve atender aos seguintes pré-requisitos: 
 
- O aprendizado personalizado de provisionamento de pessoa deve ser um locatário Administratorof o locatário onde o aprendizado personalizado será provisionado.  
- Um catálogo de aplicativos do locatário deve estar disponível na opção aplicativos do centro de administração do SharePoint. Se sua organização não tiver um catálogo de aplicativos de locatário do SharePoint, consulte a [documentação do SharePoint Online](https://docs.microsoft.com/sharepoint/use-app-catalog) para criar um.  
- O aprendizado personalizado de provisionamento de pessoa deve ser um proprietário de conjunto de sites do catálogo de aplicativos do locatário. Se a pessoa que estiver Provisionando o aprendizado personalizado não for um proprietário do conjunto de sites do catálogo de aplicativos, [Complete estas instruções](addappadmin.md) e continue. 

### <a name="to-provision-custom-learning"></a>Para provisionar o aprendizado personalizado

1. Vá para http://provisioning.sharepointpnp.com e **entre** no canto superior direito da Home Page.  Entre com as credenciais do locatário de destino no qual você planeja instalar o modelo de site.

![pnphome.png](media/inst_signin.png)

2. Desmarque o **consentimento em nome da sua organização** e selecione **aceitar**.

![pol](media/inst_perms.png)

3. Selecione **aprendizagem personalizada para o Office 365** na Galeria de soluções.

![pol](media/inst_select.png)

4. Na página inicial da solução, selecione **Adicionar ao seu locatário**

![inst_select.png](media/inst_add.png)

5. Preencha os campos na página de informações de provisionamento, conforme apropriado à sua instalação. No mínimo, insira o endereço de email para o qual você deseja obter notificações sobre o processo de provisionamento e a URL de destino do seu site a ser provisionado.  
> [!NOTE]
> Torne a URL de destino do seu site um tanto amigável para seus funcionários, como "/sites/MyTraining" ou "/teams/LearnOffice365".

![inst_options.png](media/inst_options.png)

6. Selecione **provisionar** quando estiver pronto para instalar o aprendizado personalizado no seu ambiente de locatário.  O processo de provisionamento levará até 15 minutos. Você será notificado por email (no endereço de email para receber notificação que você digitou na página de Provisionamento) quando o site estiver pronto para ser acessado.

> [!IMPORTANT]
> O administrador de locatários que provisiona o site de aprendizado personalizado deve ir para o site e, em seguida, abrir CustomLearningAdmin. aspx para inicializar as propriedades personalizadas de administração de aprendizado. No momento, o administrador de locatários também deve atribuir proprietários ao site. 

## <a name="validate-provisioning-success"></a>Validar o êxito do provisionamento

Quando o provisionamento é concluído, o administrador do locatário recebe um email do serviço de provisionamento PnP. O administrador pode copiar o link para o site fornecido no email e, em seguida, seguir as instruções para acessar o site. Como alternativa, o administrador de locatários pode navegar para <seu-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx. Isso inicializa o item de lista CustomConfig que configura o aprendizado personalizado para seu primeiro uso. A pessoa que abre a página pela primeira vez deve ser um administrador de locatários, um administrador de conjunto de sites ou proprietário do site. Você verá uma página parecida com esta: 

## <a name="add-owners-to-site"></a>Adicionar proprietários ao site
Como administrador de locatários, é improvável que você seja a pessoa que personaliza o site, portanto, você precisará atribuir proprietários ao site. Os proprietários têm privilégios administrativos no site para que eles possam modificar as páginas do site e remarcar o site. Eles também podem ocultar e mostrar o conteúdo fornecido por meio da Web Part de aprendizado personalizado. Eles também terão a capacidade de criar uma lista de reprodução personalizada e atribuí-las às subcategorias personalizadas.  

1. No menu **configurações** do SharePoint, clique em **permissões do site**.
2. Clique em **configurações de permissão avançadas**.
3. Clique em **aprendizagem personalizada para proprietários do Office 365**.
4. Clique em **novo**  >  **Adicionar usuários a este grupo**, adicione as pessoas que você deseja que sejam proprietários e clique em **compartilhar**.

8. Clique na opção a **seguir** no canto superior direito da página para acompanhar o site.  

### <a name="next-steps"></a>Próximas etapas
- Explore o [conteúdo padrão](sitecontent.md) incluído na Web Part.
