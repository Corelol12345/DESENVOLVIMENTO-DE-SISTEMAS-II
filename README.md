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
<img width="987" height="650" alt="image" src="https://github.com/user-attachments/assets/621c1259-10f2-4a86-ac23-83fa1c852638" />











