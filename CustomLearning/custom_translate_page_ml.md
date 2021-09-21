---
author: pkrebs
ms.author: pkrebs
title: Traduzir páginas do site
ms.date: 07/06/2020
description: Traduzir páginas do site
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 87130512dafe55ddd7dd0ac4f0667efb2108f360
ms.sourcegitcommit: 6005c2551bdea334767e6a056fdcb79533f2c858
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/21/2021
ms.locfileid: "59460919"
---
# <a name="translate-site-pages"></a>Traduzir páginas do site
Antes de começar a traduzir o site de caminhos de aprendizado, é importante entender alguns conceitos-chave de como o recurso multilíngue funciona com caminhos de aprendizado. 
- Informações do site - As traduções de nome de site, logotipo e navegação exigem que o site seja exibido e convertido no perfil de idioma do usuário.  
- A Web Part de caminhos de aprendizado deve ser exibida com o perfil de idioma do usuário para que ela apareça em um idioma que não seja inglês. A Web Part e o conteúdo fornecido pela Microsoft já estão convertidos para você. Para obter mais informações sobre perfis de idiomas, consulte [Change your personal language and regional settings](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7).
- A maneira como você configura os caminhos de aprendizado determina se você traduziu páginas disponíveis. Os novos sites provisionados com o Microsoft 365 do guia de aparência terão páginas traduzidas em nove idiomas disponíveis. Sites ou sites atualizados que você criar exigirá tradução manual. Consulte [Opções de instalação para caminhos de aprendizado multilíngues.](custom_setupoptions_ml.md)
- O suporte multilíngue para caminhos de aprendizado é habilitado SharePoint recursos multilíngues online para sites de comunicação. Para saber mais sobre SharePoint recursos multilíngues online, consulte [Create multilingual communication sites, pages, and news](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c). 

## <a name="working-with-a-newly-provisioned-site"></a>Trabalhando com um site recém-provisionado
Se você provisionou um novo site de caminhos de aprendizagem a partir do Microsoft 365 de guia de aparência, as páginas traduzidas já estarão disponíveis para você. Por padrão, o site fornece as seguintes páginas:

- Home.aspx
- Start-with-Six-Simple-Steps.aspx
- Get-started-with-Microsoft-365.aspx
- Get-started-with-Microsoft-Teams.aspx
- Get-started-with-SharePoint.aspx
- Get-started-with-OneDriive.aspx
- Ask-questions-and-get-help.aspx
- Eventos de treinamento calendar.aspx
- Become-a-Champion.aspx
- Recommended-Playlists.aspx
- Learning de Sucesso do Administrador

## <a name="view-translated-pages-from-the-newly-provisioned-site"></a>Exibir páginas traduzidas do site recém-provisionado
Para se familiarizar com o site de caminhos de aprendizado traduzidos, vamos dar uma olhada em algumas páginas traduzidas.

### <a name="view-the-translated-home-page"></a>Exibir a home page traduzida
Na página Inicial dos caminhos de aprendizado, selecione um idioma no menu suspenso de idiomas, conforme mostrado no exemplo a seguir. No exemplo, você vê italiano selecionado no canto superior direito e todos os elementos da página são convertidos.

![custom_ml página inicial](media/custom_ml_pages_home.png)

### <a name="view-the-translated-microsoft-365-training-page"></a>Exibir a página de Microsoft 365 de treinamento traduzida
Agora vamos dar uma olhada na página de Microsoft 365 de treinamento. 

1. Na home **page** do site de caminhos de aprendizagem, clique **Microsoft 365 treinamento**.
2. No canto superior direito da página, selecione um idioma. Neste exemplo, o italiano está selecionado.

![custom_ml_ de treinamento](media/custom_ml_pages_training.png)

Quais traduções ficam visíveis quando o idioma é selecionado?
- A SharePoint página é traduzida conforme mostrado no gráfico acima. Observe que o texto da faixa de página agora está em italiano.

O que as traduções não estão visíveis?
- O nome do site está em inglês
- A navegação do site está em inglês
- A Web Part de caminhos de aprendizado está em inglês

## <a name="view-the-fully-translated-site"></a>Exibir o site totalmente traduzido 
Para exibir um site totalmente traduzido em um idioma específico, incluindo as páginas do site, a navegação e a Web Part, o idioma pessoal do usuário e as configurações regionais devem ser definidas para esse idioma. Para obter mais informações sobre como definir o idioma e as configurações regionais, consulte [Change your personal language and regional settings](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7). É recomendável usar uma conta separada ou ter outro usuário com as configurações de idioma diferentes exibir as páginas traduzidas.  

## <a name="working-with-an-updated-or-manually-installed-learning-pathways-site"></a>Trabalhando com um site de caminhos de aprendizado atualizado ou instalado manualmente
Se você atualizou um site de Learning de caminhos existente ou instalou manualmente a Web Part em um site existente, será necessário traduzir manualmente as páginas do site. A Web Part e o conteúdo dos caminhos de aprendizado já estão traduzidos e aparecerão no idioma preferencial do usuário. Para traduzir páginas, consulte as instruções a seguir "Criar páginas para os idiomas que você deseja". 

## <a name="create-pages-for-the-languages-you-want"></a>Criar páginas para os idiomas que você deseja
Depois de habilitar seu site para recursos multilíngues e escolher os idiomas que deseja disponibilizar, você pode criar as páginas de conversão que deseja. 

1. Vá para a página de idioma padrão que você deseja disponibilizar em outro idioma.
2. Na barra superior, selecione **Tradução**.
3. Selecione **Criar** para os idiomas que você deseja.

> [!IMPORTANT]
> Depois de criar as páginas de conversão, você deve publicar (ou republicar) a página de idioma padrão para garantir que:
>- As páginas de conversão são mostradas no site de idioma correspondente.
>- As páginas de conversão são exibidas corretamente na Web Part Notícias e nas Web Parts de conteúdo realçadas.
>- O menu suspenso de idioma na parte superior do site inclui todos os idiomas habilitados.
>- Os tradutores são notificados da solicitação de conversão.

Depois de criar as páginas, o status da página (rascunho salvo, publicado e assim por diante) é mostrado no painel de conversão ao lado de cada idioma. Além disso, os tradutores atribuídos serão notificados por email de que uma tradução é solicitada.

### <a name="view-the-fully-translated-site-in-a-specific-language"></a>Exibir o site totalmente traduzido em um idioma específico
Para exibir um site totalmente traduzido em um idioma específico, incluindo as páginas do site, a navegação e a Web Part, o idioma pessoal do usuário e as configurações regionais devem ser definidas para esse idioma. Para obter mais informações sobre como definir o idioma e as configurações regionais, consulte [Change your personal language and regional settings](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7). Observe que é melhor usar uma conta separada ou ter outro usuário com as configurações de idioma diferentes exibir as páginas traduzidas.

## <a name="what-does-a-translator-do"></a>O que faz um tradutor?
 Após a configuração do site em inglês, um usuário com espanhol como idioma pessoal preferencial, por exemplo, edita manualmente e converte o título, a navegação e o conteúdo do rodapé em espanhol. Um usuário com a língua alemã escolhida como idioma pessoal faz a mesma coisa para alemão. Quando o conteúdo for traduzido, ele será exibido para todos os usuários que tenham escolhido esses idiomas. A Web Part escolhe o idioma preferencial do usuário e mostra o conteúdo traduzido nesse idioma. 

Os tradutores traduzem manualmente as cópias da página de idioma padrão para os idiomas especificados. Quando as cópias das páginas são criadas, os tradutores são notificados por email se um tradutor tiver sido especificado. O email inclui um link para a página de idioma padrão e a página de conversão recém-criada. O tradutor:
1. Selecione o **botão Iniciar tradução** no email.
2. Selecione **Editar** no canto superior direito da página e traduza o conteúdo.
3. Quando terminar, selecione **Salvar como rascunho** (se você não estiver pronto para torná-lo visível para os leitores) ou se a página estiver pronta para estar visível para todos que estão usando esse idioma no site, selecione **Publicar** ou **Postar notícias**.

Para obter mais informações sobre o processo de conversão, consulte [Create multilingual communication sites, pages, and news](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c). 

## <a name="updating-the-default-language-page"></a>Atualizando a página de idioma padrão
Quando a página de idioma padrão é atualizada, a página deve ser republicada. Em seguida, os tradutores das páginas de conversão são notificados por email de que uma atualização foi feita para que as atualizações possam ser feitas nas páginas de conversão individuais.

## <a name="set-up-a-multilingual-site-name-navigation-and-footer"></a>Configurar um nome de site multilíngue, navegação e rodapé
Para mostrar o nome, a navegação e o rodapé do seu site nos diferentes idiomas que você disponibilizou, cada um deve ser traduzido manualmente.

Por exemplo, digamos que você criou um site de comunicação com um idioma padrão em inglês e habilitou o site para os idiomas espanhol e alemão. Ao criar um site, você configura o nome e a descrição do site no idioma padrão (neste caso, em inglês). Você também pode atualizar o nome e a descrição do site depois de criá-lo. Então crie os nós de navegação e o conteúdo do rodapé em inglês.

Depois que o site estiver configurado em inglês, um usuário que escolheu espanhol como seu idioma pessoal editará e traduzirá manualmente o título, a descrição, a navegação e o conteúdo do rodapé para espanhol. Um usuário com a língua alemã escolhida como idioma pessoal faz a mesma coisa para alemão. Quando o conteúdo for traduzido, ele será exibido para todos os usuários que tenham escolhido esses idiomas. 

> [! OBSERVAÇÕES]
>- Os usuários que traduzem o conteúdo do site para seus idiomas preferenciais devem ser membros do grupo Proprietários do site ou têm permissões de site equivalentes.
>- Se uma alteração for feita no nome do site, navegação ou rodapé no idioma padrão, o item traduzido correspondente em outro idioma não será atualizado automaticamente, a menos que você opte por substituir traduções de site existentes. Se você fizer isso, o item convertido será substituído pela atualização no idioma padrão e deverá ser traduzido manualmente novamente. Para substituir traduções, vá para a página Idiomas do site para o idioma padrão e selecione Mostrar configurações avançadas. Em seguida, deslize a alternância para Substituir traduções para On. Essa opção não se aplica ao conteúdo de página ou notícias.

### <a name="to-view-the-fully-translated-site-in-a-specific-language"></a>Para exibir o site totalmente traduzido em um idioma específico
Para exibir um site totalmente traduzido em um idioma específico, incluindo as páginas do site, a navegação e a Web Part, o idioma pessoal do usuário e as configurações regionais devem ser definidas para esse idioma. Para obter mais informações sobre como definir o idioma e as configurações regionais, consulte [Change your personal language and regional settings](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7). É recomendável usar uma conta separada ou ter outro usuário com as configurações de idioma diferentes exibir as páginas traduzidas.

## <a name="for-more-information"></a>Para obter mais informações
- Para obter mais informações sobre como traduzir SharePoint de site de comunicação, consulte [Create multilingual communication sites, pages, and news](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).
- Para obter mais informações sobre como personalizar caminhos de aprendizado, consulte [Customize Learning Pathways](custom_overview.md).  
