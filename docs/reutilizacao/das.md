# <center> DOCUMENTO DE ARQUITETURA DE SOFTWARE

|Data | Versão | Descrição | Autor(es)
| -- | -- | -- | -- |
| 16.04.2021 | 0.1 | Pontapé inicial do documento: formatação; adição do 1.1 Propósito | Erick Giffoni; Isabella Carneiro |
| 17.04.2021 | 0.2 | Adição inicial do 1.2 Escopo | Erick Giffoni; Isabella Carneiro |
| 19.04.2021 | 0.3 | Objetivos e restrições | Damarcones; Kalebe |
| 19.04.2021 | 0.4 | Visão de casos de uso | Bruna Almeida, Lucas Lopes, Damarcones Porto |
| 22.04.2021 | 0.5 | Início da introdução | Rafaella Junqueira, Geraldo Victor |
| 22.04.2021 | 0.6 | Representação Arquitetural | Rafaella Junqueira, Geraldo Victor |
| 22.04.2021 | 0.7 | Overview da introdução | Rafaella Junqueira, Geraldo Victor |
| 25.04.2021 | 0.8 | Visão lógica | Rafaella Junqueira, Isabella Carneiro |
| 26.04.2021 | 0.9 | Visão lógica - diagrama de pacotes | Rafaella Junqueira, Isabella Carneiro |
| 26.04.2021 | 0.10 | Diagramas de casos de uso e descrição dos principais casos de uso | Bruna Almeida, Lucas Lopes, Damarcones Porto |
| 27.04.2021 | 0.11 | Visão de processos | Bruna Almeida, Lucas Lopes, Damarcones Porto |
| 27.04.2021 | 0.12 | Visão de implementação | Bruna Almeida, Lucas Lopes, Damarcones Porto |
| 28.04.2021 | 0.13 | Adiciona explicação sobre view no tópico 2; faz uma correção gramatical no tópico 8.1 | Erick Giffoni |
| 28.04.2021 | 0.14 | Adiciona visão de implantação | Bruna Almeida, Lucas Lopes, Damarcones Porto |
| 29.04.2021 | 0.15 | Complementa detalhes no tópico 5.2; adiciona uma explicação para a visão de processos; descreve as camadas do frontend em 8.2; adiciona a imagem e o link para o diagrama de componentes em 8.1; início da Visão de Dados com a adição do DE-R e DLD| Erick Giffoni |
| 01.05.2021 | 0.16 | Formatação do documento | Bruna Almeida, Damarcones Porto |
| 02.05.2021 | 0.17 | Adiciona tópico de Tamanho e performance | Bruna Almeida, Damarcones Porto |
| 02.05.2021 | 0.18 | Adiciona tópico de Qualidade | Bruna Almeida, Damarcones Porto |
| 02.05.2021 | 0.19 | Visão lógica - Diagrama de contexto | Rafaella Junqueira,<br>Geraldo Victor |
| 02.05.2021 | 0.20 | Tranferência do documento de .doc para markdown | Isabella Carneiro |
| 02.05.2021 | 0.21 | Tranferência do documento de .doc para markdown | Rafaella Junqueira |
<br><br>

## 1. Introdução
<div style="line-height:1.8" align="justify">
<p>O documento de arquitetura de software fornece uma visão geral de arquitetura abrangente do sistema de software. Serve como um meio de comunicação entre o arquiteto de software e outros membros de equipe de projeto, com relação a decisões arquiteturalmente significativas tomadas sobre o projeto.</p>
<p>O presente documento tem como objetivo descrever a arquitetura do projeto Cabeleleila Leila, uma aplicação web com o objetivo de facilitar e otimizar o sistema de agendamentos em um salão de beleza. Este documento oferece uma visão arquitetural geral do sistema, usando diversas visões, como visão de caso de uso, visão lógica, dentre outras, para representar diferentes aspectos do mesmo. O objetivo deste documento é capturar e comunicar as decisões arquiteturais significativas que foram tomadas no decorrer do processo de desenvolvimento.</p>
</div>

### 1.1 Propósito
<div style="line-height:1.8" align="justify">
<p>Este documento apresenta uma visão arquitetural compreensiva e holística a respeito do sistema do salão da Leila. Diferentes visões arquiteturais estão presentes aqui para representar determinados aspectos do sistema. Assim, é esperado capturar e expressar as decisões de arquitetura significativas que foram tomadas para consolidar a construção do sistema para o salão da Leila.
        
<p>Esse documento está estruturado da seguinte maneira: primeiro, uma introdução geral sobre o projeto de arquitetura e sobre o sistema em questão; em seguida, a representação arquitetural é explicada, bem como quais visões esse documento aborda; as metas e restrições de arquitetura, na sequência, abordam requisitos de software e outros objetivos importantes para a arquitetura, estratégias etc. Logo, uma série de tópicos representando cada visão utilizada nesse projeto; depois, uma descrição do tamanho e do desempenho desse software; por fim, características de qualidade que se aplicam ao projeto são discutidas.
</div>

A utilização desse documento é dada da seguinte forma:

* **Usuários do sistema**: podem fazer consultas, caso desejem entender melhor o funcionamento do software;
* **Equipe de desenvolvimento**: espera-se que desenvolva o software a partir do que está projetado aqui. Assim, fará consultas e, caso necessário, pedirá esclarecimentos ou mudanças para a equipe de arquitetos de software;
* **Equipe de bancos de dados**: concorda em projetar e implementar o banco de acordo com os objetivos, as restrições e outros aspectos relevantes apresentados aqui,  para o contexto do banco;
* **Equipe de arquitetos**: elabora, revisa, modifica e comunica esse documento de arquitetura para as outras partes interessadas apresentadas anteriormente.

### 1.2 Escopo
<div style="line-height:1.8" align="justify">

<p>O Salão da Cabeleleila Leila é uma aplicação que visa facilitar o gerenciamento de um salão de beleza por meio do cadastro de clientes e do agendamento dos serviços oferecidos pelo estabelecimento.</p>
<p>A aplicação permite que o cliente consulte os tipos de serviços prestados, seus respectivos preços, os horários de atendimento e agende um pedido. Mais ainda, o cliente pode acessar o perfil dos profissionais que atuam no local, avaliar pedidos etc.</p>
<p>Esse documento de arquitetura descreve como a aplicação funciona, quais são os requisitos para o funcionamento correto, quais são as restrições do sistema, caso existam, as tecnologias utilizadas, como o projeto está estruturado e organizado etc. Assim, esse é um dos principais documentos para o projeto do sistema do salão da Leila como um todo, sendo que ele afeta todos os interessados, desde o cliente do Salão aos desenvolvedores deste software.</p>
</div>

### 1.3 Visão Geral
<div style="line-height:1.8" align="justify">
<p>A arquitetura de um software, segundo as normas da IEEE, é a “organização fundamental de um sistema, expressa em seus componentes, nos relacionamentos entre eles e com o ambiente, e nos princípios que governam seu projeto e sua evolução”. O aplicação web Cabeleleila Leila será representada seguindo as seguintes visões arquiteturais:</p></div>
        
* **Visão de Casos de Uso**: Descreve a funcionalidade do sistema, suas interfaces externas, e seus principais usuários.
* **Visão Lógica**: Descreve como o sistema é estruturado, em termos de unidades de implementação.
* **Visão de Processos**: Descreve como o sistema de tempo-de-execução é estruturado na forma de um conjunto de elementos que têm interações e comportamento de tempo-de-execução.
* **Visão de implantação**: Descreve como o sistema é mapeado para o hardware.
* **Visão de Implementação**: Descreve como os artefatos de desenvolvimento estão organizados no sistema de arquivos.<br> 

## 2. Representação Arquitetural
<div style="line-height:1.8" align="justify">
        
<p>O padrão arquitetural utilizado no projeto é um padrão que pode ser entendido como um padrão MVC (Model-View Controller). Este padrão tem como benefício o isolamento das regras de negócios da lógica de apresentação, ou seja, a interface do usuário, uma vez que essa comunicação entre interface e usuário é definida através de um controlador (controller) que separa as camadas.<br>

<p>O modelo (model) tem a responsabilidade de gerenciar e controlar a forma como os dados se comportam por meio das funções, lógica e regras de negócios estabelecidas. É o detentor dos dados recebidos pela controller e aquele que envia as respostas mais adequadas; tanto a controller quanto a model são representadas com a utilização do framework Spring Boot utilizado no backend. A visão (view) também é responsável por apresentar as informações de forma visual ao usuário, representada neste projeto com a utilização do framework Angular.<br> 

<p>Mais ainda, em relação ao backend, a parte de código que lida com mais proximidade e faz chamadas ao banco de dados representa uma view, pois faz a interface entre a requisição e os dados que ela busca. A informação é então retornada para a model, em seguida para a controller, então de volta ao frontend, o qual monta os dados recebidos e os exibe ao usuário (outra view, representando uma interface com o usuário).
        
</div>

### 2.1 Diagrama Relacional
<div style="line-height:1.8" align="justify">

<p>O diagrama relacional representa a divisão da aplicação em microsserviços independentes referentes aos usuários, aos serviços oferecidos pelo salão e os agendamentos realizados.
</div>

[<div align="center"><img hight="auto" width="auto" src="../../img/das/relacional.png"></div>](../../img/das/relacional.png)
<figcaption align='center'>
    <b>Figura 1 - Diagrama Relacional </b>
    <br>
    <small>Autores: Rafaella Junqueira e Geraldo Victor</small>
</figcaption>
<br>

<div style="line-height:1.8" align="justify">
<p>O usuário da aplicação realiza o login e recebe um token de acesso que permanece por um período limitado de tempo. Este token é passado para o banco de dados no momento em que se pretende cadastrar ou agendar um serviço na aplicação para que haja permissão para execução da ação.
</div>

### 2.2 Spring Boot
<div style="line-height:1.8" align="justify">
<p>O Spring é um framework open source para a plataforma Java, um framework não intrusivo, baseado nos padrões de projeto inversão de controle e injeção de dependência. O Spring Boot facilita a criação de aplicativos autônomos baseados em Spring de nível de produção.</p>
</div>

### 2.3 Angular
<div style="line-height:1.8" align="justify">
<p>Angular é uma plataforma de desenvolvimento, construída em TypeScript. O Angular inclui uma estrutura baseada em componentes para a construção de aplicativos da web escalonáveis, uma coleção de bibliotecas bem integradas que cobrem uma ampla variedade de recursos, incluindo roteamento, gerenciamento de formulários e comunicação cliente-servidor.</p>
</div>
        
## 3. Objetivos e Restrições da Arquitetura
<div style="line-height:1.8" align="justify">
<p>Os objetivos arquiteturais dizem respeito às metas mais significativas impostas a um projeto, ou seja, é tudo aquilo que satisfaz as necessidades, expectativas e desejos dos Stakeholders. As restrições arquiteturais de um projeto referem-se aos fatores que limitam a execução da aplicação. Em outras palavras, as restrições podem ser definidas como condições impostas ao sistema, para que este funcione de acordo com o esperado pelos Stakeholders.</p>        
<p>Definir as restrições de um projeto é importante porque assegura a viabilidade do empreendimento e a satisfação dos Stakeholders. Quando um projeto é restringido por fronteiras claras, através de regras bem formuladas, há uma delimitação no campo de atuação do gerente de projetos. Este tópico tem por finalidade descrever os objetivos e restrições cabíveis ao projeto Leila's.</p>
</div>

### 3.1 Objetivos
<div style="line-height:1.8" align="justify">

<ul>
        <li><strong>Escalabilidade</strong>: O software deve tornar possível sua evolução e manutenção.</li>
        <li><strong>Segurança</strong>: A aplicação deve manter os dados dos usuários em total segurança através da utilização de ferramentas para a encriptação de dados.</li>
        <li><strong>Linguagem</strong>: A aplicação deve conter uma linguagem comum e de fácil entendimento para os usuários.</li>
        <li><strong>Portabilidade</strong>: A aplicação deve ser executada com desempenho igual ou similar nos navegadores Google Chrome e Mozila Firefox.</li>
        <li><strong>Usabilidade</strong>: A aplicação deve ser construída seguindo regras de usabilidade para atender a maioria dos usuários.</li>
        <li><strong>Manutenibilidade</strong>: A aplicação deve permitir manutenção e melhorias de maneira a não gerar custo e tempo muito acima do normal. Para isso ser possível, o sistema foi escrito com base em padrões de projetos já conhecidos por grande parte dos desenvolvedores Java.</li>
</ul>
</div>

### 3.2 Restriçoes
<div style="line-height:1.8" align="justify">
<ul>
<li>Tecnologias: A aplicação deverá ser desenvolvida utilizando as seguintes ferramentas e tecnologias:</li>
        <ul>
                <li>Spring Boot: Framework escrito em Java para o desenvolvimento do back-end da aplicação;</li>
                <li>Angular: Framework escrito em JavaScript para o desenvolvimento do front-end da aplicação Web. Possui fácil integração com o bootstrap e permite a utilização do HTML;</li>
                <li>Typescript: Super conjunto do JavaScript, utilizado juntamente ao framework Angular na construção do front- end;</li>
                <li>Bootstrap: Framework de CSS que torna fácil a criação de elementos em websites. Agiliza a criação de páginas esteticamente agradáveis, pois seus padrões de design seguem os princípios de usabilidade para interfaces;</li>
                <li>H2 Database: Banco de dados relacional que armazena os dados em tabelas. Utiliza a linguagem SQL para a manipulação dos dados;</li>
                <li>Github: Controle de versionamento da aplicação.</li>
        </ul>
<li>Conectividade: A aplicação necessitará de conexão com a internet para funcionar.</li>
<li>Prazo: A aplicação deverá ser finalizada na data estipulada para entrega final.</li>
<li>Idioma: A aplicação deve ser voltada para a linguagem Português-Brasil.</li>
<li>Público alvo: A aplicação deve atender usuários que desejam agendar serviços no salão Leila's.</li>
</ul>
</div>

## 4. Visões de Casos de Uso
<div style="line-height:1.8" align="justify">

<p>O Caso de Uso tem como objetivo descrever como será o uso de uma funcionalidade de um sistema. Com base nisso, a visão de Caso de Uso exerce a função de listar casos de uso que representam alguma funcionalidade central e significativa no sistema final, ou seja, descreve cenários ou casos de uso consideráveis para o sistema.
<p>A visão de caso de uso é um aspecto arquitetônico que ilustra os casos e cenários de uso que abrangem comportamento e/ou classes significativas do ponto de vista arquitetônico. Essa visão mostra um subconjunto arquitetonicamente significativo dos casos de uso e atores, que no projeto Leila's são: cliente, funcionário e administrador.
<p>Os casos de uso levantados para o projeto estão listados abaixo. Aqueles que possuem um impacto mais significativo na arquitetura do projeto estão destacados em negrito, e serão descritos em detalhes posteriormente.

<ul>
        <li>UCD01 - Cadastrar usuários;</li>
        <li>UCD02 - Realizar login;</li>
        <li>UCD03 - Agendar horário;</li>
        <li>UCD04 - Recuperar senha;</li>
        <li>UCD05 - Gerenciar estabelecimento;</li>
        <li>UCD06 - Gerenciar perfil de usuário.</li>
</ul>
</div>

Os diagramas de casos de uso gerais estão apresentados abaixo:

[<div align="center"><img hight="auto" width="auto" src="../../img/das/uc1.png"></div>](../../img/das/uc1.png)
<figcaption align='center'>
    <b>Figura 2 - Diagrama de casos de uso geral para todo tipo de usuário </b>
    <br>
    <small>Autores: Bruna Almeida e Damarcones Porto</small>
</figcaption>
<br>

[<div align="center"><img hight="auto" width="auto" src="../../img/das/uc2.png"></div>](../../img/das/uc2.png)
<figcaption align='center'>
    <b>Figura 3 - Diagrama de casos de uso geral para funcionário </b>
    <br>
    <small>Autores: Bruna Almeida e Damarcones Porto</small>
</figcaption>
<br>

[<div align="center"><img hight="auto" width="auto" src="../../img/das/uc3.png"></div>](../../img/das/uc3.png)
<figcaption align='center'>
    <b>Figura 4 - Diagrama de casos de uso geral para cliente</b>
    <br>
    <small>Autores: Bruna Almeida e Damarcones Porto</small>
</figcaption>
<br>

Os casos de uso destacados anteriormente serão detalhados a seguir:

<div style="line-height:1.8" align="justify">
<ul>
<li> <strong>UCD03 - Agendar horário:</strong> este caso de uso ocorre quando o usuário cliente solicita um serviço disponível no salão. Após selecionar o serviço desejado, será apresentado ao cliente uma lista de horários disponíveis, e basta que o cliente selecione o horário pretendido e confirme a solicitação do serviço. Este caso de uso é exclusivo para o perfil de cliente.</li>
<li><strong>UCD05 - Gerenciar estabelecimento:</strong> Caso de uso exclusivo para o perfil de administrador e ocorre quando o administrador deseja consultar serviços cadastrados no sistema, visualizar os agendamentos do salão, criar um usuário, modificar o tipo de permissão de um usuário cadastrado ou excluir um usuário cadastrado. Após fazer o que pretende no sistema, basta que o administrador confirme as alterações para que o sistema seja atualizado.</li>
</ul>
</div>

## 5. Visão Lógica
<div style="line-height:1.8" align="justify">
As visões de arquitetura podem ser consideradas abstrações ou simplificações dos modelos criados, em que se ressaltam as características importantes sem evidenciar os detalhes. A Visão Lógica é utilizada no fluxo de trabalho Análise e Design para fornecer uma base de compreensão da estrutura e da organização de design do sistema.
</div>

### 5.1 Diagrama de Contexto
<div style="line-height:1.8" align="justify">
<p>O diagrama de contexto é um gráfico, composto por um fluxo de dados que mostra as interfaces entre o projeto e a sua relação com o ambiente em que vai ser desenvolvido. O diagrama de contexto funciona como uma descrição dos processos sob a visão de mais alto nível.
</div>

[<div align="center"><img hight="auto" width="auto" src="../../img/das/relacional.png"></div>](../../img/das/relacional.png)
<figcaption align='center'>
    <b>Figura 1 - Diagrama Relacional </b>
    <br>
    <small>Autores: Rafaella Junqueira e Geraldo Victor</small>
</figcaption>
<br>

<div style="line-height:1.8" align="justify">
<p>O usuário faz suas interações com as interfaces criadas através do Framework Angular, cujos padrões de chamada são feitas via endpoint utilizando a tecnologia REST para web services. Essa integração de comunicação é feita do frontend para o backend, aqui desenvolvido utilizando o Framework Spring Boot. 
<p>Por fim, as informações são validadas e carregadas através da técnica ORM (Object-relational mapping) com o Hibernate, que relaciona propriedades de uma classe com colunas do banco de dados, e então são retornadas ao usuário de acordo com a necessidade do que foi solicitado.
</div>

### 5.2 Diagrama de Pacotes

## 6. Visão de Processos

### 6.1 Principais Processos
* createUsuario (): Esse processo é responsável pela criação de usuários do tipo cliente e funcionário, lembrando que o tipo administrador é criado diretamente no sistema;
* getServicos (): Busca os serviços cadastrados no sistema dependendo do objetivo da busca;
* gerenciarServicos (): Esse método edita os serviços nas características em que ele foi cadastrado ou mesmo exclusão/inclusão de serviços;

## 7. Visão de Implantação
<div style="line-height:1.8" align="justify">
Esta seção descreve como o sistema é mapeado para o hardware. Os dados da aplicação Web ficam armazenados no banco de dados PostgreSQL de tal maneira que quando requisitado pelo Back-end, construído em Java, realiza os serviços enviados através da interface, no caso o Front-end, desenvolvido em Angular, que por sua vez, mostra todas as informações necessárias ao usuário.
</div>
<!--- colocar imagem -->

## 8. Visão de Implementação
<div style="line-height:1.8" align="justify">
A finalidade da visão de implementação é captar as decisões de arquitetura tomadas para a implementação. Esta seção descreve a estrutura geral do modelo de implementação, a decomposição do software em camadas e subsistemas no modelo de implementação, e quaisquer componentes arquitetonicamente significativos.
</div>

### 8.1 Visão Geral

### 8.2 Camadas
<div style="line-height:1.8" align="justify">
O projeto é dividido em duas camadas: Front-end e Back-end:.
Front-end: os seguintes pacotes fazem parte do Front-end do projeto Leila’s:
* app: pode-se dizer que é o pacote principal, embora não atue sozinho. Toda a lógica da aplicação, projeto de páginas, rotas, componentes utilizados, arquivos auxiliares, funcionalidades etc estão presentes aqui;
* assets: aqui ficam os "ativos" utilizados nas interfaces com o usuário, os quais incluem diversas imagens, logos etc.;
* environments: representa um conjunto de configurações de ambiente para a aplicação, podendo incluir: variáveis; números de portas de serviços; URLs utilizadas etc.;
* shared: aqui encontra-se arquivos, variáveis, interfaces, constantes etc, compartilhadas para a aplicação como um todo.<br>

Back-end: os pacotes dessa camada estão descritos a seguir.
* Config: nela está contida as configurações iniciais do MVC e da classe SpringFoxConfig;
* Domain: contém as entidades necessárias para o gerenciamento de usuários, tanto cliente quanto funcionário, sendo que o administrador já será setado automaticamente, e os serviços a serem oferecidos pelo estabelecimento;
* Exceptions: É a responsável pelo lançamento de exceções decorrentes de erros;
* Repositories: existe no contexto de executar requisições de método CRUD;
* Security: toda regra de serviço envolvendo questões de segurança estão implementadas nele;
* Service: no pacote service está contida a lógica que implementa a interface para o CRUD;
* Web: responsável basicamente pelo controle de validação de entidades. Um exemplo é a classe UserController, que impede a duplicidade de nomes de usuários.
</div>

## 9. Visão de Dados
<div style="line-height:1.8" align="justify">
Para a visão de dados, representamos aqui como o sistema da Leila's persiste nessas informações. O modelo de entidade-relacionamento (ME-R), bem como o diagrama entidade-relacionamento (DE-R), somado ao diagrama lógico de dados (DLD) foram utilizados. Por questões relacionadas ao tamanho deste documento, apresentamos abaixo somente o DE-R e o DLD.
</div>
        
### 9.1 DE-R

### 9.2 DLD

## 10. Tamanho e Performance
<div style="line-height:1.8" align="justify">


O tamanho da aplicação, levando em consideração apenas o Back-end, foi estimado em 42.9Mb. Esse valor foi alcançado utilizando o comando “MVN install”, gerando um arquivo .jar, o que torna possível a execução do Back-end em qualquer sistema operacional que contenha Java.
Em relação à performance, o sistema foi desenvolvido com foco na otimização de resposta às requisições. Sendo assim, é esperado que o desempenho geral do sistema atenda às expectativas e à testes de Stress.
</div>


## 11. Qualidade
<div style="line-height:1.8" align="justify">

A qualidade da aplicação pode ser mensurada a partir da abordagem NFR. O NFR Framework é uma abordagem para representar e analisar Requisitos Não-Funcionais. Seu objetivo é ajudar desenvolvedores na implementação de soluções personalizadas, levando em consideração as características do domínio e do sistema em questão. Tais características incluem Requisitos Não-funcionais, Requisitos funcionais, prioridades e carga de trabalho. Esses fatores determinam a escolha de alternativas de desenvolvimento para um determinado sistema (CHUNG et al., 2000).<br>

A partir disso, foram levantados NFR’s que aumentam a qualidade do produto, em relação à eficiência, usabilidade, entre outros.
* Usabilidade: A interface do sistema é simples, clara e de fácil interação, seguindo uma padronização de cores e fontes, definidas no documento de identidade visual.
* Segurança: Quando o usuário acessa o sistema através de Login, um token temporário é criado, para realizar a autenticação do usuário e resgatar dados privativos do banco de dados.
* Manutenabilidade: Todo o projeto Leila´s foi documentado no repositório do grupo. Isso facilita a consulta da documentação, e apoia a manutenibilidade do código.
* Confiabilidade: o sistema foi desenvolvido para garantir que o mesmo se recupere em caso de falhas.
* Portabilidade: A utilização do Docker garante um ambiente estável, o que auxilia na criação de possíveis novos módulos.<br>

O projeto ainda está em fase de desenvolvimento até o presente momento (maio de 2021), portanto algumas métricas não podem ser obtidas.
</div>

## Referências

DEVMEDIA, **Introdução ao Padrão MVC**. Disponível em: devmedia.com.br/introducao-ao-padrao-mvc/29308#MVC

LEWAGON, **O que é padrão MVC?**. Disponível em: lewagon.com/pt-BR/blog/o-que-e-padrao-mvc 

SIGED, **Documento de Arquitetura**. Disponível em: fga-eps-mds.github.io/2020-2-SiGeD/architecturedocument/#arquitetura

CIN, **Conceito: Visão Lógica**. Disponível em: cin.ufpe.br/~gta/rup-vc/core.base_rup/guidances/concepts/logical_view_C135365E.html

ROBSON CAMARGO, **Quais os benefícios de criar um diagrama de contexto?**. Disponível em: robsoncamargo.com.br/blog/Quais-os-beneficios-de-criar-um-diagrama-de-contexto

MICHAEL RICHARDSON, **Concept: Use-Case View**. Disponível em: michael-richardson.com/processes/rup_for_sqa/core.base_rup/guidances/concepts/use-case_view_11F15731.htm

ECE, **Use Case View**. Disponível em: ece.uvic.ca/~itraore/seng422-05/notes/arch05-2.pdf

ATÉ O MOMENTO, **O que é caso de uso?**. Disponível em: ateomomento.com.br/o-que-e-caso-de-uso/

QRODÍZIO, **Documento de Arquitetura**. Disponível em: unbarqdsw.github.io/2020.1_G10_QRodizio/documento_de_arquitetura.html#historico-de-revisao

WALDERSON, **Conceito: Visão de Processos**. Disponível em: walderson.com/IBM/RUP7/LargeProjects/core.base_rup/guidances/concepts/process_view_E3DD0B09.html

TRT9, **Diretriz: Visão Arquitetural**. Disponível em: trt9.jus.br/pds/pdstrt9/guidances/guidelines/architectural_view_FF6EDA37.html

UFPR, **Visões Arquiteturais**. Disponível em: https://www.inf.ufpr.br/andrey/ci163/VisoesAl.pdf

WOCO, **Documento de Arquitetura**. Disponível em: unbarqdsw.github.io/2020.1_G9_WoCo/#/Arquitetura%20de%20Software/4.1%20Estilos%20e%20Padr%C3%B5es%20Arquiteturais/DAS?id=_7-vis%c3%a3o-de-implementa%c3%a7%c3%a3o

TRIÁGIL, **Documento de Arquitetura**. Disponível em: unbarqdsw.github.io/2020.1_G1_Triagil/arquitetura_software_e_reutilizacao/documento_de_arquitetura/

DIÁRIO DA SAÚDE, **Documento de Arquitetura de Software (DAS)**. Disponível em: https://unbarqdsw.github.io/2020.1_G5_Diario_da_Saude/#das/#visao-de-dados