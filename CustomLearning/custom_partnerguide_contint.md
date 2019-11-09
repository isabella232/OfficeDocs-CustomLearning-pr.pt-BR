---
author: pkrebs
ms.author: pkrebs
title: Modelos de integração de parceiros
ms.date: 3/9/2019
description: Modelos de integração de parceiros
ms.openlocfilehash: 0d52210c600e14fc9f224fbe6f91645fe4045c45
ms.sourcegitcommit: 6a17a7ab6d28349654520f2c28d08c480e3c7b47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/08/2019
ms.locfileid: "38076015"
---
# <a name="partner-integration-models"></a>Modelos de integração de parceiros
Embora não seja possível complementar o conteúdo de cursores de aprendizado da Microsoft 365 diretamente do serviço de provisionamento do SharePoint Online, há vários modelos de integração que os parceiros podem aproveitar para criar um serviço de agregação de valor alinhado ofertas. Os modelos de integração de parceiros acima são apresentados em ordem de complexidade crescente e níveis de investimento. Portanto, nossa orientação é criar sua especialização e graduação para níveis mais avançados com base em seus modelos de negócios.

![CG-Part-intmodel. png](media/cg-part-intmodel.png) 

## <a name="how-should-i-get-started"></a>Como devo começar? 
Para começar, veja algumas práticas recomendadas a seguir.     

### <a name="1-begin-with-building-expertise-as-an-enabler"></a>1. comece com a criação de expertise como um viabilizador. 
Você pode ajudar uma porcentagem da sua base de clientes imediatamente, habilitando o portal de treinamento de cursores de aprendizado e realizando a ajuda do conteúdo da Microsoft direcionada. Para obter instruções sobre como provisionar os caminhos de https://docs.microsoft.com/en-us/office365/customlearning/custom_provisionaprendizado, consulte.  

### <a name="2-then-extend-your-services-as-an-integrator"></a>2. em seguida, estenda seus serviços como um integrador
Execute uma análise de retorno de automação sobre o investimento, dependendo da quantidade de suas necessidades de integração de conteúdo e/ou serviços. Por exemplo, talvez não seja necessário realizar os custos de desenvolvimento e operacional com relação às diretrizes de integração de conteúdo se você puder criar rapidamente uma lista de reprodução personalizada direcionada que aponte para seu conteúdo para pagamento ou faça referência a seus serviços.

### <a name="3-when-the-return-on-investment-makes-sense--consider-redistribution"></a>3. quando o retorno sobre o investimento faz sentido – considere redistribuição 
Quando o retorno sobre o investimento faz sentido – considere redistribuição (ou trabalhar com os parceiros de cursores de aprendizado relacionados) para criar soluções reempacotadas. Eles são baseados na estrutura de práticas e padrões do SharePoint, que oferece soluções para extrair sites personalizados e implantar em ambientes do cliente 

## <a name="partner-provided-content-integration-guidelines"></a>Diretrizes de integração de conteúdo fornecidas pelo parceiro
O conteúdo para os caminhos de aprendizado do Microsoft 365 é orientado por um conjunto de arquivos JSON que atuam como manifestos de conteúdo para seu pacote de aprendizado. Há três arquivos: Metadata. JSON, playlists. JSON e assets. JSON. Esses arquivos precisam ser estruturados para corresponder aos modelos que a Web Part reconhece e, em seguida, hospedado de uma CDN (rede de distribuição de conteúdo) para permitir que a Web Part seja carregada. A Microsoft fornecerá modelos de início desses arquivos para começar.  

**Isenção de responsabilidade:** a estrutura de arquivos JSON está sujeita a alterações com base no trabalho da solução futura. O programa de adoção antecipada (EAP) do Microsoft 365 Learning Precursors será informado sobre qualquer alteração iminente dessa natureza. Junto com qualquer compatibilidade com versões anteriores do cliente e/ou diretrizes de transição. 

### <a name="download-the-microsoft-365-learning-pathways-solution"></a>Baixar a solução de cursores de aprendizagem da Microsoft 365
Você pode baixar a solução de cursores de aprendizado da Microsoft 365, junto com os arquivos JSON, do repositório https://github.com/pnp/custom-learning-office-365do github:. Observe que, no momento, a Microsoft não está executando a solicitação pull do GitHub na solução. Mas você pode usar os arquivos do GitHub como um ponto de partida para a criação de seu próprio pacote de conteúdo personalizado. 

### <a name="metadatajson-structure"></a>Estrutura Metadata. JSON
Você pode pensar nesse arquivo como o cérebro dos menus e da estrutura. Ele contém toda a estrutura de navegação, além de selecionar listas para dados nos outros dois arquivos. 


|              Nome        |                     Descrição                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|**Tecnologias**              |O conteúdo é marcado e pode ser ocultado com base na tecnologia que é atribuída.                 |  
|&nbsp;&nbsp;ID                |GUID que representa a tecnologia                                                           |  
|&nbsp;&nbsp;Tdomínio              |Nome para exibição da tecnologia                                                             |
|&nbsp;&nbsp;*Subjects []*     |Uma matriz de assuntos que são um subconjunto da tecnologia                                   | 
|&nbsp;&nbsp;&nbsp;&nbsp;ID    |GUID que representa o assunto                                                              |
|&nbsp;&nbsp;&nbsp;&nbsp;Tdomínio  |Nome para exibição do assunto                                                                |
|**Categories []**             |As categorias informam a navegação da Web Part. Cada categoria representa um nível superior da navegação                                                                                                                 |
|&nbsp;&nbsp;ID                |GUID que representa a categoria/subcategoria                                                 |
|&nbsp;&nbsp;Tdomínio              |Nome para exibição da categoria/subcategoria                                                  |
|&nbsp;&nbsp;Ampliá             |URL para a imagem que deve ser exibida no UX (relativa à base de CDN)            |
|&nbsp;&nbsp;Technologyid      |O GUID da tecnologia à qual este conteúdo está relacionado (opcional – cadeia de caracteres vazia)            |
|&nbsp;&nbsp;SubjectID         |O GUID do sujeito ao qual este conteúdo está relacionado (opcional – cadeia de caracteres vazia)               |
|&nbsp;&nbsp;Originais            |Da matriz de origem, não usada especificamente em experiência de usuário diferente de os dados personalizados adicionados pelo usuário é marcado como "locatário", e a área de administração de UX não permite a edição de nada que não esteja marcado como "locatário".                           |
|&nbsp;&nbsp;*Subcategorias []*|As subcategorias são basicamente o nível de navegação do nível 2 para baixo. A estrutura é o mesmo que uma categoria apenas aninhada.          |
|**Audiências []**             |Quando as listas de reprodução associadas a uma categoria/subcategoria são várias audiências marcadas, um seletor estará disponível para mostrar as audiências disponíveis. |         
|&nbsp;&nbsp;ID                |GUID da audiência                                                                       |  
|&nbsp;&nbsp;Tdomínio              |Nome para exibição da audiência                                                               |       
|**Fontes []**               |A matriz de cadeias de caracteres que marca o conteúdo com sua fonte, não usada especificamente em experiência de usuário diferente de dados personalizados adicionados pelo usuário é marcada como "locatário", e a área de administração de UX não permite a edição de nada que não esteja marcado como "locatário".                                                   |  
|**Níveis []**               |Quando as listas de reprodução associadas a uma categoria/subcategoria são vários níveis marcados, um seletor estará disponível para mostrar os níveis disponíveis.             |  
|&nbsp;&nbsp;ID                |GUID do nível                                                                          |  
|&nbsp;&nbsp;Tdomínio              |Nome para exibição do nível                                                                  | 
|**StatusTag [ ]**           |A marca de status é para identificar o conteúdo com vários status que serão expostos no UX. Alguns desses sinalizadores serão mostrados para o consumidor e alguns apenas para o administrador.                                                   |  
|&nbsp;&nbsp;ID                |GUID do StatugTag                                                                      |  
|&nbsp;&nbsp;Tdomínio              |Nome para exibição do StatusTag                                                              | 
|**Telemetria []**            |                                                                                           |  
|&nbsp;&nbsp;AppInsightsKey    |GUID da chave do App insights que você configurou para controlar o carregamento da Web Part do visualizador. O controle pode ser desativado por um administrador para o locatário inteiro, mas as informações enviadas são usuário anônimo com a ID do locatário. Confira esta seção para obter mais informaçõeshttps://github.com/pnp/custom-learning-office-365#disabling-telemetry-collection               |  
|**Versão**                   |As informações de versão são usadas pela solução para indicar aos administradores que a Web Part atualizou e também permite que a Web Part seja AutoAtualizar conteúdo personalizado para a versão mais recente do manifesto, caso sejam feitas alterações significativas.         | 
|&nbsp;&nbsp;Manifesto          |A versão do manifesto                                               |
|&nbsp;&nbsp;ManifestMinWebPart|A versão mínima da WebPart que funciona com a versão do manifesto             |
|&nbsp;&nbsp;CurrentWebPart    |URL para a imagem que deve ser exibida no UX (relativa à base de CDN)            |
|&nbsp;&nbsp;Rederramado           |A URL do repositório onde estão as instruções de atualização da Web Part.                    |
|**Pacotes de conteúdo**             |No momento, não há suporte para pacotes de conteúdo para CDN adicionais. Os pacotes de conteúdo permitem que a Microsoft sugira outras soluções criadas pela Microsoft que podem ser provisionadas por meio do serviço de provisionamento que aproveita o M365LP para fornecer conteúdo e que se encontram no CDNs personalizado.       | 
|&nbsp;&nbsp;ID                |GUID do pacote de conteúdo/CDN                                                              |
|&nbsp;&nbsp;Tdomínio              |Nome para exibição da CDN                                                                   |
|&nbsp;&nbsp;Descrição       |Descrição a ser exibida na interface do usuário para adicionar um pacote de conteúdo                               |
|&nbsp;&nbsp;Ampliá             |Imagem a ser exibida na interface do usuário para adicionar um pacote de conteúdo                                     |
|&nbsp;&nbsp;ProvisionURL      |A URL do pacote de serviço de provisionamento para criar o conjunto de sites do pacote de conteúdo  |
|&nbsp;&nbsp;CDNbase           |A URL base para os manifestos do pacote de conteúdo                                       |
|AssetOrigins                  |Uma matriz de origem da URL utilizada no arquivo assets. JSON descrito mais tarde. Se a URL de origem oferecer suporte, uma mensagem de postagem será enviada para help_getClientHeight. Uma resposta na propriedade data de: "help_getClientHeight = {altura de conteúdo}" (por exemplo, "help_getClientHeight = 5769") permitirá que o iFrame seja redimensionado para a altura apropriada do conteúdo enquadrado.         |

### <a name="playlistsjson-structure"></a>Estrutura de listas de reprodução. JSON
playlists. JSON – o manifesto de playlists é uma matriz de objetos que descrevem os metadados sobre uma lista de reprodução e os ativos incluídos na lista de reprodução.

|              Nome        |                     Descrição                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|Id                            |GUID que representa a lista de reprodução                                                             |  
|Título                         |Nome de exibição da lista de reprodução                                                               |
|Image                         |URL relativa (de CDN) para uma imagem para visualizar a lista de reprodução                              |                      
|Levelid                       |Nível associado                                                                           |
|AudienceID                   |Público associado                                                                        |
|Technologyid                 |Tecnologia associada                                                                      |
|SubjectID                    |Nome para exibição da categoria/subcategoria                                                  |
|Origem                        |A partir da matriz de origem, não usada especificamente no UX diferente dos dados personalizados adicionados pelo usuário está marcado como "locatário", e a área de administração de UX não permite a edição de nada que não esteja marcado como "locatário".                                              |
|CatId                         |A ID de categoria ou de subcategoria que representa o contêiner em que a playlist deve ser mostrada. No momento, o manifesto não oferece suporte à seleção de uma categoria ou subcategoria como o contêiner, caso também tenha filhos de subcategorias.        |
|Descrição                   |Uma descrição mostrada para cada lista de reprodução no UX                                           |
|StatusTagId                   |Marca de status associada                                                                      |
|StatusNote                    |Observações sobre o conteúdo exibido para administradores                                            |
|*Ativos []*                        |Uma matriz de GUIDs para os ativos que fazem parte desta playlist, em ordem de exibição.        |         

### <a name="assetjson-structure"></a>Estrutura de ativos. JSON
playlists. JSON – o manifesto de playlists é uma matriz de objetos que descrevem os metadados sobre uma lista de reprodução e os ativos incluídos na lista de reprodução.

|              Nome        |                     Descrição                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|Id                            |GUID que representa a lista de reprodução                                                             |  
|Título                         |Nome de exibição da lista de reprodução                                                               |
|Descrição                   |---                                                                                           |                      
|URL                           |A URL de origem do ativo a ser aplicada ao iFrame                                  |
|Technologyid                  |Tecnologia associada                                                                      |
|SubjectID                     |Assunto associado                                                                         |
|Origem                        |Nome para exibição da categoria/subcategoria                                                  |
|StatusTagId                   |Marca de status associada                                                                      |
|StatusNote                    |Observações sobre o conteúdo exibido para administradores.                                           |

### <a name="caching"></a>PMK
A versão atual da Web Part do visualizador utiliza uma versão em cache dos arquivos de manifesto por 24 horas. Após 24 horas, o primeiro usuário que acertar a Web Part leva o impacto de desempenho para atualizar o cache baixando os manifestos da CDN de origem e mesclar essas informações com tecnologias e listas de reprodução ocultas, bem como mesclar em subcategorias personalizadas, listas de reprodução e ativos. Como alternativa, a Web Part de administração sempre baixa o conteúdo dos manifestos e o mescla e atualiza o cache.  Portanto, em outras palavras, o administrador pode forçar uma atualização de cache a qualquer momento carregando a Web Part de administração, não se referindo à página de administração.

## <a name="content-pack-guidelines"></a>Diretrizes de pacote de conteúdo
O recurso de pacote de conteúdo desbloqueia os seguintes cenários:
- A capacidade de os parceiros redistribuirem o conteúdo de aprendizado personalizado de valor agregado personalizado sob medida para o ambiente do cliente
- A capacidade para organizações com uma equipe de treinamento forte e suporte de ti para criar conteúdo de aprendizado personalizado direcionado a seus próprios sistemas internos e governança
- A capacidade para a Microsoft de fornecer outros caminhos de aprendizado no futuro que os clientes podem optar por

Este conjunto de documentação atual é direcionado intencionalmente para parceiros devido à complexidade do recurso. A equipe de serviço está trabalhando ativamente para melhorar o suporte e permitir o #2 de cenário no futuro. 

### <a name="how-content-packs-work"></a>Como os pacotes de conteúdo funcionam
A Microsoft utiliza páginas do GitHub como uma fonte de rede de distribuição de conteúdo (CDN) para seus arquivos de manifesto e imagens. Temos uma pasta docs na raiz do nosso repositório do GitHub que inclui subpastas para cada versão dos arquivos de manifesto. Dentro de cada pasta há três arquivos de manifesto, mais uma pasta de imagens para armazenar todas as imagens de categoria, subcategoria e lista de reprodução. 

É importante que você mantenha a mesma estrutura de controle de versão que a Microsoft deve optar por estender a solução de cursores de aprendizado com seu próprio pacote de conteúdo. O ponto de extremidade da CDN não deve incluir a pasta da versão, pois a versão do manifesto à qual a Web Part oferece suporte é Baked nela e é automaticamente acrescentada à URL da CDN. Obviamente, forneceremos tempo para criar novas instâncias de seus arquivos de manifesto sempre que o revisarmos.

![CG-Part-JSON-Folder. png](media/cg-part-json-folder.png) 

Para obter mais informações sobre como usar páginas do GitHub como sua fonte de CDN, confira a [https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages](https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages)seguinte documentação da ajuda:.

A solução da Microsoft faz com que as informações sobre os ativos sejam abertas para o público, já que não há nenhuma segurança sobre quem tem acesso a esses arquivos. Acreditamos que deve haver uma camada de conteúdo livre para um consumidor, que diz que se você precisa de pagamento de parede para alguns ou todos os seus conteúdos, precisará implementar isso de forma diferente nas limitações técnicas da solução e usar as páginas do GitHub é de nenhuma média s um requisito. Qualquer provedor de CDN que você gostaria de usar é bom se você mantiver a estrutura de numeração de versão que descrevemos. Conforme mencionado anteriormente, a versão da estrutura do manifesto à qual a Web Part oferece suporte é Baked no código e é automaticamente acrescentada à URL da CDN. 

### <a name="content-pack-integration-guidance"></a>Orientação de integração do pacote de conteúdo 
As Web Parts do administrador e do visualizador foram estendidas para permitir que o consumidor configure pontos de extremidade adicionais da CDN em seu locatário, que permitirá que a Web Part do visualizador selecione qual CDN eles devem originar os dados que eles exibem. 

Principais enquadramento para ter em mente este recurso: 
- Isso é o principal aplicável para cenários de redistribuição de parceiros – onde a configuração manual de playlist é muito complicada 
- Pacotes de conteúdo personalizados são um recurso avançado e devem ser usados apenas por parceiros com experiência de administração de conteúdo da Web. Fontes de conteúdo não confiáveis podem apresentar conteúdo não seguro em seu site. Você só deve adicionar fontes confiáveis.

> **Importante** Antes de adicionar um pacote de conteúdo personalizado, você deve ter provisionado os caminhos de aprendizado do Microsoft 365 3,0 ou posterior. Para o informataion sobre o provisionamento de caminhos de aprendizado do Microsoft 365, confira [provisionar os caminhos de aprendizado da microsoft 365](https://docs.microsoft.com/en-us/office365/customlearning/custom_provision).

### <a name="content-whitelisting"></a>Lista de conteúdo
Como um parceiro, você é responsável por ajudar seus clientes a garantir que seu conteúdo seja whitelist em seu ambiente. Sugerimos que você crie um cenário de teste em seu ambiente para validar que seu conteúdo pode ser iFrame em uma página do SharePoint dentro do firewall. Siga as instruções para [criar páginas do SharePoint de listas de reprodução personalizadas](https://docs.microsoft.com/en-us/office365/customlearning/custom_createnewpage) para confirmar se esse é o caso.

### <a name="add-a-content-pack-to-learning-pathways"></a>Adicionar um pacote de conteúdo aos caminhos de aprendizado
Depois que você tiver criado modificado o JSON e definido sua CDN, poderá adicionar o pacote de contato aos caminhos de aprendizado. 

1. Na **Home** Page do site de cursores de aprendizado, aponte para **página inicial** e clique em **Administração de caminhos de aprendizado**. 
2. Na página **Administração** , clique em **... Adicione o pacote de conteúdo** no canto superior direito da página.
3. Clique em pacote de conteúdo personalizado e insira um nome para o pacote de conteúdo e, em seguida, especifique a CDN onde os arquivos JSON estão localizados.

![CG-Part-addconpack. png](media/cg-part-addconpack.png)

4. Clique em **Salvar**. O conteúdo do seu pacote de conteúdo personalizado agora deve aparecer na página de administração. Veja um exemplo. 

![CG-Part-addconpackex. png](media/cg-part-addconpackex.png)

### <a name="filter-to-the-content-pack-in-the-web-part"></a>Filtrar para o pacote de conteúdo na Web Part
Com os caminhos de aprendizado, você pode adicionar a Web Part de cursores de aprendizado à página, filtrar a Web Part para apontar para a fonte do pacote de conteúdo personalizado e, em seguida, filtrar a Web Part para a categoria, a subcategoria, a lista de reprodução e o ativo que você deseja. 

1. No site de cursores de aprendizado, clique em **novo**e em **página**.
2. Clique em **em branco**e, em seguida, **crie página**.
3. Dê um nome à página. 
4. Clique em **+ Adicionar uma nova seção** no lado esquerdo da página.
5. Clique **+** na parte superior central da nova seção e, em seguida, adicione a Web Part **caminhos de aprendizado da Microsoft 365** .
6. Clique na Web Part e, em seguida, clique no ícone **Editar** .
7. Na caixa **selecionar a fonte de aprendizado** , selecione seu pacote de conteúdo personalizado e, em seguida, filtre a Web Part para o conteúdo desejado. Veja a seguir um exemplo da Web Part filtrada para uma lista de reprodução de um pacote de conteúdo personalizado.

![CG-Part-conpackfilter. png](media/cg-part-conpackfilter.png)  




