# <center> GoF Abstract Factory
<br>
    
### Histórico de versão<br>

|Data | Versão | Descrição | Autor(es)|
| -- | -- | -- | -- |
| 01.04.2021 | 0.1 | Criação do documento | Rafaella Junqueira<br>Isabella Carneiro |
| 01.04.2021 | 1.0 | Adição do diagrama UML | Rafaella Junqueira<br>Erick Giffoni |

### Participantes

* Rafaella Junqueira
* Isabella Carneiro
* Erick Giffoni

### Introdução
<div align="justify">

O Abstract Factory é um padrão que permite a criação de famílias de objetos relacionados ou dependentes por meio de uma única interface e sem que a classe concreta seja especificada. O objetivo deste padrão é isolar a criação de objetos de seu uso e criar famílias de objetos relacionados sem ter que depender de suas classes concretas,  permitindo a introdução de novos tipos derivados sem que haja alteração ao código da classe base.
<br><br>
Essa prática ajuda a excluir a dependência entre o cliente e a classe dos objetos usados por ele. Este padrão é usado quando se deseja fornecer uma biblioteca de classes e revelar sua interface mas não sua implementação, assim, não permite-se que objetos sejam diretamente criados com new.
</div><br>

### Metodologia
<div align="justify">

A documentação deste padrão foi realizada em conjunto por meio de reunião virtual utilizando a plataforma Discord e para a modelagem utilizou-se a ferramenta <a href = "https://www.lucidchart.com">Lucidchart</a>.

</div><br>

### Aplicação no projeto
<div align="justify">

O projeto utiliza diversas interfaces que derivam de uma interface principal denominada CrudRepository, e como exemplo disso, há a interface PessoaRepository. Deste modo, entende-se que a PessoaRepository representa a fábrica astrata enquanto a CrudRepository representa a fábrica concreta.
</div><br>

[<div align="center"><img src="../../img/padroes/pessoa-repository.png"></div>](../../img/padroes/pessoa-repository.png)
<figcaption align='center'>
    <b>Figura 1 - Representação de PessoaRepository herdando CrudRepository</b>
</figcaption>
<br>

<div align="justify">
Dada a organização de pastas da aplicação, garante-se que os arquivos do tipo service interagem com as fábricas abstratas, no caso representado, com a PessoaRepository.
</div><br>

[<div align="center"><img src="../../img/padroes/pessoa-service.png"></div>](../../img/padroes/pessoa-service.png)
<figcaption align='center'>
    <b>Figura 2 - Representação de PessoaService interagindo com PessoaRepository</b>
</figcaption>
<br>

### Modelagem UML

<div align="justify">

O diagrama UML representa a forma como o padrão está sendo empregado no projeto, exemplificando o uso da PessoaRepository por meio da PessoaSerice. No diagrama, a CrudRepository representa o que seria a fábrica concreta, a PessoaRepository a fábrica abstrata e a PessoaService atua como cliente. A modelagem foi feita apenas para fins de entendimento, deste modo, os atributos e métodos da classe foram suprimidos.

</div><br>

[<div align="center"><img src="../../img/padroes/uml-gof-abstract.png"></div>](../../img/padroes/uml-gof-abstract.png)
<figcaption align='center'>
    <b>Figura 3 - Representação da fábrica abstrata e da fábrica concreta</b>
    <br>
    <small>Autores: Rafaella Junqueira e Erick Giffoni</small>
</figcaption>
<br>
<div align="justify">

Vale lembrar que esse padrão está sendo amplamente utilizado no projeto, entretanto, para fins de explicação e para não tornar este documento longo, utilizamos apenas exemplos relacionados à classe Pessoa presente na aplicação.
</div><br>

## Referências

DevMedia, **Entendendo os conceitos dos Padrões de Projetos em Java**. Disponível em [https://www.devmedia.com.br/entendendo-os-conceitos-dos-padroes-de-projetos-em-java/29083](https://www.devmedia.com.br/entendendo-os-conceitos-dos-padroes-de-projetos-em-java/29083)

Refactoring Guru, **Abstract Factory**. Disponível em [https://refactoring.guru/pt-br/design-patterns/abstract-factory](https://refactoring.guru/pt-br/design-patterns/abstract-factory) Acesso em 01 de abril de 2021.