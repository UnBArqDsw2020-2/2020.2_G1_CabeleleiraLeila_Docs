# <center> Padrões GRASP's
<br>
    
### Histórico de versão<br>
    
|Data | Versão | Descrição | Autor(es)|
| -- | -- | -- | -- |
| 25.03.2021 | 0.1 | Criação do documento | Rafaella Junqueira<br>Kalebe Lopes|
| 25.03.2021 | 0.2 | Adição conteúdo Baixo Acoplamento | Rafaella Junqueira<br>Kalebe Lopes|
| 25.03.2021 | 0.3 | Adição conteúdo Controller | Rafaella Junqueira<br>Kalebe Lopes |
| 28.03.2021 | 1.0 | Edição e revisão da versão 1.0 | Erick Giffoni |
| 01.04.2021 | 1.1 | Refatoração do documento | Isabella Carneiro |
| 05.04.2021 | 1.2 | Adição conteúdo Indireção | Rafaella Junqueira<br>Geraldo Victor<br>Kalebe Lopes |

### Participantes

* Rafaella Junqueira
* Kalebe Lopes
* Erick Giffoni
* Isabella Carneiro
* Geraldo Victor
<br>

### Padrões utilizados no projeto
- [Baixo acoplamento](#baixo-acoplamento)<br>
- [Controller](#controller)<br> 
- [Indireção](#indirecao)<br>
<br>

### Introdução
<div align="justify">
<p>O General Responsability Assignment Software Patterns um conjunto de ferramentas mentais, um auxílio de aprendizagem para ajudar no projeto de software orientado a objetos. Consiste em diretrizes para atribuir responsabilidade a classes e objetos em projeto orientado a objetos.</p>
<p>O termo responsabilidade deve ser entendido como as obrigações que um objeto possui quando se leva em conta o seu papel dentro de um determinado contexto. Todos esses padrões servem para a resolução de problemas comuns e bastante típicos de desenvolvimento de software orientado a objeto. Portanto, tais técnicas apenas documentam e normatizam as práticas já consolidadas, testadas e conhecidas no mercado.</p>
<p>Ressaltamos que os padrões documentados estão sendo amplamente utilizados no projeto, entretanto, para fins de explicação, utilizamos apenas alguns exemplos representativos onde cada padrão pode ser encontrado no projeto.</p>
</div>

### Metodologia
<div align="justify">
<p>A documentação dos padrões GRASP foi realizada em conjunto pelos membros citados. Para cada padrão, houve uma reunião onde os integrantes discutiram sobre a definição teórica do padrão e como ele estava aplicado no projeto. Logo em seguida, ainda durante as reuniões, foram modelados os diagramas UML para o respectivo assunto abordado em cada uma delas.</p>
</div><br>

## <center> Baixo Acoplamento
<div align="justify"><br>
<p>O padrão de Baixo Acoplamento é um padrão de avaliação, que determina como atribuir responsabilidades de suporte de modo que o acoplamento entre classes permaneça baixo. A utilização deste padrão oferece benefícios, como menor dependência entre as classes, redução de impacto das mudanças e aumento do potencial de reutilização das classes.</p>
</div>

### Aplicações no projeto
<div align="justify">
<p>Os códigos criados utilizam a divisão de responsabilidades entre as classes, de modo que, para a evitar a dependência entre elas, existem interfaces que abarcam os métodos comuns a todas. Assim, caso haja necessidade de mudanças, basta alterar apenas a interface específica daquela classe.</p>
<p>Este padrão é aplicado, por exemplo, entre a classe de serviço ServicoService e a interface ServicoRepository, a qual herda os métodos advindos da interface CrudRepository. Ou seja, a classe ServicoService usa a ServicoRepository, e esta tem herança da CrudRepository.</p> 
Para a representação do funcionamento do padrão GRASP de baixo acoplamento adotado no projeto, foi modelado um diagrama UML exemplificando a utilização da interface ServiceRepository por parte da classe de serviço intitulada ServicoService.</p>
</div>

[<div align="center"><img src="../../img/padroes/baixo-acoplamento.png"></div>](../../img/padroes/baixo-acoplamento.png)
<figcaption align='center'>
    <b>Figura 1 - Exemplo de uso de interface pela classe ServicoService</b>
    <br>
    <small>Autores: Rafaella Junqueira e Kalebe Lopes</small>
</figcaption>
<br>

## <center> Controller
<div align="justify"><br>
<p>O padrão Controller (ou Controlador) é aquele que atribui a responsabilidade de lidar com os eventos do sistema para uma classe que representa um cenário de caso de uso do sistema global. Um objeto controlador é um objeto de interface não-usuário, responsável por receber ou manipular um evento do sistema. O controlador é definido como o primeiro objeto além da camada UI que recebe e coordena as operações do sistema, e deve delegar o trabalho a ser feito aos outros objetos.</p>
<p>O padrão visa responder a seguinte pergunta: <strong>Quem deve ser o responsável por lidar com um evento de uma interface de entrada?</strong> Ainda, este padrão pode ser considerado uma parte da camada de aplicação/serviço, uma vez que a aplicação tenha feito uma distinção explícita entre a camada de aplicativo/serviço e a camada de domínio em um sistema orientado a objetos.</p>
</div>

### Aplicações no projeto

<div align="justify"><br>
<p>A parte Backend do projeto está estruturada de forma que o diretório web/resources recebe os arquivos responsáveis por realizar o primeiro contato das requisições provenientes do Frontend. Assim, esses arquivos assumem o papel de controladores da aplicação, uma vez que para cada tipo de requisição existe uma maneira de recebê-la e tratá-la. A partir disso, a responsabilidade de lidar com mais detalhes sobre o pedido recebido é atribuída aos arquivos alocados na pasta services.</p>
<p>Um exemplo de utilização do padrão é o controlador dos serviços, ServicoResource.java, em que cada tipo de requisição https é mapeada por um método específico. Cada método irá capturar um tipo de requisição (o evento de entrada), como get, put, post ou delete, e atribuir a responsabilidade de tratar esse evento ao arquivo ServicoService.java.</p>
<p>A representação do funcionamento do padrão ao projeto foi modelada em um diagrama UML que exemplifica a criação de um serviço por parte do usuário administrador. A imagem demonstra o fluxo entre uma requisição realizada no Frontend e seu primeiro contato com o Backend via ServicoResource. Em seguida, a ação de criar o serviço solicitado é realizada pela ServicoService.</p>
</div>

[<div align="center"><img src="../../img/padroes/uml-controller.png"></div>](../../img/padroes/uml-controller.png)
<figcaption align='center'>
    <b>Figura 2 - Exemplo de criação de um serviço</b>
    <br>
    <small>Autores: Rafaella Junqueira e Kalebe Lopes</small>
</figcaption>
<br>

## <center> Indireção
<div align="justify"><br>
<p>O padrão de indireção suporta baixo acoplamento (e potencial de reutilização) entre dois elementos, atribuindo a objeto intermediário a responsabilidade de ser o mediador entre eles. Será atribuída a responsabilidade a um objeto intermediário que faz mediação entre componentes e serviços de modo que esses não sejam diretamente acoplados.</p>
<p>O objetivo deste padrão é responder às seguintes perguntas: <strong>Como evitar acoplamento direto entre duas ou mais classes? Como evitar baixo acoplamento e manter alta possibilidade de reuso através do desacoplamento de objetos?</strong> Uma solução para essas questão é a criação de uma camada de indireção entre os dois
componentes que não mais dependem um do outro: ambos dependem da indireção</p>
</div>

### Aplicações no projeto
<div align="justify"><br>
<p>Um exemplo de aplicação deste padrão é a introdução do componente controlador para mediação entre dados (modelo) e sua representação (visualização) no padrão MVC. A parte backend do projeto é estruturada de forma que os arquivos do diretório Resource funcionam como os controllers e os arquivos do diretório Service como as models, responsáveis por receber as requisições vindas do controller e gerar respostas a partir destas requisições.</p>
</div>

[<div align="center"><img src="../../img/padroes/uml-mvc.png"></div>](../../img/padroes/uml-mvc.png)
<figcaption align='center'>
    <b>Figura 3 - Estrutura do projeto</b>
    <br>
    <small>Autores: Rafaella Junqueira e Kalebe Lopes</small>
</figcaption>

<div align="justify"><br>
<p>Os dados do backend são retornados em forma de arquivos .json e estes serão consumidos pelo framework Angular, responsável por realizar a exibição do conteúdo por meio de componentes html. Os comportamentos desses componentes são definidos em arquivos do tipo typescript e estilizados em arquivos css.</p>
</div>

## Referências
<br>
Universidade Federal de Uberlândia. **Padrões GRASPs** Disponível em [http://www.facom.ufu.br/~bacala/ESOF/05a-Padr%C3%B5es%20GRASP.pdf](http://www.facom.ufu.br/~bacala/ESOF/05a-Padr%C3%B5es%20GRASP.pdf). Acesso em 12 de março de 2021.

SERRANO, Milene. **Demais GRASPs**, 2021. Material apresentado na Disciplina de Arquitetura e Desenho de Software do curso de Engenharia de Software da UnB, FGA. Acesso em 9 de março de 2021.

DEVMEDIA, **Desenvolvimento com qualidade com GRASP** Disponível em [https://www.devmedia.com.br/desenvolvimento-com-qualidade-com-grasp/28704](https://www.devmedia.com.br/desenvolvimento-com-qualidade-com-grasp/28704) Acesso em 9 de março de 2021.

DEVMEDIA, **Padrão MVC - Java Magazine** Disponível em [https://www.devmedia.com.br/padrao-mvc-java-magazine/21995#2](https://www.devmedia.com.br/padrao-mvc-java-magazine/21995#2) Acesso em 1 de abril de 2021.

DEVMEDIA, **Java Spring MVC: Criando Aplicações Web em Java** Disponível em [https://www.devmedia.com.br/java-spring-mvc-criando-aplicacoes-web-em-java/31521](https://www.devmedia.com.br/java-spring-mvc-criando-aplicacoes-web-em-java/31521) Acesso em 1 de abril de 2021.