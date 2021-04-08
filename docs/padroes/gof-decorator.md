# <center> GoF Decorator
<br>
    
### Histórico de versão<br>

|Data | Versão | Descrição | Autor(es)|
| -- | -- | -- | -- |
| 07.04.2021 | 0.1 | Criação do documento | Isabella Carneiro<br>Damarcones Porto<br>Bruna Almeida<br>Lucas Lopes<br>Rafaella Junqueira<br>
| 07.04.2021 | 1.0 | Adição do diagrama UML |Isabella Carneiro<br>Damarcones Porto<br>Bruna Almeida<br>Lucas Lopes Rafaella Junqueira<br>|

### Participantes

* Isabella Carneiro
* Bruna Almeida
* Rafaella Junqueira
* Damarcones Porto
* Lucas Lopes

### Introdução
<div align="justify">

O Padrão Decorator anexa responsabilidades adicionais a um objeto dinamicamente. Os decoradores fornecem uma alternativa flexível de subclasse para estender a funcionalidade
<br><br>
</div><br>

### Metodologia
<div align="justify">

A documentação deste padrão foi realizada em conjunto por meio de reunião virtual utilizando a plataforma Discord e para a modelagem utilizou-se a ferramenta <a href = "https://www.lucidchart.com">Lucidchart</a>.

</div><br>

### Aplicação no projeto
<div align="justify">

No trecho de código a seguir podemos notar algumas aplicações do padrão Decorator no projeto, como por exemplo o @RestController que utiliza um Decorator para transformar os dados vindo via http para o formato aplicattion/json e retorna json em suas respostas.
Temos também o @RequestMapping que faz o mapeamento das rotas, @Autowired que marca um campo que será uma instancia gerenciada pelo sistema do spring e o @PostMapping que é uma notação utilizada para mapear verbos no http do tipo POST.


</div><br>

[<div align="center"><img src="../../img/padroes/gofs/gof-decorator.png"></div>](../../img/padroes/gof/gof-decorator.png)
<figcaption align='center'>
    <b>Figura 1 - Representação do padrão Decorator</b>
</figcaption>
<br>

### Modelagem UML

<div align="justify">

O diagrama UML representa a forma como o padrão está sendo empregado no projeto, exemplificando o uso do @RequestMapping

</div><br>

[<div align="center"><img src="../../img/padroes/gofs/gof-decorator2.png"></div>](../../img/padroes/gof/gof-decorator2.png)
<figcaption align='center'>
    <b>Figura 2 - Representação do RequestMapping</b>
    <br>
    <small>Autores: Isabella Carneiro</small>
</figcaption>
<br>

## Referências

DevMedia, **Padrão de Projeto Decorator em Java**. Disponível em [https://www.devmedia.com.br/padrao-de-projeto-decorator-em-java/26238](https://www.devmedia.com.br/padrao-de-projeto-decorator-em-java/26238)
