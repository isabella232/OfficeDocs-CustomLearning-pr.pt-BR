---
author: pkrebs
ms.author: pkrebs
title: Provisione o site de Aprendizado Personalizado
ms.date: 02/10/2019
description: Provisionar o site Aprendizagem Personalizada para o Office 365 por meio do Mecanismo de Provisionamento do SharePoint
ms.service: sharepoint online
ms.openlocfilehash: be45ade7588f08801062710d310ca967ddd23926
ms.sourcegitcommit: 907c657e7cc5a4a44d2b9f38cc35fea9ac5c5943
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2021
ms.locfileid: "51162918"
---
# <a name="provision-custom-learning"></a>Provisione o Aprendizado Personalizado

Com o Serviço de Provisionamento do SharePoint Online, um Administrador de Locatários do Office 365 pode iniciar o processo de provisionamento com alguns cliques simples. O Serviço de Provisionamento é a maneira recomendada de provisionar o Aprendizado Personalizado. É rápido, fácil e leva apenas alguns minutos para iniciar o processo. No entanto, antes de começar com o Serviço de Provisionamento, certifique-se de que você tenha atendido aos pré-requisitos para provisionamento.

## <a name="prerequisites"></a>Pré-requisitos
 
Para configurar com êxito o Aprendizado Personalizado com o Serviço de Provisionamento do Serviço de Provisionamento do [SharePoint Online,](https://provisioning.sharepointpnp.com)a pessoa que está fazendo o provisionamento deve atender aos seguintes pré-requisitos: 
 
- A pessoa que provisiona o Custom Learning deve ser um Administrador de Locatário do locatário onde o Aprendizado Personalizado será provisionado.  
- Um Catálogo de Aplicativos de locatário deve estar disponível na opção Aplicativos do Centro de Administração do SharePoint. Se sua organização não tiver um catálogo de aplicativos de locatários do SharePoint, consulte a documentação do [SharePoint Online](/sharepoint/use-app-catalog) para criar um.  
- A pessoa que provisiona o Custom Learning deve ser um Proprietário do Conjunto de Sites do Catálogo de Aplicativos de Locatário. Se a pessoa que provisiona o Custom Learning não for um Proprietário do Conjunto de Sites do Catálogo de [Aplicativos, conclua essas instruções](addappadmin.md) e continue. 

### <a name="to-provision-custom-learning"></a>Para provisionar o Aprendizado Personalizado

1. Vá para http://provisioning.sharepointpnp.com e **entre** no canto superior direito da home page.  Entre com as credenciais do locatário direcionado onde você planeja instalar o modelo de site.

![pnphome.png](media/inst_signin.png)

2. Limpe o **Consentimento em nome da sua organização e** selecione **Aceitar**.

![pol](media/inst_perms.png)

3. Selecione **Aprendizagem Personalizada para o Office 365** na galeria de soluções.

![pol](media/inst_select.png)

4. Na home page da solução, selecione **Adicionar ao locatário**

![inst_select.png](media/inst_add.png)

5. Preencha os campos na página de informações de provisionamento, conforme apropriado à sua instalação. No mínimo, insira o endereço de email para o qual você deseja receber notificações sobre o processo de provisionamento e a URL de destino para o qual seu site deve ser provisionado.  
> [!NOTE]
> Tornar a URL de destino do seu site algo amigável para seus funcionários, como "/sites/MyTraining" ou "/teams/LearnOffice365".

![inst_options.png](media/inst_options.png)

6. Selecione **Provisionar** quando estiver pronto para instalar o Aprendizado Personalizado em seu ambiente de locatário.  O processo de provisionamento levará até 15 minutos. Você será notificado por email (no endereço de email para receber notificação que você digitou na página de Provisionamento) quando o site estiver pronto para ser acessado.

> [!IMPORTANT]
> O Administrador de Locatários que provisiona o site de Aprendizado Personalizado deve acessar o site e, em seguida, abrir CustomLearningAdmin.aspx para inicializar as propriedades de Administrador de Aprendizagem Personalizada. Neste momento, o Administrador de Locatários também deve atribuir Proprietários ao site. 

## <a name="validate-provisioning-success"></a>Validar o sucesso do provisionamento

Quando o provisionamento é concluído, o Administrador de Locatário recebe um email do Serviço de Provisionamento PnP. O administrador pode copiar o link para o site fornecido no email e seguir as instruções para ir para o site. Como alternativa, o administrador de locatários pode navegar até <YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx. Isso inicializa o item de lista CustomConfig que configura o Custom Learning para seu primeiro uso. A pessoa que abre esta página pela primeira vez deve ser um Administrador de Locatário, Administrador do Conjunto de Sites ou Proprietário do site. Você deve ver uma página com esta aparência: 

## <a name="add-owners-to-site"></a>Adicionar proprietários ao site
Como Administrador de Locatários, é improvável que você seja a pessoa que personalização do site, portanto, você precisará atribuir Proprietários ao site. Os proprietários têm privilégios administrativos no site para que possam modificar páginas do site e renomear o site. Eles também têm a capacidade de ocultar e mostrar o conteúdo fornecido por meio da Web Part de Aprendizagem Personalizada. Eles também terão a capacidade de criar playlist personalizada e atribuí-las a subcategorias personalizadas.  

1. No menu Configurações **do** SharePoint, clique em **Permissões do Site.**
2. Clique **em Configurações avançadas de Permissão**.
3. Clique em Aprendizagem personalizada para proprietários do **Office 365.**
4. Clique **em Novo** Adicionar Usuários a esse  >  **grupo,** adicione as pessoas que você deseja que sejam Proprietários e clique em **Compartilhar**.

8. Clique na **opção** A seguir no canto superior direito da página para seguir o site.  

### <a name="next-steps"></a>Próximas etapas
- Explore o [conteúdo padrão](sitecontent.md) incluído na webpart.