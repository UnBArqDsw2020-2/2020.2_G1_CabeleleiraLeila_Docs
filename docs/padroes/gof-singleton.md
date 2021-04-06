# <center> GoF Singleton
<br>
    
### Histórico de versão<br>

|Data | Versão | Descrição | Autor(es)|
| -- | -- | -- | -- |
| 05.04.2021 | 0.1 | Criação do documento | Bruna Almeida<br>Damarcones Porto<br>Isabella Carneiro|
| 05.04.2021 | 1.0 | Adição do diagrama UML | Bruna Almeida<br>Damarcones Porto<br>Isabella Carneiro <br> Lucas Lopes|



### Participantes

* Bruna Almeida
* Damarcones Porto
* Isabella Carneiro
* Lucas Lopes

### Introdução
<div align="justify">
O Padrão Singleton, que pertence à categoria dos Padrões Criacionais, tem como objetivo fornecer um ponto único de acesso à instância de um objeto, de modo que qualquer local da aplicação consiga acessá-lo. Para evitar uma redundância de criação e liberação de objetos, pode-se utilizar um Singleton: O objeto da classe será criado apenas uma vez e essa mesma instância será utilizada por todos os locais que a solicitarem. O singleton garante um ponto global de acesso ao seu objeto.
<br><br>

As vantagens de usar o Padrão Singleton incluem uma redução de processamento ao criar e liberar objetos constantemente, o que contribui para o desempenho do sistema; e, por representar um único objeto, é possível compartilhar dados entre telas.
</div><br>


### Metodologia
<div align="justify">
A documentação e modelagem do padrão Singleton foi desenvolvida a partir de uma reunião com alguns integrantes, na plataforma Discord. Além disso, o diagrama UML foi desenvolvido pelos integrantes através da plataforma <a href="https://app.diagrams.net/">Draw.io</a>.
</div><br>

### Aplicação no projeto
<div align="justify">

O projeto utiliza este padrão principalmente nas funcionalidades que necessitam de um tipo de autenticação. Nos exemplos a seguir estão implementadas as classes SpringFoxConfig e JwtAuthenticationEntryPoint, que envolvem segurança de acesso.

</div><br>

<br>

[<div align="center"><img src="../../img/padroes/gofs/singleton_1.jpg"></div>](../../img/padroes/gofs/singleton_1.jpg)
<figcaption align="center">
    <b>Figura 1 - Representação da classe SpringFoxConfig.</b>
</figcaption>
<br>


[<div align="center"><img src="../../img/padroes/gofs/singleton_2.jpg"></div>](../../img/padroes/gofs/singleton_2.jpg)
<figcaption align="center">
    <b>Figura 2 - Representação da classe JwtAuthenticationEntryPoint</b>
</figcaption>

<br>

### Modelagem UML
<div align="justify">
O diagrama UML representa a forma como o padrão está sendo empregado no projeto, exemplificando o uso da SpringFoxConfig.
</div><br>

[<div align="center"><img src="../../img/padroes/gofs/uml-singleton.png"></div>](../../img/padroes/gofs/uml-singleton.png)
<figcaption align="center">
    <b>Figura 3 - Representação UML da classe JSpringFoxConfig</b>
</figcaption>

<br>

<div align="justify">

Vale lembrar que esse padrão está sendo amplamente utilizado no projeto, entretanto, para fins de explicação e para não tornar este documento longo, utilizamos apenas exemplos relacionados à classe SpringFoxConfig presente na aplicação.

</div><br>

<br>

## Referências
DEVMEDIA, **Padrão de Projeto Singleton em Java** Disponível em [https://www.devmedia.com.br/padrao-de-projeto-singleton-em-java/26392](https://www.devmedia.com.br/padrao-de-projeto-singleton-em-java/26392) Acesso em 1 de abril de 2021.

ANDRÉ CELESTINO, **[Delphi] Design Patterns GoF – Singleton**. Disponível em [https://www.andrecelestino.com/delphi-design-patterns-singleton/](https://www.andrecelestino.com/delphi-design-patterns-singleton/) Acesso em 5 de abril de 2021.

MEDIUM, **Singleton Design Pattern**. Disponível em [https://medium.com/rafaelantoniolucio/singleton-design-pattern-3e903f625265](https://medium.com/rafaelantoniolucio/singleton-design-pattern-3e903f625265) Acesso em 5 de abril de 2021.
