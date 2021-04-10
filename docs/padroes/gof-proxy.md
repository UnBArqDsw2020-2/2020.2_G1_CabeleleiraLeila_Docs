# <center> GoF Proxy
<br>
    
### Histórico de versão<br>

|Data | Versão | Descrição | Autor(es)|
| -- | -- | -- | -- |
| 09.04.2021 | 0.1 | Criação do documento | Bruna Almeida<br>Damarcones Porto<br>Isabella Carneiro<br>Lucas Lopes|
| 09.04.2021 | 1.0 | Adição do diagrama UML | Bruna Almeida<br>Damarcones Porto<br>Isabella Carneiro <br> Lucas Lopes|

### Participantes

* Bruna Almeida
* Damarcones Porto
* Isabella Carneiro
* Lucas Lopes

### Introdução
<div align="justify">
O Proxy é um padrão Estrutural, com o objetivo principal de encapsular um objeto através de um outro objeto que possui a mesma interface, de forma que o segundo objeto, conhecido como “Proxy”, controla o acesso ao primeiro, que é o objeto real.
<br><br>

A principal vantagem de utilizar o Proxy é que, ao utilizar um substituto, podemos fazer desde operações otimizadas até proteção do acesso ao objeto. No entanto isto também pode ser visto como um problema, pois, como a responsabilidade de um proxy não é bem definida é necessário conhecer bem seu comportamento para decidir quando utilizá-lo ou não.
</div><br>


### Metodologia

<div align="justify">
A documentação e modelagem do padrão GoF Proxy foi desenvolvida a partir de uma reunião com alguns integrantes, na plataforma Discord.
</div><br>

### Aplicação no projeto
<div align="justify">


</div> <br>

[<div align="center"><img src="../../img/padroes/gofs/gof-proxy-1.png"></div>](../../img/padroes/gofs/gof-proxy-1.png.png)
<figcaption align="center">
    <b>Figura 1 - Representação da classe CustomErrorResponse.</b>
</figcaption>
<br>

[<div align="center"><img src="../../img/padroes/gofs/gof-proxy-2.png"></div>](../../img/padroes/gofs/gof-proxy-2.png)
<figcaption align="center">
    <b>Figura 2 - Representação da classe ExceptionAdvice.</b>
</figcaption>
<br>



### Referências

DEVMEDIA, Conheça o Pattern Proxy - GoF (Gang of Four). Disponível em: [devmedia.com.br/conheca-o-pattern-proxy-gof-gang-of-four/4066](https://www.devmedia.com.br/conheca-o-pattern-proxy-gof-gang-of-four/4066). Acesso em 9 de abril de 2021.

BRIZENO, Proxy. Disponível em: [brizeno.wordpress.com/category/padroes-de-projeto/proxy/](https://brizeno.wordpress.com/category/padroes-de-projeto/proxy/). Acesso em 9 de abril de 2021.

PADRÕES DE PROJETO IFC, Padrão Proxy. Disponível em: [padroesdeprojetoifc.wordpress.com/2016/11/30/padrao-proxy/](https://padroesdeprojetoifc.wordpress.com/2016/11/30/padrao-proxy/). Acesso em 9 de abril de 2021.