---
author: pkrebs
ms.author: pkrebs
title: Modelos de integração de parceiros
ms.date: 3/9/2019
description: Modelos de integração de parceiros
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: a91cdf4ee6aa3bbc22033dd484605ea5405b3c4c
ms.sourcegitcommit: 33acfc2149de89e8375b064b2223cae505d2a102
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52575986"
---
# <a name="partner-integration-models"></a>Modelos de integração de parceiros
Embora não seja possível complementar o conteúdo dos caminhos de aprendizado do Microsoft 365 diretamente 'fora da caixa' do serviço de Provisionamento Online do SharePoint, há vários modelos de integração que os parceiros podem aproveitar para criar ofertas de serviço de adereço de valor alinhadas. Os modelos de integração de parceiros acima são apresentados em ordem de complexidade crescente e níveis de investimento. Portanto, nossas diretrizes são criar sua experiência e se formar para níveis mais avançados com base em seus modelos de negócios.

![Flow gráfico mostra a função de habilitadores, integradores e redistibutores.](media/cg-part-intmodel.png)

## <a name="how-should-i-get-started"></a>Como devo começar? 
Para começar, aqui estão algumas práticas recomendadas a seguir.     

### <a name="1-begin-with-building-expertise-as-an-enabler"></a>1. Comece com a experiência de criação como um Habilitador. 
Você pode ajudar uma porcentagem da sua base de clientes imediatamente habilitando seu portal de treinamento de caminhos de aprendizagem e realizando a curadoria de conteúdo direcionada da Microsoft. Para obter instruções sobre como provisionar caminhos de aprendizado, consulte [Provisionar uma nova solução de caminhos de aprendizado.](/office365/customlearning/custom_provision)  

### <a name="2-then-extend-your-services-as-an-integrator"></a>2. Em seguida, estenda seus serviços como um Integrador
Execute um retorno de automação na análise de investimento , dependendo da quantidade de suas necessidades de integração de conteúdo e/ou serviços. Por exemplo, pode não fazer sentido assumir os custos operacionais e de desenvolvimento em relação às nossas diretrizes de integração de conteúdo se você puder criar manualmente rapidamente uma lista de reprodução personalizada direcionada apontando para o conteúdo pago ou referenciar seus serviços.

### <a name="3-when-the-return-on-investment-makes-sense--consider-redistribution"></a>3. Quando o retorno sobre o investimento faz sentido – considere Redistribuição 
Quando o retorno sobre o investimento faz sentido – considere Redistribuição (ou trabalhar com parceiros de caminhos de aprendizado relacionados) para criar soluções reembaladas. Eles se baseiam na estrutura padrões e práticas SharePoint que fornece soluções para extrair sites personalizados e implantar em ambientes de clientes 

## <a name="partner-provided-content-integration-guidelines"></a>Diretrizes de integração de conteúdo fornecidas pelo parceiro
O conteúdo Microsoft 365 de aprendizado é orientado por um conjunto de arquivos JSON que atuam como manifestos de conteúdo para seu pacote de aprendizagem. Há três arquivos: metadata.js, playlists.jse assets.json. Esses arquivos precisam ser estruturados para corresponder aos modelos que a Web Part reconhece e hospedados de uma rede de distribuição de conteúdo (CDN) para permitir que a Web Part os carregue. A Microsoft fornecerá modelos in-locar esses arquivos para começar.  

**Aviso de isenção de responsabilidade:** a estrutura de arquivo JSON está sujeita a alterações com base no trabalho da solução futura. O Microsoft 365 de aprendizado parceiro Programa De adoção Antecipado (EAP) será informado de quaisquer alterações iminentes dessa natureza. Juntamente com qualquer orientação de compatibilidade e/ou transição do cliente. 

### <a name="download-the-microsoft-365-learning-pathways-solution"></a>Baixar a solução Microsoft 365 de aprendizado
Você pode baixar a Microsoft 365 de aprendizado, juntamente com os arquivos JSON, do repositório GitHub: https://github.com/pnp/custom-learning-office-365 . Observe que, neste momento, a Microsoft não está GitHub solicitação pull na solução. Mas você pode usar os arquivos GitHub como ponto de partida para criar seu próprio pacote de conteúdo personalizado. 

### <a name="metadatajson-structure"></a>Metadata.jsestrutura
Você pode pensar nesse arquivo como o cérebro dos menus e da estrutura. Ele contém toda a estrutura de navegação, bem como listas de opções para dados nos outros dois arquivos. 


|              Nome        |                     Descrição                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|**Tecnologias**              |O conteúdo é marcado e pode ser oculto com base na Tecnologia atribuída.                 |  
|&nbsp;&nbsp;Id                |GUID representando a tecnologia                                                           |  
|&nbsp;&nbsp;Nome              |Nome de exibição da tecnologia                                                             |
|&nbsp;&nbsp;*Subjects[ ]*     |Uma matriz de assuntos que são um subconjunto da tecnologia                                   | 
|&nbsp;&nbsp;&nbsp;&nbsp;Id    |GUID representando o assunto                                                              |
|&nbsp;&nbsp;&nbsp;&nbsp;Nome  |Nome de exibição do assunto                                                                |
|**Categorias [ ]**             |As categorias informam a navegação da webpart. Cada categoria representa um nível superior da navegação                                                                                                                 |
|&nbsp;&nbsp;Id                |GUID representando a categoria/subcategoria                                                 |
|&nbsp;&nbsp;Nome              |Nome para exibição da categoria/subcategoria                                                  |
|&nbsp;&nbsp;Image             |URL da imagem que deve ser exibida no UX (em relação à base CDN)            |
|&nbsp;&nbsp;TechnologyId      |O GUID da Tecnologia à que esse conteúdo está relacionado (opcional – cadeia de caracteres vazia)            |
|&nbsp;&nbsp;SubjectId         |O GUID do Assunto a que esse conteúdo está relacionado (opcional – cadeia de caracteres vazia)               |
|&nbsp;&nbsp;Source            |Da matriz Source, não usada especificamente no UX, além dos dados personalizados adicionados pelo usuário, é marcada como "Locatário" e a área de administração do UX não permite a edição de nada que não seja marcado como "Locatário".                           |
|&nbsp;&nbsp;*Subcategorias[ ]*|Sub-Categories são basicamente o nível de nav do nível 2 para baixo. A estrutura é a mesma que um Category apenas aninhado.          |
|**Audiências [ ]**             |Quando as listas de reprodução associadas a uma categoria/subcategoria são várias audiências marcadas, um seletor estará disponível para mostrar os públicos disponíveis. |         
|&nbsp;&nbsp;Id                |GUID da audiência                                                                       |  
|&nbsp;&nbsp;Nome              |Nome de exibição da audiência                                                               |       
|**Fontes [ ]**               |Matriz de cadeias de caracteres que marcam o conteúdo com sua origem, não especificamente usadas no UX que não os dados personalizados adicionados pelo usuário são marcados como "Locatário" e a área de administração do UX não permite a edição de nada que não seja marcado como "Locatário".                                                   |  
|**Níveis [ ]**               |Quando as listas de reprodução associadas a uma categoria/subcategoria são vários níveis marcados, um seletor estará disponível para mostrar os níveis disponíveis.             |  
|&nbsp;&nbsp;Id                |GUID do Nível                                                                          |  
|&nbsp;&nbsp;Nome              |Nome de exibição do Nível                                                                  | 
|**StatusTag [ ]**           |A marca de status é para identificar o conteúdo com vários status que serão expostos no UX. Alguns desses sinalizadores serão show para o consumidor e alguns somente para o administrador.                                                   |  
|&nbsp;&nbsp;Id                |GUID do StatugTag                                                                      |  
|&nbsp;&nbsp;Nome              |Nome de exibição da StatusTag                                                              | 
|**Telemetria [ ]**            |                                                                                           |  
|&nbsp;&nbsp;AppInsightsKey    |GUID da chave de insights do aplicativo que você definiu para acompanhar o carregamento da Web Part do visualizador. O controle pode ser desligado por um administrador para todo o locatário, mas as informações enviadas são de usuário anonimizado com a id do locatário. Confira esta seção para obter mais informações https://github.com/pnp/custom-learning-office-365#disabling-telemetry-collection               |  
|**Versão**                   |As informações de versão são usadas pela solução para indicar aos administradores que a webpart foi atualizada e também permitir que a WebPart atualize o conteúdo personalizado para a versão mais recente do manifesto se alterações significativas foram feitas.         | 
|&nbsp;&nbsp;Manifesto          |A versão do manifesto                                               |
|&nbsp;&nbsp;ManifestMinWebPart|A versão mínima da webpart que funciona com a versão do manifesto             |
|&nbsp;&nbsp;CurrentWebPart    |URL da imagem que deve ser exibida no UX (em relação à base CDN)            |
|&nbsp;&nbsp;RepoURL           |A URL do repositório onde estão as instruções de web part de atualização.                    |
|**Content Packs**             |Neste momento, não há suporte para pacotes de conteúdo CDN de outros usuários. Os pacotes de conteúdo permitem que a Microsoft sugira outras soluções criadas pela Microsoft que podem ser provisionadas por meio do serviço de Provisionamento que aproveita o M365LP para fornecer conteúdo e estão dentro e de si mesmas CDNs personalizadas.       | 
|&nbsp;&nbsp;Id                |GUID do pacote de conteúdo/CDN                                                              |
|&nbsp;&nbsp;Nome              |Nome de exibição do CDN                                                                   |
|&nbsp;&nbsp;Descrição       |Descrição a ser exibida na interface do usuário para adicionar um pacote de conteúdo                               |
|&nbsp;&nbsp;Image             |Imagem a ser exibida na interface do usuário para adicionar um pacote de conteúdo                                     |
|&nbsp;&nbsp;ProvisionURL      |A URL do pacote de serviço de provisionamento para criar o conjunto de sites do pacote de conteúdo  |
|&nbsp;&nbsp;CDNbase           |A URL base para os manifestos do pacote de conteúdo                                       |
|AssetOrigins                  |Uma matriz de origem da URL é usada no arquivo assets.json descrito posteriormente. Se a URL de origem for compatível com ela, uma mensagem de postagem será enviada para help_getClientHeight. Uma resposta na propriedade data de: "help_getClientHeight={altura do conteúdo}" (por exemplo, "help_getClientHeight=5769") permitirá que o iFrame seja resized para a altura apropriada do conteúdo emoldurado.         |

### <a name="playlistsjson-structure"></a>Playlists.jsestrutura
playlists.json – O manifesto de listas de reprodução é uma matriz de objetos que descrevem os metadados sobre uma playlist e os ativos incluídos na playlist.

|              Nome        |                     Descrição                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|Id                            |GUID representando a playlist                                                             |  
|Título                         |Nome de exibição da playlist                                                               |
|Image                         |URL relativa (de CDN) para uma imagem para visualizar a playlist                              |                      
|LevelId                       |Nível associado                                                                           |
|AudienceId                   |Audiência associada                                                                        |
|TechnologyId                 |Tecnologia associada                                                                      |
|SubjectId                    |Nome para exibição da categoria/subcategoria                                                  |
|Origem                        |Na matriz de origem, não usada especificamente no UX, além dos dados personalizados adicionados pelo usuário, ela é marcada como "Locatário" e a área de administração do UX não permite a edição de nada que não seja marcado como "Locatário".                                              |
|CatId                         |A ID Category ou SubCategory que representa o contêiner em que a playlist deve ser mostrada. Atualmente, o manifesto não dá suporte à seleção de categoria ou subcategoria como contêiner se ele também tiver filhos de SubCategoria.        |
|Descrição                   |Uma descrição mostrada para cada playlist no UX                                           |
|StatusTagId                   |Marca de status associada                                                                      |
|StatusNote                    |Observações sobre o conteúdo exibido aos administradores                                            |
|*Assets[]*                        |Uma matriz de GUID para os ativos que fazem parte dessa playlist, em ordem de exibição.        |         

### <a name="assetjson-structure"></a>Asset.jsestrutura
playlists.json – O manifesto de listas de reprodução é uma matriz de objetos que descrevem os metadados sobre uma playlist e os ativos incluídos na playlist.

|              Nome        |                     Descrição                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|Id                            |GUID representando a playlist                                                             |  
|Título                         |Nome de exibição da playlist                                                               |
|Descrição                   |---                                                                                           |                      
|URL                           |A URL de origem do ativo, a ser aplicada ao iFrame                                  |
|TechnologyId                  |Tecnologia associada                                                                      |
|SubjectId                     |Assunto associado                                                                         |
|Origem                        |Nome para exibição da categoria/subcategoria                                                  |
|StatusTagId                   |Marca de status associada                                                                      |
|StatusNote                    |Observações sobre o conteúdo exibido aos administradores.                                           |

### <a name="caching"></a>Caching
A versão atual da Web Part do visualizador utiliza uma versão em cache dos arquivos de manifesto por 24 horas. Após 24 horas, o primeiro usuário que atingiu a Webpart assume o sucesso de desempenho para atualizar o cache baixando os manifestos do CDN de origem e mesclando essas informações com tecnologias ocultas e playlists, bem como mesclando em sub-categorias, playlists e ativos personalizados. Como alternativa, a Web Part do administrador sempre baixa o conteúdo dos manifestos e os mescla e atualiza o cache.  Portanto, em outras palavras, o administrador pode forçar uma atualização de cache a qualquer momento carregando a Web Part do administrador, também conhecido como ir para a página Administração.

## <a name="content-pack-guidelines"></a>Diretrizes do Pacote de Conteúdo
O recurso Content Pack desbloqueia os seguintes cenários:
- A capacidade dos parceiros de redistribuir conteúdo personalizado de aprendizado personalizado para o ambiente dos clientes
- A capacidade de organizações com uma equipe de treinamento forte e suporte de IT para criar conteúdo de aprendizado personalizado direcionado para seus próprios sistemas internos e governança
- A capacidade da Microsoft de fornecer caminhos de aprendizado adicionais no futuro em que os clientes podem optar

Esse conjunto de documentação atual é intencionalmente direcionado para Parceiros devido à complexidade do recurso. A equipe de serviço está trabalhando ativamente para dar melhor suporte e habilitar #2 cenário, no futuro. 

### <a name="how-content-packs-work"></a>Como funcionam os Pacotes de Conteúdo
A Microsoft utiliza GitHub páginas como uma fonte Rede de Distribuição de Conteúdo (CDN) para seus arquivos de manifesto e imagens. Temos uma pasta de documentos na raiz do repositório GitHub que inclui sub pastas para cada versão dos arquivos de manifesto. Dentro de cada pasta, há três arquivos de manifesto, além de uma pasta de imagens para armazenar todas as imagens de categoria, subcategoria e playlist. 

É importante que você mantenha a mesma estrutura de controle de versão que a Microsoft deve optar por estender a solução de caminhos de aprendizado com seu próprio pacote de conteúdo. Seu CDN de extremidade não deve incluir a pasta de versão, pois a versão de manifesto suportada pela Web Part é baked nele e é automaticamente anexada à url CDN. Obviamente, você terá tempo para criar novas instâncias de seus arquivos de manifesto sempre que o revisões.

![Captura de tela mostra a estrutura de exemplo.](media/cg-part-json-folder.png) 

Para obter mais informações sobre como usar GitHub como sua fonte de CDN, consulte a documentação de ajuda a seguir: [https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages](https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages) .

A solução da Microsoft abre as informações sobre os ativos para o público, pois não há segurança em torno de quem tem acesso a esses arquivos. Acreditamos que deve haver uma camada livre de conteúdo para um consumidor, que disse que, se você precisar pagar uma parede para algum ou todo o conteúdo, será necessário implementar isso de forma diferente nas limitações técnicas da solução e o uso de páginas GitHub não é de forma alguma um requisito. Qualquer CDN provedor que você gostaria de usar está bom se você manter a estrutura de numeração de versão que descrevemos. Conforme mencionado anteriormente, a versão da estrutura de manifesto suportada pela Web Part é baked no código e é automaticamente anexada à URL CDN. 

### <a name="content-pack-integration-guidance"></a>Diretrizes de integração do Pacote de Conteúdo 
As Web Parts do administrador e do visualizador foram estendidas para permitir que o consumidor configure pontos de extremidade de CDN adicionais em seu locatário, o que permitirá que a Web Part do visualizador selecione qual CDN eles devem origem dos dados exibidos. 

Enquadramento de chave para ter em mente esse recurso: 
- Isso é aplicável principal para cenários de redistribuição de parceiros – em que a configuração manual de playlist é muito complicada 
- Os Pacotes de Conteúdo Personalizados são um recurso avançado e devem ser usados apenas por parceiros com experiência para administrar conteúdo da Web. Fontes de conteúdo não confiáveis podem introduzir conteúdo não seguro em seu site. Você só deve adicionar fontes em que você confia.

> **IMPORTANTE** Antes de adicionar um Pacote de Conteúdo Personalizado, você deve ter provisionado Microsoft 365 de aprendizado 3.0 ou posterior. Para informações sobre o provisionamento de Microsoft 365 de aprendizagem, consulte [Provision Microsoft 365 learning pathways](./custom_provision.md).

### <a name="content-whitelisting"></a>Whitelisting de conteúdo
Como parceiro, é sua responsabilidade ajudar seus consumidores a garantir que seu conteúdo seja whitelisted em seu ambiente. Sugerimos que você crie um cenário de teste em seu ambiente para validar que seu conteúdo pode ser iFrame'd em uma página SharePoint dentro do firewall. Siga as [instruções Criar SharePoint para Playlists Personalizadas](./custom_createnewpage.md) para confirmar se esse é o caso.

### <a name="add-a-content-pack-to-learning-pathways"></a>Adicionar um Pacote de Conteúdo aos Caminhos de Aprendizagem
Depois de criar o JSON modificado e definido seu CDN, você poderá adicionar o Contact Pack aos caminhos de aprendizado. 

1. Na home **page** dos caminhos de aprendizado, aponte para **Home** e clique em Administração de caminhos **de aprendizagem.** 
2. Na página **Administração,** clique em **... Adicione Content Pack** no canto superior direito da página.
3. Clique em Pacote de Conteúdo Personalizado e insira um nome do Pacote de Conteúdo e especifique o CDN onde os arquivos JSON estão localizados.

   ![Tela onde você inserir o nome e os caminhos.](media/cg-part-addconpack.png)

4. Clique em **Salvar**. O conteúdo do Pacote de Conteúdo Personalizado agora deve aparecer na página Administração. Veja um exemplo. 

   ![Exemplo de página de administração.](media/cg-part-addconpackex.png)

### <a name="filter-to-the-content-pack-in-the-web-part"></a>Filtrar para o Pacote de Conteúdo na Web Part
Com os caminhos de aprendizado, você pode adicionar a Web Part de caminhos de aprendizado a uma página, filtrar a Web Part para apontar para a fonte do Pacote de Conteúdo Personalizado e filtrar a Web Part para a categoria, subcategoria, playlist e ativo que você deseja. 

1. No site de caminhos de aprendizado, clique em **Novo** e, em seguida, **Página**.
2. Clique **em Branco** e, em seguida, Criar **Página**.
3. Dê um nome à página. 
4. Clique **em + Adicionar uma nova seção** no lado esquerdo da página.
5. Clique no meio superior da nova seção e adicione a web part de Microsoft 365 **+** **de aprendizado.**
6. Clique na Web Part e clique no **ícone Editar.**
7. Na caixa **Selecionar a Fonte de** Aprendizado, selecione seu Pacote de Conteúdo Personalizado e filtre a Web Part para o conteúdo que você deseja. O exemplo a seguir fornece um exemplo da Web Part filtrada para uma playlist de um Pacote de Conteúdo Personalizado.

   ![Captura de tela de uma Web Part de exemplo filtrada para uma playlist de um Pacote de Conteúdo Personalizado.](media/cg-part-conpackfilter.png)