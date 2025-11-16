# Projeto Linha Aérea

## Cenário de Negócio / Concepção

### Problema ou oportunidade percebida
Atualmente, as passagens aéreas da empresa só podem ser adquiridas por meio de atendimento telefônico ou diretamente nos guichês localizados nos aeroportos. Esse processo limita o alcance de vendas, reduz a conveniência para os clientes e gera filas e sobrecarga no atendimento presencial.

### Razão ou justificativa para esta demanda
Com o crescimento do uso de plataformas digitais para compra de passagens, tornou-se essencial oferecer uma alternativa online que seja acessível, rápida e segura. A digitalização do processo de venda busca atender à demanda por comodidade, ampliar o público-alvo e aumentar a competitividade da companhia aérea no mercado.

### Descrição sucinta do produto de software
Será desenvolvido um site de vendas de passagens aéreas, permitindo que usuários consultem horários, destinos e preços, realizem reservas e efetuem o pagamento diretamente pela plataforma. O sistema também contará com funcionalidades de cadastro de usuários, gerenciamento de voos e emissão de bilhetes eletrônicos.

### Clientes, usuários e demais envolvidos/impactados com o produto
- **Clientes**: Passageiros que desejam adquirir passagens de forma online.
- **Usuários**: Clientes finais, equipe de atendimento, equipe de TI e administradores da companhia aérea.
- **Envolvidos/Impactados**: Setores operacionais da empresa, suporte técnico, equipe de marketing, além de parceiros e integradores de meios de pagamento.

### Principais critérios de qualidade para o produto
- **Usabilidade**: Interface intuitiva e fácil de navegar para todos os perfis de usuários.
- **Disponibilidade**: Sistema acessível 24/7, com alta taxa de uptime.
- **Segurança**: Proteção de dados dos usuários e das transações financeiras.
- **Desempenho**: Tempo de resposta rápido, mesmo com alto volume de acessos.
- **Escalabilidade**: Capacidade de suportar o crescimento da base de usuários e voos ofertados.

### Casos de Uso

<img width="1680" height="2860" alt="Blank diagram" src="https://github.com/user-attachments/assets/65f1f4f2-c366-438c-a906-df90b07170c8" />

### Casos de Uso Resumidos por Ator
---------------

### Usuário

<img width="1607" height="414" alt="image" src="https://github.com/user-attachments/assets/269577de-92d5-4d84-a351-869a93b832ca" />


### Funcionário

<img width="1533" height="256" alt="image" src="https://github.com/user-attachments/assets/d558def5-f2e9-48df-b120-54e5c777ce55" />


### Central de Pagamentos

<img width="1593" height="155" alt="image" src="https://github.com/user-attachments/assets/7a94a4f7-6f4c-40a8-bc52-b9b6039ac7f3" />

--------------------------

### Caso de Uso Crítico

<img width="661" height="227" alt="image" src="https://github.com/user-attachments/assets/3985ecee-aa97-4b11-a0f9-d681e7d4a2f4" />

<img width="665" height="258" alt="image" src="https://github.com/user-attachments/assets/ef2d2734-25f0-4967-ba8a-c054fc5bf5b4" />

<img width="632" height="104" alt="image" src="https://github.com/user-attachments/assets/502e8f36-8d1d-4a09-9f51-43f41f8f149a" />

<img width="580" height="101" alt="image" src="https://github.com/user-attachments/assets/08c17b71-43a0-45eb-aa1f-b6494a998a52" />

<img width="529" height="101" alt="image" src="https://github.com/user-attachments/assets/e77ae0a7-4959-4f07-ac74-f7e1494cbf77" />

-----------------
### Diagrama de Dominio
### Explicação do Processo de Modelagem de Domínio

A modelagem de domínio do projeto foi conduzida por meio de um processo iterativo, evoluindo de um entendimento inicial do negócio para um modelo mais detalhado e preciso. Utilizamos o Diagrama de Classe, uma das formas de representação da UML (Linguagem de Modelagem Unificada), para estruturar visualmente as entidades e suas relações.

O processo pode ser descrito em três etapas principais:

1. Identificação das Entidades e Padrões de Análise
A fase inicial consistiu em identificar os principais substantivos do negócio, que representam as entidades do nosso domínio. A partir dos requisitos do sistema, definimos classes como Cliente, Voo, Passagens, Pedido e Atendente.

Neste ponto, o diagrama ainda continha elementos que descreviam ações do sistema (verbos), como "Pesquisar Voos". Para alinhar o modelo com o padrão de um diagrama de domínio, que foca nas entidades, essas classes foram removidas na etapa seguinte, simplificando a representação.

2. Detalhamento e Modificações
Com as entidades principais já definidas, o foco se voltou para o aprimoramento do diagrama. Adicionamos os atributos essenciais a cada classe, como data e numero para o Voo, e nome e email para a Conta. Essa modificação foi crucial para dar mais substância ao modelo, especificando as informações que cada entidade deveria conter.

3. Definição de Relacionamentos e Restrições
A etapa final foi a de definir como as entidades interagem entre si. Para isso, estabelecemos os relacionamentos e suas cardinalidades. Por exemplo:

A relação entre Voo e Passagens foi definida com a cardinalidade 1..*, indicando que um Voo pode ter muitas Passagens.

A conexão entre Cliente e Passagens também foi marcada com 1..*, mostrando que um Cliente pode adquirir várias Passagens.

Em outros casos, como a relação entre Passagens e Pedido, a cardinalidade 1..* reforçou que um único Pedido pode conter muitas Passagens.

Esse processo incremental nos permitiu construir um modelo de domínio robusto, que não apenas mapeia as entidades do nosso sistema, mas também ilustra as regras de negócio de forma clara e visual.

<img width="3889" height="1973" alt="Blank diagram (1)" src="https://github.com/user-attachments/assets/e83e8e7d-21aa-4ec9-bdab-f37d4b73a7a3" />

-------------------------------

### Prototipagem

### Pagina inicial com as passagens

Principais Elementos e Objetivos
Barra de Navegação Superior: Permite ao usuário alternar entre as seções principais do site, como Passagens, Pacotes e Destinos, além de acessar as configurações e o perfil.

Barra de Busca e Filtros: A área central para iniciar uma nova busca de passagens, com campos para texto (origem/destino) e data.

Filtros Laterais: Localizados à esquerda, oferecem ferramentas para refinar a pesquisa, permitindo ao usuário ajustar o preço e outras opções como a escolha de assento.

Lista de Passagens Encontradas: Exibe de forma clara os resultados da busca, mostrando as passagens disponíveis com informações básicas em cada item.

Controles de Navegação (Paginação): Na parte inferior da tela, os botões Previous, Next e os números de página permitem navegar facilmente por todos os resultados.

Botões de Ação Flutuantes: No canto inferior direito, os botões de compartilhar e de chat oferecem ao usuário opções de interação e suporte durante a navegação.

<img width="987" height="650" alt="image" src="https://github.com/user-attachments/assets/621c1259-10f2-4a86-ac23-83fa1c852638" />

---------------------------------------------

### Pagina Seleção de Passagem

Principais Elementos e Objetivos
Opções de Voo (Central): Exibe os detalhes do voo de ida (Voo Ida) e permite que o usuário escolha a classe. As duas opções mostradas são Econômica e Executiva, cada uma com seu preço e uma lista de benefícios. O objetivo é permitir que o usuário selecione a tarifa desejada.

Formulário de Contato (Lateral Direita): Uma seção dedicada à coleta de dados do usuário. Inclui campos para Nome, Sobrenome, Email e uma Mensagem. O objetivo é permitir que o usuário forneça suas informações e, possivelmente, entre em contato ou finalize a compra.

Barra de Navegação Superior: Mantém a consistência visual, permitindo ao usuário navegar entre as seções Passagens, Pacotes e Destinos, além de acessar as configurações e seu perfil.

Botões de Ação Flutuantes: Na parte inferior direita, os botões de compartilhar e de chat fornecem opções de interação e suporte durante o processo.

<img width="1113" height="731" alt="image" src="https://github.com/user-attachments/assets/8b4cc437-099b-47ce-af4f-ddf2dd20bb26" />

--------------------------------------

### Pagina de Checkout

Principais Elementos e Objetivos
Resumo das Passagens (Central): Exibe de forma clara os detalhes das passagens de ida e volta que o usuário selecionou. Cada resumo possui um layout padrão com título e subtítulo, além de botões para remover ou editar a seleção. O objetivo é permitir que o usuário revise sua escolha antes de prosseguir com o pagamento.

Dados de Pagamento (Lateral Direita): Nesta seção, o usuário insere suas informações de pagamento em campos de entrada genéricos. O objetivo é coletar os dados necessários para processar a transação.

Valor Total: Um painel destacado mostra o valor final da compra, R$ 564,45, dando ao usuário a informação exata do custo total.

Botões de Ação: O usuário pode cancelar a transação ou finalizar a compra. O botão "Finalizar" é o principal, pois leva o usuário à conclusão do processo de checkout.

Barra de Navegação Superior: Permite a navegação para outras seções do site, como Passagens, Pacotes e Destinos.

Botões de Ação Flutuantes: No canto inferior direito, os botões de compartilhar e chat fornecem opções de suporte e interação, permanecendo visíveis ao longo do processo de compra.

<img width="940" height="622" alt="image" src="https://github.com/user-attachments/assets/867a682a-f7d9-4354-87b2-49d7df942b58" />

--------------------------------

# Especificação Suplementar

## Histórico de Revisões

| Versão | Data       | Descrição                                                                                                                | Autor |
| :----- | :--------- | :----------------------------------------------------------------------------------------------------------------------- | :---- |
| 1.1    | 27/10/2025 | Criação da estrutura inicial do documento na Wiki, definindo as seções principais conforme solicitado na tarefa do TG3. | Marco |
| 1.2    | 29/10/2025 | Adição da seção "Funcional", com a listagem e descrição detalhada de todos os casos de uso extraídos dos diagramas.   | Marco |
| 1.3    | 31/10/2025 | Preenchimento das seções de Requisitos Não Funcionais (Segurança, Usabilidade, Confiabilidade e Desempenho).               | Marco |
| 1.4    | 02/11/2025 | Revisão final do documento completo. Adição da seção "Regras de Negócio" com base no Diagrama de Domínio e pequenos ajustes de formatação. | Marco |

## Introdução

Este documento é o repositório de todos os requisitos da **Plataforma de Compra de Passagens** que não estão detalhados nos diagramas de casos de uso. Ele serve como um complemento, especificando critérios de qualidade e restrições operacionais do sistema.

## Funcional

Os requisitos funcionais do sistema, extraídos dos diagramas e divididos por ator, são:

#### Ator: Usuário
* **Pesquisar Voos Disponíveis:** Permite ao cliente consultar horários, datas, origens e destinos disponíveis.
* **Cadastrar-se na Plataforma:** Permite que um novo usuário crie uma conta no sistema.
* **Realizar Login:** Permite que um usuário autentique-se na plataforma para acessar suas informações.
* **Comprar Passagem:** Processo completo onde o cliente seleciona um voo, escolhe assentos, insere seus dados, pode optar por utilizar milhas e efetua o pagamento.
* **Consultar Passagens Compradas:** Permite ao usuário visualizar o histórico de passagens que adquiriu.
* **Cancelar Passagem:** Permite que o usuário cancele uma passagem já comprada, sujeito às regras da empresa.
* **Emitir Bilhete Eletrônico:** Após a confirmação da compra, o sistema gera e disponibiliza o bilhete eletrônico para o cliente.
* **Consultar Rotas:** Permite ao usuário consultar todas as rotas operadas pela companhia.

#### Ator: Atendente
* **Cadastrar Novas Rotas:** Permite ao atendente registrar novas rotas (origem/destino) no sistema.
* **Editar Informações do Voos:** Permite alterar informações de um voo já existente (ex: horário, status).
* **Cancelar Voos:** Permite remover um voo do sistema, o que deve acionar uma notificação para os clientes afetados.
* **Gerenciar Usuários:** Permite visualizar, editar ou remover contas de usuários do sistema. Inclui a capacidade de gerenciar as passagens associadas a eles.

#### Ator: Central de Pagamentos (Sistema Externo)
* **Processar Pagamento:** Recebe as informações de pagamento do nosso sistema e valida os dados da transação.
* **Confirmar Transação:** Envia uma confirmação (aprovada) ou recusa (negada) do pagamento de volta ao nosso sistema.

## Segurança

* Toda utilização que envolva dados pessoais ou operações de gerenciamento (área do cliente, painel do atendente) requer autenticação do usuário.
* Para o **Atendente**, operações críticas como `Cancelar Voos` e `Gerenciar Usuários` devem exigir autenticação de duplo fator para garantir a segurança dos dados.
* As senhas dos usuários devem ser armazenadas de forma criptografada, utilizando algoritmos de *hash* modernos.

## Usabilidade

#### Fatores Humanos
* O cliente será capaz de ver o que está escrito em diferentes telas (desktop e mobile). Dessa forma:
    * O texto deve ser facilmente visível e os botões facilmente clicáveis.
    * Cores associadas com formas comuns de daltonismo devem ser evitadas.
* Velocidade, facilidade e um processo isento de erros são de importância primordial no processamento de vendas, pois o comprador deseja finalizar a compra rapidamente.
* O atendente, ao gerenciar voos e usuários, deve ter uma interface clara e objetiva, que minimize a chance de erros operacionais. Alertas de confirmação para ações destrutivas (como cancelar um voo) são obrigatórios.

## Confiabilidade

#### Facilidade de recuperação
* Se ocorrer uma falha na comunicação com a **Central de Pagamentos**, o sistema não deve perder os dados da sessão do cliente. Deve ser exibida uma mensagem de erro clara, permitindo que o usuário tente o pagamento novamente sem precisar preencher todas as informações do zero.

## Desempenho
* Conforme mencionado nos fatores humanos, os compradores querem completar uma venda rapidamente. Um gargalo em potencial é a autorização externa de pagamento. Nosso objetivo é obter uma autorização em **menos de 10 segundos**, em 90% das vezes.
* A consulta de voos deve retornar os resultados em **menos de 4 segundos**, mesmo em períodos de alta demanda.

## Regras de Negócio (Inferidas do Diagrama de Domínio)

* Cada **Passagem** emitida deve estar vinculada a um **Pedido** e a um **Cliente** específico.
* Um **Pedido** deve estar associado a um ou mais **Voos**.
* Um **Atendente** é o ator responsável por gerenciar os dados de **Voos**, **Rotas** e **Usuários**.
* Toda transação de compra que gera um **Pedido** deve ser processada e validada pela **Central de Pagamentos**.
-----------------------------------------
# Diagrama de Sequência
<img width="1453" height="994" alt="Diagrama" src="https://github.com/user-attachments/assets/08b042b0-6cfd-4be3-a796-c039a4d89bac" />

## Análise do Design com Padrões GRASP

A arquitetura de software para o caso de uso "Comprar Passagem", ilustrada no diagrama de sequência, foi desenvolvida com base nos padrões GRASP (General Responsibility Assignment Software Patterns). A aplicação desses padrões visa a criação de um design com baixo acoplamento, alta coesão e maior manutenibilidade.

A seguir, descrevemos os padrões aplicados e a justificativa técnica para suas utilizações.

### 1. Padrão: Controlador (Controller)

* **Princípio Fundamental:** Atribuir a responsabilidade de lidar com eventos da interface do usuário a uma classe intermediária, que não faz parte da camada de apresentação, mas representa o sistema ou um cenário de caso de uso.

* **Aplicação no Projeto:** Foi implementada a classe `ControladorPedido`. No diagrama, a `TelaSelecaoPassagem` não contém a lógica de negócio para a compra. Em vez disso, ela delega a responsabilidade ao `ControladorPedido` através da chamada `iniciarCompra()`. O controlador, por sua vez, coordena as interações subsequentes com as classes de domínio (`Pedido`) e sistemas externos (`CentralPagamentos`).

* **Justificativa da Utilização:**
    * **Baixo Acoplamento:** Esta abordagem dissocia a camada de apresentação (UI) da lógica de negócio. Modificações na interface não impactam as regras de como uma compra é processada, e vice-versa.
    * **Alta Coesão e Reutilização:** O `ControladorPedido` se torna uma classe coesa, com a única responsabilidade de orquestrar o processo de compra. Essa lógica centralizada pode ser reutilizada por diferentes interfaces no futuro (ex: um aplicativo mobile), sem duplicação de código.

### 2. Padrão: Criador (Creator)

* **Princípio Fundamental:** Atribuir a responsabilidade de criar um objeto (Classe B) a outra classe (Classe A) se a Classe A agrega, contém ou possui uma forte associação com os objetos da Classe B.

* **Aplicação no Projeto:**
    * A classe `ControladorPedido` foi designada para criar instâncias de `Pedido`, pois é ela quem recebe os dados iniciais do usuário necessários para a criação do pedido.
    * A classe `Pedido` é responsável por criar as instâncias de `Passagem`, pois um pedido conceitualmente agrega ou contém um conjunto de passagens.

* **Justificativa da Utilização:**
    * **Coesão e Contexto:** A criação dos objetos ocorre no contexto em que eles fazem mais sentido. Isso mantém a lógica de negócio organizada e evita a criação de "classes fábrica" genéricas que diminuem a coesão do sistema.

### 3. Padrão: Especialista da Informação (Information Expert)

* **Princípio Fundamental:** Atribuir uma responsabilidade à classe que detém a informação necessária para cumpri-la. Este é o princípio mais basilar para a atribuição de responsabilidades em um sistema orientado a objetos.

* **Aplicação no Projeto:** A responsabilidade de calcular o valor total da compra foi atribuída à classe `Pedido`.

* **Justificativa da Utilização:**
    * **Encapsulamento e Baixo Acoplamento:** A classe `Pedido` é a única que conhece a lista completa de `Passagens` associadas a ele. Portanto, ela é a especialista com as informações necessárias para realizar o cálculo. Atribuir essa responsabilidade a outra classe (como o `ControladorPedido`) exigiria que o `Pedido` expusesse sua estrutura interna, violando o encapsulamento e aumentando o acoplamento entre as classes.


----------------------------------------------------------

# Diagrana de Componentes

O diagrama de componentes abaixo foca na estrutura modular do sistema, mostrando as dependências e as interfaces de comunicação entre os blocos.

## Diagrama

O diagrama a seguir divide o sistema em quatro componentes principais, mostrando como o `Frontend` (interface do usuário) se comunica com o `Servidor API` para acessar o `Banco de Dados` e o `Sistema de Pagamentos Externo`.

<img width="886" height="235" alt="diagrama de componentes" src="https://github.com/user-attachments/assets/cf1ca90d-4c6b-4eb3-9cbc-026bf9453740" />

## Descrição dos Componentes e Conexões

Abaixo detalhamos o papel de cada componente e a justificativa para suas conexões, conforme ilustrado no diagrama.

### 1. Componentes Principais

* **[WebApp (Frontend)]:** É o componente de apresentação, responsável por toda a interface gráfica que roda no navegador do usuário (cliente). Ele é feito com tecnologias web (HTML, CSS, JavaScript) e é responsável por exibir os voos e capturar os dados do usuário.
* **[Servidor API (Backend)]:** Este é o "cérebro" do sistema. É onde toda a lógica de negócio (definida nos padrões GRASP do TG4) reside. Ele expõe as funcionalidades do sistema de forma segura através de "Interfaces" (APIs).
* **[Banco de Dados (MySQL)]:** É o componente responsável pela persistência dos dados. Armazena todas as informações vitais, como o cadastro de usuários, voos, rotas, pedidos e passagens.
* **[Sistema de Pagamentos (Externo)]:** É um componente de terceiros, fora do nosso controle. Ele é especializado e seguro para processar transações financeiras (ex: dados de cartão de crédito).

### 2. Justificativa das Conexões (Dependências)

O motivo de cada linha no diagrama é explicado abaixo:

* **Frontend `..>` API (de Voos e Pedidos):**
    * **Descrição:** O Frontend *depende* das interfaces `API de Voos` e `API de Pedidos` que são providas pelo Servidor API.
    * **Motivo:** A interface web (Frontend) não contém lógica de negócio nem tem acesso direto aos dados. Para exibir os voos, ela precisa *consultar* a `API de Voos`. Para realizar uma compra, ela precisa *enviar* os dados para a `API de Pedidos`. Esta separação é a base da arquitetura web moderna, garantindo segurança e flexibilidade.

* **Servidor API `..>` Banco de Dados:**
    * **Descrição:** O Servidor API *depende* do Banco de Dados.
    * **Motivo:** O servidor precisa de um local para armazenar e recuperar informações de forma permanente. Quando o Frontend pede a lista de voos, a API busca essa informação no Banco de Dados. Quando uma compra é aprovada, a API *salva* os dados desse pedido no Banco de Dados.

* **Servidor API `..>` Sistema de Pagamentos:**
    * **Descrição:** O Servidor API *depende* do Sistema de Pagamentos Externo.
    * **Motivo:** Nosso sistema não deve (e por regras de segurança, não pode) processar ou armazenar dados sensíveis de cartão de crédito. Quando o usuário finaliza a compra, a API *delega* a responsabilidade da transação financeira para este sistema externo, que é especialista nisso. A API apenas envia o valor e aguarda uma resposta de "aprovado" ou "recusado".









