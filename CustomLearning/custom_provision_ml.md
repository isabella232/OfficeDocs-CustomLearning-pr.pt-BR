---
author: pkrebs
ms.author: pkrebs
title: Provisionar uma nova solução multilíngue de caminhos de aprendizado
ms.date: 02/10/2019
description: Provisionar o site de caminhos de aprendizado do Microsoft 365 por meio do serviço de provisionamento do SharePoint
ROBOTS: NOINDEX, NOFOLLOW
ms.openlocfilehash: 6948162d8a96c9a6582484c5f4fc8acad18405a7
ms.sourcegitcommit: f355885fb93d66abf61df535fa704ccdb8df9b64
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/05/2020
ms.locfileid: "45038991"
---
# <a name="provision-a-new-learning-pathways-multilingual-solution"></a>Provisionar uma nova solução multilíngue de caminhos de aprendizado
As organizações que não têm caminhos de aprendizado provisionados em seus locatários podem usar o serviço de provisionamento do SharePoint para adicionar a solução de caminhos de aprendizado multilíngue. Com esta opção, o modelo de cursores de aprendizado do SharePoint é traduzido em nove idiomas e pode ser usado com um mínimo de modificações. 

> [!IMPORTANT]
> Se você já tiver os caminhos de aprendizado provisionados em seu locatário, é recomendável seguir o caminho de [atualização](custom_update_ml.md) para os caminhos de aprendizado. Se você instalar os caminhos de aprendizado sobre uma instância existente no seu locatário, as alterações feitas no modelo de site ou nas listas de execução de cursores de aprendizado poderão ser perdidas.

## <a name="prerequisites-for-multilingual-support"></a>Pré-requisitos para suporte multilíngue
 
Para configurar com êxito os caminhos de aprendizado do Microsoft 365 com o serviço de provisionamento, a pessoa que está fazendo o provisionamento deve atender aos seguintes pré-requisitos: 
 
- Os caminhos de aprendizado do provisionamento de pessoas devem ser um administrador de locatários do locatário em que os caminhos de aprendizado serão provisionados.  
- Um catálogo de aplicativos do locatário deve estar disponível na opção aplicativos do centro de administração do SharePoint. Se sua organização não tiver um catálogo de aplicativos de locatário do SharePoint, consulte a [documentação do SharePoint Online](https://docs.microsoft.com/sharepoint/use-app-catalog) para criar um. Você deve aguardar pelo menos duas horas após criar o catálogo de aplicativos antes de provisionar os caminhos de aprendizado.  
- Os caminhos de aprendizado do provisionamento de pessoas devem ser proprietários de conjunto de sites do catálogo de aplicativos do locatário. Se os caminhos de aprendizado de provisionamento de pessoa não forem um proprietário de conjunto de sites do catálogo de aplicativos, [conclua estas instruções](addappadmin.md) e continue. 

## <a name="ensure-the-tenant-admin-account-doesnt-have-a-language-selected"></a>Garantir que a conta de administração de locatário não tenha um idioma selecionado
Antes de provisionar os caminhos de aprendizado, certifique-se de que a conta de administrador do locatário não tenha um idioma selecionado. Confira aqui como verificar se a conta de administrador não tem um idioma selecionado. 
1.  Com seu perfil de administrador de borda, acesse office.com.
2.  Insira as credenciais do usuário (se necessário).
3.  No Microsoft 365, clique em **todos os aplicativos** > Delve. 
4.  Clique **em**  >  **Atualizar perfil**.
5.  Role para baixo na página e clique em **como alterar as configurações de idioma e regionais**.
6.  Clique **aqui**e, em seguida, clique nas reticências **...**.
7.  Em **meus idiomas de exibição**, você não deve ver **idiomas selecionados**. Se um idioma for selecionado, desmarque-a.

### <a name="to-provision-learning-pathways"></a>Para provisionar os caminhos de aprendizado

1. Vá para a [página de solução de cursores de aprendizado da Microsoft 365](https://provisioning.sharepointpnp.com/details/3df8bd55-b872-4c9d-88e3-6b2f05344239).
2. Clique em **Adicionar ao seu locatário**. Se você não estiver conectado ao seu locatário, o serviço de provisionamento solicitará suas credenciais de administrador de locatário. 
3. Na caixa de diálogo permissões solicitadas, selecione **consentimento em nome da sua organização** e selecione **aceitar**.

O serviço de provisionamento requer essas permissões para criar o catálogo de aplicativos do locatário, instalar o aplicativo no catálogo de aplicativos do locatário e provisionar o modelo de site. Não há impacto geral no locatário. Essas permissões são explicitamente usadas com o objetivo da instalação da solução. Você deve aceitar essas permissões para continuar a instalação.

4. Preencha os campos da página informações de provisionamento, conforme apropriado para sua instalação. No mínimo, insira o endereço de email para o qual você deseja obter notificações sobre o processo de provisionamento e a URL de destino do seu site a ser provisionado.  
> [!NOTE]
> Torne a URL de destino do seu site um tanto amigável para seus funcionários, como "/sites/MyTraining" ou "/teams/LearnMicrosoft365".

![inst_options.png](media/inst_options.png)

6. Clique em **provisionar** quando estiver pronto para instalar os caminhos de aprendizado no seu ambiente de locatário.  O processo de provisionamento pode levar até 15 minutos. Você será notificado por email quando o site estiver pronto. 

> [!IMPORTANT]
> O administrador de locatários que provisiona o site de caminhos de aprendizado deve ir para o site e, em seguida, abrir **CustomLearningAdmin. aspx** para inicializar as propriedades de administração de caminhos de aprendizado. No momento, o administrador de locatários também deve atribuir proprietários ao site. 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Validar o êxito do provisionamento e inicializar a lista CustomConfig

Quando o provisionamento é concluído, o administrador do locatário que provisionou o site recebe um email do serviço de provisionamento PnP. O email contém um link para o site. Neste ponto, o administrador de locatário deve ir para o site usando o link fornecido no email e configurar o site para o primeiro uso:

- Acesse `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`. Abrir **CustomLearningAdmin. aspx** Inicializa o item de lista **CustomConfig** que configura os caminhos de aprendizado para o primeiro uso. Você verá uma página parecida com esta:

![cg-adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Adicionar proprietários ao site
Como administrador de locatários, é improvável que você seja a pessoa que personaliza o site, portanto, você precisará atribuir alguns proprietários ao site. Os proprietários têm privilégios administrativos no site para que eles possam modificar as páginas do site e remarcar o site. Eles também têm a capacidade de ocultar e Mostrar conteúdo e criar subcategorias e playlists personalizadas.  

1. No menu **configurações** do SharePoint, clique em **permissões do site**.
2. Clique em **configurações de permissão avançadas**.
3. Clique em **Microsoft 365 cursores de aprendizado**.
4. Clique em **novo**  >  **Adicionar usuários a este grupo**e adicione as pessoas que você deseja que sejam proprietários. 
5. Adicione um link para [explorar o site](custom_exploresite.md) na mensagem de compartilhamento e clique em **compartilhar**.

## <a name="add-translators-to-the-site"></a>Adicionar tradutores ao site
Se você estiver usando tradutores para o site, poderá atribuir permissões a eles. Os tradutores exigem permissões de membros ou superiores. 

## <a name="choose-options-for-using-multiple-languages-on-the-site"></a>Escolha opções para usar vários idiomas no site
O serviço de provisionamento do SharePoint cria o site de cursores de aprendizado em nove idiomas. As seguintes recomendações se aplicam:
- Desative os idiomas que você não deseja suportar
- Se você não estiver dando suporte a um site multilíngue, desative o recurso multilíngue. Consulte a seção "desativar o suporte multilíngue" mais adiante neste tópico.

### <a name="remove-languages-you-dont-want-to-support"></a>Remover idiomas que você não deseja suportar
Para organizações que optam por suportar apenas um idioma, além do idioma padrão Inglês, recomendamos remover idiomas que não são suportados. 
1. No site de caminhos de aprendizado, selecione **configurações** no canto superior direito da página e, em seguida, selecione **informações do site**.
2. Na parte inferior do painel de informações do site, selecione **Exibir todas as configurações do site**.
3. Em **Administração do site**, selecione **configurações de idioma**.
4. Em **habilitar páginas e notícias a serem traduzidas em vários idiomas**, **deslize a opção para ativar.** Ele deve estar ativado por padrão.
5. Em Adicionar ou remover idiomas do site, clique em **remover** para remover os idiomas que você não precisa para o site. Veja a seguir um exemplo da página de configurações de idioma para mostrar o italiano suportado para o site, além do idioma padrão inglês.

![custom_update_ml_langsettings.png](media/custom_update_ml_langsettings.png)

> [!NOTE]
> Ao remover idiomas, não é possível remover o idioma padrão em inglês. 

### <a name="assign-translators"></a>Atribuir tradutores
Se você for traduzir páginas, opcionalmente atribua um ou mais tradutores para cada idioma (exceto o idioma padrão do site). 
- Na coluna **Tradutor** , comece a digitar o nome de uma pessoa que você deseja que seja um tradutor e selecione o nome na lista. 

> [!NOTE]
> Qualquer pessoa no Active Directory da sua organização pode ser atribuída como um tradutor. Pessoas atribuídas como tradutores não receberão automaticamente as permissões apropriadas. Quando alguém sem permissões de edição para um site tenta acessar o site, ele será direcionado para uma página da Web onde poderá solicitar acesso.

## <a name="turn-off-multilingual-support"></a>Desativar o suporte multilíngue
Se você não quiser um site multilíngue, por exemplo, se quiser um site somente em inglês, recomendamos que você desative o recurso multilíngue. 

1. No site de caminhos de aprendizado, selecione **configurações** no canto superior direito da página e, em seguida, selecione **informações do site**.
2. Na parte inferior do painel de informações do site, selecione **Exibir todas as configurações do site**.
3. Em **Administração do site**, selecione **configurações de idioma**.
4. Em **habilitar páginas e notícias a serem traduzidas em vários idiomas**, **deslize a opção para ativar.** Ele deve estar ativado por padrão.
- Em **habilitar páginas e notícias a serem traduzidas**, selecione **desativado**. 

### <a name="add-languages"></a>Adicionar idiomas
Os caminhos de aprendizado dão suporte a 9 idiomas, mas é recomendável que você adicione apenas os idiomas de que você precisa para suportar o site de cursores de aprendizado. Você pode adicionar idiomas a qualquer momento. 
- Em **Adicionar ou remover idiomas do site**, comece a digitar o nome de um idioma em **selecionar ou digite um idioma**ou escolha um idioma na lista suspensa. Você pode repetir essa etapa para adicionar vários idiomas. Você pode adicionar ou remover idiomas do seu site a qualquer momento, voltando para esta página.



