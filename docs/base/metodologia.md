# <center> Metodologia

## Histórico de versão
|Data | Versão | Descrição | Autor(es)
| -- | -- | -- | -- |
| 16.02.2021 | 0.1 | Criação do documento | [Kalebe Lopes](https://github.com/KalebeLopes), [Isabella Carneiro](https://github.com/isabellacgmsa)|
| 17.02.2021 | 0.2 | Adição de alguns tópicos | [Isabella Carneiro](https://github.com/isabellacgmsa)|
| 17.02.2021 | 0.3 | Adição de alguns tópicos | [Kalebe Lopes](https://github.com/KalebeLopes)|
| 17.02.2021 | 0.4 | Adição das ferramentas | [Kalebe Lopes](https://github.com/KalebeLopes)|

### Participantes
* Isabella Carneiro
* Kalebe Lopes

## 1. Introdução
O documento de metodologia busca descrever as abordagens utilizadas durante o processo de desenvolvimento desse projeto. Nele será descrito quais metodologias foram usadas como referência, e quais métodos foram adotados para o nosso contexto. Esse documento também visa explorar como a equipe se organizou e comunicou durante o projeto.

## 2. Metodologias Ágeis
Todas as metodologias adotadas durante esse projeto tem relação com dois princípios fundamentais do desenvolvimento ágil de software.

Com base nesses princípios, foi utilizado partes de várias metodologias já conhecidas como SCRUM, Kanban e XP com o objetivo de utilizar uma metodologia que melhor adaptasse ao nosso contexto.

### 2.1. Scrum
O Scrum é um framework de gerenciamento de projetos, da organização ao desenvolvimento ágil de produtos complexos e adaptativos com o mais alto valor possível, através de várias técnicas, utilizando desde o início de 1990 e que atualmente é utilizado em mais de 60% dos projetos ágeis em todo o mundo.

Essa metodologia define várias atividades que devem ocorrer durante o processo de desenvolvimento. No nosso contexto foram adotadas as seguintes atividades: Product Backlog, Sprints, Sprint Planning, Sprint Review, Daily Meeting,

#### Sprint: 
Uma sprint é a unidade básica de desenvolvimento na metodologia Scrum. As sprints podem durar entre uma semana e um mês, e são um esforço dentro de uma faixa de tempo. Esse faixa de tempo deve ser relativamente curta para possibilitar entregas parciais do sistema, gerando valor e permitindo a avaliação dinâmica do trabalho.

No nosso contexto, foi definido que as sprints irão durar entre 7 a 10 dias.
#### Sprint Planning:
Sprint planning é um evento de planejamento onde será definido quais tarefas (no nosso caso issues) do product backlog serão feitas na próxima sprint. 

No nosso contexto, o projeto e suas entregas estão definidos no plano de ensino da disciplina. Desse modo, todas as atividade e seus prazos são conhecidas, restando somente a definição dos responsáveis pela sua realização.
Com isso em mente, é realizado reuniões nas segundas-feiras para definir quais as atividades devem ser priorizadas, com base na milestones mais próxima da data atual. Uma vez definido as atividades, é definido os responsáveis e a data de término da sprint.

#### Daily Meeting:
Na metodologia Scrum é recomendado que se realize reuninões de status do projeto diariamente, sendo essa reunião conhecida como daily meeting. Essa reunião é sempre realizada em um mesmo horário e deve durar no máximo 15 minutos. O objetivo é deixar todos os integrantes cientes do trabalho um do outro, desse modo cada participante deve responder três perguntas:

O que você tem feito da daily passada para a daily atual?
O que você está planejando fazer da daily atual para a daily de amanhã?
Você tem algum problema impedindo você de realizar sua atividade?

No contexto do nosso trabalho, será realizado por um grupo separado do Telegram unicamente para as dailys, de modo que fique organizada a conversa.

#### Product Backlog: 
Product backlog é um dos artefatos descritos pelo SCRUM. Esse artefato é uma lista dinâmica de requisitos do projeto, ou seja, são as atividades e limitações que o projeto deve realizar ou está sujeito para que seja bem sucedido. 

No nosso contexto, essa lista de requisitos são as issues do nosso repositório. Essas issues são abstrações de cartões de tarefas que descrevem o que deve ser feito e as limitações como tempo e pessoas alocadas.

O único campo obrigatório na criação de uma issue é o título e a experiência dos integrantes do projeto demostrou que issues mal escritas são mal intepretadas e resultam em entregas de baixa qualidade.

Visando padronizar a criação de issues no nosso projeto, foi criado um template de criação onde é preciso definir outros campos. Esses campos são: Descrição, Critérios de aceitação e tarefas.

Na descrição irá descrever a atividade da issue, inserindo informações necessárias para o entendimento. Nesse campo deve ser evitado descrições genéricas e ambíguas.

Nos critérios de aceitação deve descrever quais serão os indicadores usados para verificar a qualidade do trabalho entregue. 
#### Sprint Review:
Sprint Review é um evento de validação e verificação que ocorre antes do Sprint planning. Durante esse evento é analisado as entregas da sprint anterior e sua qualidade. Após essa análise a atividade pode ser concluída ou pode voltar para o product backlog, associada com um pedido de correção. Durante esse evento também é discutido dificuldades enfrentadas e pontos de melhoria para a próxima sprint.

No nosso contexto, os sprints review ocorrem em duas etapas. A etapa de validação e verificação ocorre durante a sprint, sempre que um pull request é criado. Pull request é a abstração da entrega de uma atividade. As atividades são realizadas em um ambiente individual de desenvolvimento, esse ambiente é um clone do ambiente original onde fica as atividades entregues, esse ambiente é conhecido por branches. Sempre uma atividade é concluída em seu ambiente clone, é criado um pull request, isso é, um pedido para que as alterações criadas no ambiente clone vá para o ambiente original. É nessa etapa que ocorre a validação e verificação. Antes do pull request ser aceito é revisionado a atividade.

A segunda etapa ocorre antes da sprint review, onde é discutido as dificuldades enfrentadas e as sugestões de melhoria para a próxima sprint.

### 2.2. KANBAN
Kanban é um quadro de cartões, sendo que cada cartão representa uma atividade, onde é controlado os fluxos em que cada cartão se encontra. Esses fluxos podem ser vários, dependendo do processo em questão, mas no geral são 3 fluxos principais: "a fazer", "fazendo" e "feito".

#### Backlog: 
É a lista que contém todas as tarefas a serem feitas para a conclusão do projeto.
#### Em andamento: 
É a "coluna" que armazena as tarefas que estão em andamento. No nosso contexto, são as issues que estão abertas.
#### Revisão:
É a "coluna" que armazena as tarefas que estão sob revisão. No nosso contexto, é a análise dos critérios de aceitação definidos na criação das issues no momento em que um pull request é aberto.
#### Concluído:
É a "coluna" que armazena as tarefas já revisadas. No nosso contexto, são as issues na qual seus pull requerts já foram verificados e aceitos.

### 2.3. XP
Extreme Programming é uma metodologia com foco em agilidade de equipes e qualidade de projetos, apoiada em valores como simplicidade, comunicabilidade e feedback. Objetivando a execução de projetos dentro prazo e do orçamento, fazendo que o cliente fique satisfeito com os resultados sem que a equipe do projeto seja sobrecarregada. 
#### Programação em pares:
A produção do software é feita em pares, isso significa que duas pessoas focam em resolver um determinado problema. A ideia por trás dessa prática é que dois cérebros e quatro olhos são melhores que um cérebro e dois olhos. Além de possibilitar a revisão contínua do código,  a identificação de eventuais erros no momento da digitação e uma solução mais rápida aos problemas, faz com que a qualidade do código aumente e a quantidade de linhas diminua.
#### Integração Contínua:
A Integração Contínua é uma prática utilizada para construir ou integrar as etapas do desenvolvimento de um software, de modo que o código principal permaneça sem bugs ao final de cada uma das etapas. No nosso contexto, utilizamos o GitHub para fazer o versionamento do sistema e, a cada nova construção ou integração de diferentes funcionalidades, é realizada a revisão dos seus critérios de aceitação.      
#### Feedback:
O feedback constante é uma característica marcante do XP. É o processo de troca de informações que ocorre entre clientes e a equipe de desenvolvimento durante a produção de um software. O feedback rápido visa descobrir possíveis problemas prematuros e facilita a resolução dos mesmos.
#### Refatoração:
Refatorar é uma forma positiva de aumentar a usabilidade do software. Promove um design simples e torna o projeto final um produto de sucesso e qualidade. As funcionalidades do sistema devem ser refatoradas sempre que for necessário.

## 3. Ferramentas
<img src='https://user-images.githubusercontent.com/44823367/108258632-01158d00-713f-11eb-9df5-5c7262bc1dbc.jpg' style='margin-top:10px;margin-bottom:30px;'>

* **GitHub**: Utilizado para fazer a hospedagem do código-fonte e o versionamento do projeto.
* **Telegram**: Utilizado para agilizar a comunicação entre a equipe e realizar o daily meeting.  
* **Zenhub**: Utilizado para aplicarmos o método Kanban no projeto.
* **OneDrive**: Utilizado para armazenar documentos criados pelo time.
* **Balsamiq**: Utilizado para a criação do protótipo de baixa fidelidade.
* **Figma**: Utilizado para a criação do protótipo de alta fidelidade.
* **Google Meet**: Utilizado para fazer reuniões de forma remota com os integrantes da equipe.

## 4. Referências

DEVMEDIA, **Extreme Programming**. Disponível em [https://www.devmedia.com.br/extreme-programming-conceitos-e-praticas/1498]( https://www.devmedia.com.br/extreme-programming-conceitos-e-praticas/1498). Último acesso 17/02/2021.

HYYGER BLOG, **Refactoring in Extreme Programming**. Disponível em [https://hygger.io/blog/refactoring-in-extreme-programming/#:~:text=Refactoring%20is%20especially%20necessary%20in,fast%20as%20it%20is%20possible](https://hygger.io/blog/refactoring-in-extreme-programming/#:~:text=Refactoring%20is%20especially%20necessary%20in,fast%20as%20it%20is%20possible). Último acesso 17/02/2021.

STOCK. Disponível em: [https://unbarqdsw.github.io/2020.1_G12_Stock/#/Project/Metodologias](https://unbarqdsw.github.io/2020.1_G12_Stock/#/Project/Metodologias). Último acesso 17/02/2021.
