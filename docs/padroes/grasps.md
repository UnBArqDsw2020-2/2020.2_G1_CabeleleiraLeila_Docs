# <center> GRASP's
<br>
    
### Histórico de versão<br>
    
|Data | Versão | Descrição | Autor(es)|
| -- | -- | -- | -- |
| 25.03.2021 | 0.1 | Criação do documento | Rafaella Junqueira<br>Kalebe Lopes|
| 25.03.2021 | 0.2 | Adição do diagrama Baixo Acoplamento | Rafaella Junqueira<br>Kalebe Lopes|
| 25.03.2021 | 0.2 | Adição do diagrama Controller | Rafaella Junqueira<br>Kalebe Lopes |
| 28.03.2021 | 1.0 | Edição e revisão da versão 1.0 | Erick Giffoni |
| 01.04.2021 | 1.1 | Refatoração do documento | Isabella Carneiro |

### Participantes

* Rafaella Junqueira
* Kalebe Lopes
* Erick Giffoni
* Isabella Carneiro

### Introdução
<div align="justify">

O General Responsability Assignment Software Patterns um conjunto de ferramentas mentais, um auxílio de aprendizagem para ajudar no projeto de software orientado a objetos. Consiste em diretrizes para atribuir responsabilidade a classes e objetos em projeto orientado a objetos.
<br><br>
O termo responsabilidade deve ser entendido como as obrigações que um objeto possui quando se leva em conta o seu papel dentro de um determinado contexto. Todos esses padrões servem para a resolução de problemas comuns e bastante típicos de desenvolvimento de software orientado a objeto. Portanto, tais técnicas apenas documentam e normatizam as práticas já consolidadas, testadas e conhecidas no mercado.
<br><br>
Ressaltamos que os padrões documentados estão sendo amplamente utilizados no projeto, entretanto, para fins de explicação, utilizamos apenas alguns exemplos representativos onde cada padrão pode ser encontrado no projeto.
</div><br>


### Padrões utilizados no projeto

| | |
|:--:|:--:|
[Baixo acoplamento]() | [Controller]() 


## <center> Baixo Acoplamento
<div align="justify">

O padrão de Baixo Acoplamento é um padrão de avaliação, que determina como atribuir responsabilidades de suporte de modo que o acoplamento entre classes permaneça baixo. A utilização deste padrão oferece benefícios, como menor dependência entre as classes, redução de impacto das mudanças e aumento do potencial de reutilização das classes.

</div><br>

### Aplicações no projeto
<div align="justify">

Os códigos criados utilizam a divisão de responsabilidades entre as classes, de modo que, para a evitar a dependência entre elas, existem interfaces que abarcam os métodos comuns a todas. Assim, caso haja necessidade de mudanças, basta alterar apenas a interface específica daquela classe.
<br><br>
Este padrão é aplicado, por exemplo, entre a classe de serviço ServicoService e a interface ServicoRepository, a qual herda a implementação dos métodos advindos da interface CrudRepository. 
Para a representação do funcionamento do padrão GRASP de baixo acoplamento adotado no projeto, foi modelado um diagrama UML exemplificando a utilização da interface ServiceRepository por parte da classe de serviço intitulada ServicoService.
Note que a classe ServicoService usa a ServicoRepository, e esta tem herança da CrudRepository.
</div><br>

[<div align="center"><img src="../../img/padroes/baixo-acoplamento.png"></div>](../../img/padroes/baixo-acoplamento.png)
<figcaption align='center'>
    <b>Figura 1 - Exemplo de uso de interface pela classe ServicoService</b>
    <br>
    <small>Autores: Rafaella Junqueira e Kalebe Lopes</small>
</figcaption>
<br>

## <center> Controller
<div align="justify">

O padrão Controller (ou Controlador) é aquele que atribui a responsabilidade de lidar com os eventos do sistema para uma classe que representa um cenário de caso de uso do sistema global. Um objeto controlador é um objeto de interface não-usuário, responsável por receber ou manipular um evento do sistema. O controlador é definido como o primeiro objeto além da camada UI que recebe e coordena as operações do sistema, e deve delegar o trabalho a ser feito aos outros objetos.
<br><br>
O padrão visa responder a seguinte pergunta: Quem deve ser o responsável por lidar com um evento de uma interface de entrada?. Ainda, esse padrão pode ser considerado uma parte da camada de aplicação/serviço, uma vez que a aplicação tenha feito uma distinção explícita entre a camada de aplicativo/serviço e a camada de domínio em um sistema orientado a objetos.

</div><br>

### Aplicações no projeto
<div align="justify">

A parte Backend do projeto está estruturada de forma que o diretório web/resources recebe os arquivos responsáveis por realizar o primeiro contato das requisições provenientes do Frontend. Assim, esses arquivos assumem o papel de controladores da aplicação, uma vez que para cada tipo de requisição existe uma maneira de recebê-la e tratá-la. A partir disso, a responsabilidade de lidar com mais detalhes sobre o pedido recebido é atribuída aos arquivos alocados na pasta services.
<br><br>
Um exemplo de utilização do padrão é o controlador dos serviços, ServicoResource.java, em que cada tipo de requisição https é mapeada por um método específico. Cada método irá capturar um tipo de requisição (o evento de entrada), como get, put, post ou delete, e atribuir a responsabilidade de tratar esse evento ao arquivo ServicoService.java.
<br><br>
A representação do funcionamento do padrão ao projeto foi modelada em um diagrama UML que exemplifica a criação de um serviço por parte do usuário administrador. A imagem demonstra o fluxo entre uma requisição realizada no Frontend e seu primeiro contato com o Backend via ServicoResource. Em seguida, a ação de criar o serviço solicitado é realizada pela ServicoService.
</div>

[<div align="center"><img src="../../img/padroes/uml-controller.png"></div>](../../img/padroes/uml-controller.png)
<figcaption align='center'>
    <b>Figura 2 - Exemplo de criação de um serviço</b>
    <br>
    <small>Autores: Rafaella Junqueira e Kalebe Lopes</small>
</figcaption>
<br>

## Referências
<br>

Universidade Federal de Uberlândia. **Padrões GRASPs** Disponível em [http://www.facom.ufu.br/~bacala/ESOF/05a-Padr%C3%B5es%20GRASP.pdf](http://www.facom.ufu.br/~bacala/ESOF/05a-Padr%C3%B5es%20GRASP.pdf). Acesso em 12 de março de 2021.

SERRANO, Milene. **Demais GRASPs**, 2021. Material apresentado na Disciplina de Arquitetura e Desenho de Software do curso de Engenharia de Software da UnB, FGA. Acesso em 9 de março de 2021.

DEVMEDIA, **Desenvolvimento com qualidade com GRASP** Disponível em [https://www.devmedia.com.br/desenvolvimento-com-qualidade-com-grasp/28704](https://www.devmedia.com.br/desenvolvimento-com-qualidade-com-grasp/28704) Acesso em 9 de março de 2021.