# <center> Chain of Responsability
<br>
    
### Histórico de versão<br>

|Data | Versão | Descrição | Autor(es)|
| -- | -- | -- | -- |
| 07.04.2021 | 0.1 | Criação do documento | Rafaella Junqueira<br>Lucas Lopes<br>Geraldo Victor<br>Kalebe Lopes|

### Participantes

* Rafaella Junqueira
* Lucas Lopes
* Geraldo Victor
* Kalebe Lopes

### Introdução
<div align="justify">
<p>O Chain of Responsibility, ou cadeia de responsabilidades, é um padrão de projeto comportamental que se baseia em transformar certos comportamentos em objetos solitários chamados handlers. Este padrão permite a passagem de pedidos por uma corrente desses handlers. Ao receber um pedido, cada handler decide se o processa ou o passa adiante para o próximo handler na corrente.</p>
<p>Nesta cadeia de responsabilidades, a principal função é evitar a dependência entre um objeto receptor e um objeto solicitante, por isso está ligado a ideia de baixo acoplamento, por permitir que outros objetos da cadeia tenham a oportunidade de tratar uma solicitação. A utilização do padrão permite determinar quem será o objeto que irá tratar a requisição durante a execução.</p>
</div>

### Metodologia
<div align="justify">
<p>A documentação do padrão GoF Chain of Responsability, assim como a modelagem do diagrama UML, foi realizada por meio de reuniões da equipe através da plataforma Discord.
</div>

### Aplicação no projeto
<div align="justify">
<p>O padrão pode ser visto, por exemplo, quando aplicado às classes UsernameIsNotEmpty e PasswordIsNotEmptyProcess, onde o comportamento do processo é direcionado para o responsável de acordo com o pedido recebido.</p>
</div>

[<div align="center"><img src="../../img/padroes/chain1.png"></div>](../../img/padroes/chain2.png)
<figcaption align='center'>
    <b>Figura 1 - Representação da classe UsernameIsNotEmpty </b>
</figcaption>
<br>

[<div align="center"><img src="../../img/padroes/chain2.png"></div>](../../img/padroes/chain2.png)
<figcaption align='center'>
    <b>Figura 2 - Representação da classe PasswordIsNotEmptyProcess</b>
</figcaption>
<br>

<!-- ### Modelagem UML

[<div align="center"><img src="../../img/padroes/"></div>](../../img/padroes/)
<figcaption align='center'>
    <b>Figura X - </b>
    <br>
    <small>Autores: Rafaella Junqueira e Lucas Lopes</small>
</figcaption>
<br> -->

## Referências
<br>
REFACTORING GURU, **Chain of Responsibility**, Disponível em [https://refactoring.guru/pt-br/design-patterns/chain-of-responsibility](https://refactoring.guru/pt-br/design-patterns/chain-of-responsibility)

