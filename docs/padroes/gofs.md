# <center> Padrões GoF
<br>
    
### Histórico de versão<br>
    
|Data | Versão | Descrição | Autor(es)|
| :--: | :--: | -- | -- |
| 04.04.2021 | 0.1 | Criação do documento | Rafaella Junqueira<br>Geraldo Victor<br>Isabella Carneiro |
| 04.04.2021 | 0.2 | Adição do conteúdo criacionais | Rafaella Junqueira<br>Geraldo Victor<br>Isabella Carneiro |
| 04.04.2021 | 0.3 | Adição do conteúdo comportamentais |Geraldo Victor<br> Rafaella Junqueira<br>Kalebe Lopes |
| 04.04.2021 | 0.4 | Adição do conteúdo estruturais | Lucas Lopes<br>Rafaella Junqueira<br>Erick Giffoni |


### Participantes

* Rafaella Junqueira
* Kalebe Lopes
* Erick Giffoni
* Isabella Carneiro
* Geraldo Victor
<br>

### Padrões utilizados no projeto
<!-- - [Abstract Factory](gof-abstract-factory.md) // mudar!!! -->
| Tipo | Padrão |
| -- | -- |
| Criacionais | [Builder](gof-builder.md)<br>[Singleton](gof-singleton.md)
| Estruturais | [Decorator](gof-decorator.md)<br>[]()
| Comportamentais | [Observer](gof-observer.md)<br>
| Emergentes | [Injeção de dependência]()<br>

<br>

### Introdução
<div align="justify">

<p>Um padrão de projeto é uma solução geral para um problema que ocorre com frequência dentro de um determinado contexto no projeto de software. Os padrões são melhores práticas formalizadas podem ser usadas para resolver problemas comuns ao projetar uma aplicação e, quando se referem a projeto orientados a objeto, normalmente mostram relacionamentos e interações entre classes ou objetos.<p>
<p>

Esses padrões de projeto visam facilitar a reutilização de soluções de desenho e facilitar a comunicação, documentação e aprendizado dos sistemas de software. Os padrões GoF são divididos em 3 categorias: <a href="#criacionais">criacionais</a>,  <a href="#comportamentais">comportamentais</a> e <a href="#estruturais">estruturais</a>, que abarcam um total de 24 tipos de padrões.
<p>

</div>

### Criacionais
<div align="justify">
<p>Os padrões de criação são aqueles que abstraem e/ou adiam o processo criação dos objetos, ajudando a tornar um sistema que não seja dependente da maneira como seus objetos são criados, compostos e representados. Estes padrões fornecem vários mecanismos de criação de objetos, que aumentam a flexibilidade e reutilização de código já existente.</p>
Esta categoria abarca os padrões:</p>
</div>
- **Singleton**: assegura que somente um objeto de uma determinada classe seja criado em todo o projeto;
- **Abstract** Factory: permite que um cliente crie famílias de objetos sem especificar suas classes concretas;
- **Builder**: encapsular a construção de um produto e permitir que ele seja construído em etapas;
- **Prototype**: permite você criar novas instancias simplesmente copiando instancias existentes;
- **Factory Mathod**: as subclasses decidem quais classes concretas serão criadas.

### Comportamentais
<div align="justify">
<p>Os padrões de comportamento se concentram nas atribuições de responsabilidades entre os objetos, mas não descrevem apenas padrões de objetos ou de classes, mas também os padrões de comunicação entre os objetos.</p>
Esta categoria abarca os padrões:</p>
</div>
- **Chain of Responsability**: permite dar a mais de um objeto a oportunidade de processar uma solicitação;
- **Command**: encapsula uma solicitação como um objeto;
- **Iterator**: fornece uma maneira de acessar seqüencialmente uma coleção de objetos sem expor a sua implementação;
- **Mediator**: centraliza operações complexas de comunicação e controle entre objetos relacionados;
- **Memento**: permite restaurar um objeto a um dos seus estados prévios, por exemplo, quando o usuário seleciona um “desfazer”;
- **Observer**: permite notificar outros objetos quando ocorre uma mudança de estado;
- **State**: encapsula comportamentos baseados em estados e usa a delegação para alternar comportamentos;
- **Strategy**: encapsula comportamentos intercambiáveis e usa a delegação para decidir qual deles será usado;
- **Template Method**: As subclasses decidem como implementar os passos de um algoritimo;
- **Visitor**: permite acrescentar novos recursos a um composto de objetos e o encapsulamento não é importante;


### Estruturais
<div align="justify">
<p>Os padrões estruturais se preocupam com a forma como classes e objetos são compostos para formar estruturas maiores. Quando aplicados à orientação a objetos, as classes utilizam a herança para compor interfaces ou implementações, e  os de objeto descrevem maneiras de compor objetos para obter novas funcionalidades. Estes padrões explicam como montar objetos e classes em estruturas maiores mas ainda mantendo essas estruturas flexíveis e eficientes.</p>
Esta categoria abarca os padrões:</p>
</div>
- **Decorator**: envelopa um objeto para fornecer novos comportamentos;
- **Proxy**: envelopa um objeto para controlar o acesso a ele;
- **FlyWeigth**: uma instancia de uma classe pode ser usada para fornecer muitas “instancias virtuais”;
- **Facade**: simplifica a interface de um conjunto de classes;
- **Composite**: Os clientes tratam as coleções de objetos e os objetos individuais de maneira uniforme;
- **Bridge**: permite criar uma ponte para variar não apenas a sua implementação, como também as suas abstrações;
- **Adapter**: envelopa um objeto e fornece a ele uma interface diferente;


## Referências
<br>
SERRANO, Milene. **Padrões GoF**, 2021. Material apresentado na Disciplina de Arquitetura e Desenho de Software do curso de Engenharia de Software da UnB, FGA. Acesso em 10 de março de 2021.

DEVMEDIA, **Design Patterns: Padrões “GoF”**. Disponível em [https://www.devmedia.com.br/design-patterns-padroes-gof/16781](https://www.devmedia.com.br/design-patterns-padroes-gof/16781) Acesso em 4 de abril de 2021.

REFACTORING GURU, **O Catálogo dos Padrões de Projeto** Disponível em [https://refactoring.guru/pt-br/design-patterns/catalog](https://refactoring.guru/pt-br/design-patterns/catalog) Acesso em 4 de abril de 2021.
