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
| 02.05.2021 | 0.19 | Visão lógica - Diagrama de contexto | Rafaella Junqueira, Geraldo Victor |
| 02.05.2021 | 0.20 | Tranferência do documento de .word para .md | Isabella Carneiro |
<br><br>

## 1. Introdução
<div align="justify">
O documento de arquitetura de software fornece uma visão geral de arquitetura abrangente do sistema de software. Serve como um meio de comunicação entre o arquiteto de software e outros membros de equipe de projeto, com relação a decisões arquiteturalmente significativas tomadas sobre o projeto.<br>
        
O presente documento tem como objetivo descrever a arquitetura do projeto Cabeleleila Leila, uma aplicação web com o objetivo de facilitar e otimizar o sistema de agendamentos em um salão de beleza. Este documento oferece uma visão arquitetural geral do sistema, usando diversas visões, como visão de caso de uso, visão lógica, dentre outras, para representar diferentes aspectos do mesmo. O objetivo deste documento é capturar e comunicar as decisões arquiteturais significativas que foram tomadas no decorrer do processo de desenvolvimento.<br>
</div>

### 1.1 Propósito
<div align="justify">
Este documento apresenta uma visão arquitetural compreensiva e holística a respeito do sistema do salão da Leila. Diferentes visões arquiteturais estão presentes aqui para representar determinados aspectos do sistema. Assim, é esperado capturar e expressar as decisões de arquitetura significativas que foram tomadas para consolidar a construção do sistema para o salão da Leila.
        
Esse documento está estruturado da seguinte maneira: primeiro, uma introdução geral sobre o projeto de arquitetura e sobre o sistema em questão; em seguida, a representação arquitetural é explicada, bem como quais visões esse documento aborda; as metas e restrições de arquitetura, na sequência, abordam requisitos de software e outros objetivos importantes para a arquitetura, estratégias etc. Logo, uma série de tópicos representando cada visão utilizada nesse projeto; depois, uma descrição do tamanho e do desempenho desse software; por fim, características de qualidade que se aplicam ao projeto são discutidas.

A utilização desse documento é dada da seguinte forma:
* Usuários do sistema: podem fazer consultas, caso desejem entender melhor o funcionamento do software;
* Equipe de desenvolvimento: espera-se que desenvolva o software a partir do que está projetado aqui. Assim, fará consultas e, caso necessário, pedirá esclarecimentos ou mudanças para a equipe de arquitetos de software;
* Equipe de bancos de dados: concorda em projetar e implementar o banco de acordo com os objetivos, as restrições e outros aspectos relevantes apresentados aqui,  para o contexto do banco;
* Equipe de arquitetos: elabora, revisa, modifica e comunica esse documento de arquitetura para as outras partes interessadas apresentadas anteriormente.
</div>

### 1.2 Escopo
<div align="justify">

O Salão da Cabeleleila Leila é uma aplicação que visa facilitar o gerenciamento de um salão de beleza por meio do cadastro de clientes e do agendamento dos serviços oferecidos pelo estabelecimento.

A aplicação permite que o cliente consulte os tipos de serviços prestados, seus respectivos preços, os horários de atendimento e agende um pedido. Mais ainda, o cliente pode acessar o perfil dos profissionais que atuam no local, avaliar pedidos etc.

Esse documento de arquitetura descreve como a aplicação funciona, quais são os requisitos para o funcionamento correto, quais são as restrições do sistema, caso existam, as tecnologias utilizadas, como o projeto está estruturado e organizado etc. Assim, esse é um dos principais documentos para o projeto do sistema do salão da Leila como um todo, sendo que ele afeta todos os interessados, desde o cliente do Salão aos desenvolvedores deste software.
</div>

### 1.3 Referências
DEVMEDIA, Introdução ao Padrão MVC. Disponível em: devmedia.com.br/introducao-ao-padrao-mvc/29308#MVC
LEWAGON, O que é padrão MVC?. Disponível em: lewagon.com/pt-BR/blog/o-que-e-padrao-mvc 
SIGED, Documento de Arquitetura. Disponível em: fga-eps-mds.github.io/2020-2-SiGeD/architecturedocument/#arquitetura
CIN, Conceito: Visão Lógica. Disponível em: cin.ufpe.br/~gta/rup-vc/core.base_rup/guidances/concepts/logical_view_C135365E.html
ROBSON CAMARGO, Quais os benefícios de criar um diagrama de contexto?. Disponível em: robsoncamargo.com.br/blog/Quais-os-beneficios-de-criar-um-diagrama-de-contexto
MICHAEL RICHARDSON, Concept: Use-Case View. Disponível em: michael-richardson.com/processes/rup_for_sqa/core.base_rup/guidances/concepts/use-case_view_11F15731.htm
ECE, Use Case View. Disponível em: ece.uvic.ca/~itraore/seng422-05/notes/arch05-2.pdf
ATÉ O MOMENTO, O que é caso de uso?. Disponível em: ateomomento.com.br/o-que-e-caso-de-uso/
QRODÍZIO, Documento de Arquitetura. Disponível em: unbarqdsw.github.io/2020.1_G10_QRodizio/documento_de_arquitetura.html#historico-de-revisao
WALDERSON, Conceito: Visão de Processos. Disponível em: walderson.com/IBM/RUP7/LargeProjects/core.base_rup/guidances/concepts/process_view_E3DD0B09.html
TRT9, Diretriz: Visão Arquitetural. Disponível em: trt9.jus.br/pds/pdstrt9/guidances/guidelines/architectural_view_FF6EDA37.html
UFPR, Visões Arquiteturais. Disponível em: https://www.inf.ufpr.br/andrey/ci163/VisoesAl.pdf
WOCO, Documento de Arquitetura. Disponível em: unbarqdsw.github.io/2020.1_G9_WoCo/#/Arquitetura%20de%20Software/4.1%20Estilos%20e%20Padr%C3%B5es%20Arquiteturais/DAS?id=_7-vis%c3%a3o-de-implementa%c3%a7%c3%a3o
TRIÁGIL, Documento de Arquitetura. Disponível em: unbarqdsw.github.io/2020.1_G1_Triagil/arquitetura_software_e_reutilizacao/documento_de_arquitetura/
DIÁRIO DA SAÚDE, Documento de Arquitetura de Software (DAS). Disponível em: https://unbarqdsw.github.io/2020.1_G5_Diario_da_Saude/#das/#visao-de-dados

### 1.4 Visão Geral
<div align = "justify">
       A arquitetura de um software, segundo as normas da IEEE, é a “organização fundamental de um sistema, expressa em seus componentes, nos relacionamentos entre eles e com o ambiente, e nos princípios que governam seu projeto e sua evolução”. O aplicação web Cabeleleila Leila será representada seguindo as seguintes visões arquiteturais: 
        
* Visão de Casos de Uso: Descreve a funcionalidade do sistema, suas interfaces externas, e seus principais usuários.
* Visão Lógica: Descreve como o sistema é estruturado, em termos de unidades de implementação.
* Visão de Processos: Descreve como o sistema de tempo-de-execução é estruturado na forma de um conjunto de elementos que têm interações e comportamento de tempo-de-execução.
* Visão de implantação: Descreve como o sistema é mapeado para o hardware.
* Visão de Implementação: Descreve como os artefatos de desenvolvimento estão organizados no sistema de arquivos.
 
<\div>

## 2. Representação Arquitetural
<div align = "justify">
        
O padrão arquitetural utilizado no projeto é um padrão que pode ser entendido como um padrão MVC (Model-View Controller). Este padrão tem como benefício o isolamento das regras de negócios da lógica de apresentação, ou seja, a interface do usuário, uma vez que essa comunicação entre interface e usuário é definida através de um controlador (controller) que separa as camadas.<br>

O modelo (model) tem a responsabilidade de gerenciar e controlar a forma como os dados se comportam por meio das funções, lógica e regras de negócios estabelecidas. É o detentor dos dados recebidos pela controller e aquele que envia as respostas mais adequadas; tanto a controller quanto a model são representadas com a utilização do framework Spring Boot utilizado no backend. A visão (view) também é responsável por apresentar as informações de forma visual ao usuário, representada neste projeto com a utilização do framework Angular.<br> 

Mais ainda, em relação ao backend, a parte de código que lida com mais proximidade e faz chamadas ao banco de dados representa uma view, pois faz a interface entre a requisição e os dados que ela busca. A informação é então retornada para a model, em seguida para a controller, então de volta ao frontend, o qual monta os dados recebidos e os exibe ao usuário (outra view, representando uma interface com o usuário).
        
<\div>

### 2.1 Diagrama Relacional
<div align = "justify">

O diagrama relacional representa a divisão da aplicação em microsserviços independentes referentes aos usuários, aos serviços oferecidos pelo salão e os agendamentos realizados.
<!--- colocar imagem -->
O usuário da aplicação realiza o login e recebe um token de acesso que permanece por um período limitado de tempo. Este token é passado para o banco de dados no momento em que se pretende cadastrar ou agendar um serviço na aplicação para que haja permissão para execução da ação.
<\div>

### 2.2 Spring Boot
<div align = "justify">
O Spring é um framework open source para a plataforma Java, um framework não intrusivo, baseado nos padrões de projeto inversão de controle e injeção de dependência. O Spring Boot facilita a criação de aplicativos autônomos baseados em Spring de nível de produção.
<\div>

### 2.3 Angular
<div align = "justify">
Angular é uma plataforma de desenvolvimento, construída em TypeScript. O Angular inclui uma estrutura baseada em componentes para a construção de aplicativos da web escalonáveis, uma coleção de bibliotecas bem integradas que cobrem uma ampla variedade de recursos, incluindo roteamento, gerenciamento de formulários e comunicação cliente-servidor.
<\div>
        
## 3. Objetivos e Restrições da Arquitetura
<div align = "justify">
Os objetivos arquiteturais dizem respeito às metas mais significativas impostas a um projeto, ou seja, é tudo aquilo que satisfaz as necessidades, expectativas e desejos dos Stakeholders. As restrições arquiteturais de um projeto referem-se aos fatores que limitam a execução da aplicação. Em outras palavras, as restrições podem ser definidas como condições impostas ao sistema, para que este funcione de acordo com o esperado pelos Stakeholders.<br>
        
Definir as restrições de um projeto é importante porque assegura a viabilidade do empreendimento e a satisfação dos Stakeholders. Quando um projeto é restringido por fronteiras claras, através de regras bem formuladas, há uma delimitação no campo de atuação do gerente de projetos. Este tópico tem por finalidade descrever os objetivos e restrições cabíveis ao projeto Leila's.

<\div>
### 3.1 Objetivos
<div align = "justify">
* Escalabilidade: O software deve tornar possível sua evolução e manutenção.
* Segurança: A aplicação deve manter os dados dos usuários em total segurança através da utilização de ferramentas para a encriptação de dados.
* Linguagem: A aplicação deve conter uma linguagem comum e de fácil entendimento para os usuários.
* Portabilidade: A aplicação deve ser executada com desempenho igual ou similar nos navegadores Google Chrome e Mozila Firefox.
* Usabilidade: A aplicação deve ser construída seguindo regras de usabilidade para atender a maioria dos usuários.
* Manutenibilidade: A aplicação deve permitir manutenção e melhorias de maneira a não gerar custo e tempo muito acima do normal. Para isso ser possível, o sistema foi escrito com base em padrões de projetos já conhecidos por grande parte dos desenvolvedores Java.
<\div>

### 3.2 Restriçoes 
* Tecnologias: A aplicação deverá ser desenvolvida utilizando as seguintes ferramentas e tecnologias:
        * Spring Boot: Framework escrito em Java para o desenvolvimento do back-end da aplicação;
        * Angular: Framework escrito em JavaScript para o desenvolvimento do front-end da aplicação Web. Possui fácil integração com o bootstrap e permite a utilização do HTML;
        * Typescript: Super conjunto do JavaScript, utilizado juntamente ao framework Angular na construção do front- end;
        * Bootstrap: Framework de CSS que torna fácil a criação de elementos em websites. Agiliza a criação de páginas esteticamente agradáveis, pois seus padrões de design seguem os princípios de usabilidade para interfaces;
        * PostgreSQL: Banco de dados relacional que armazena os dados em tabelas. Utiliza a linguagem SQL para a manipulação dos dados;
        * Github: Controle de versionamento da aplicação.
* Conectividade: A aplicação necessitará de conexão com a internet para funcionar.
* Prazo: A aplicação deverá ser finalizada na data estipulada para entrega final.
* Idioma: A aplicação deve ser voltada para a linguagem Português-Brasil.
* Público alvo: A aplicação deve atender usuários que desejam agendar serviços no salão Leila's.

