# <center> GRASP Baixo Acoplamento
<br>
### Histórico de versão<br>
|Data | Versão | Descrição | Autor(es)
| -- | -- | -- | -- |
| 25.02.2021 | 0.1 | Criação do documento | Rafaella Junqueira<br>Kalebe Lopes|
| 25.02.2021 | 0.2 | Adição do diagrama UML | Rafaella Junqueira<br>Kalebe Lopes|


### Participantes

* Rafaella Junqueira
* Kalebe Lopes
* Erick Giffoni

### Introdução
<div align="justify">

O padrão de Baixo Acoplamento é um padrão de avaliação, que determina como atribuir responsabilidades de suporte, de modo que o acoplamento entre classes permaneça baixo. A utilização deste padrão oferece benefícios como menor dependência entre as classes, redução de impacto das mudanças e aumento do potencial de reutilização das classes.
<br><br>

</div>

### Aplicação no projeto
<div align="justify">

Os códigos criados utilizam a divisão de responsabilidades entre as classes, de modo que, para a evitar a dependência entre elas, existem interfaces que abarcam os métodos comuns a todas. Assim, caso haja necessidade de mudanças, basta alterar apenas a interface.
<br><br>
As imagens abaixo exemplificam o baixo acoplamento entre a classe de serviço, ServicoService, e a interface ServicoRepository que herda a implementação dos métodos advindos da interface CrudRepository.  
</div><br>


[<div align="center"><img src="../../img/padroes/servico-repository.png"></div>](../../img/padroes/servico-repository.png)
<figcaption align='center'>
    <b>Figura 1 - Interface que implementa a interface crud</b>
</figcaption>
<br>

[<div align="center"><img src="../../img/padroes/servico-interface.png"></div>](../../img/padroes/servico-interface.png)
<figcaption align='center'>
    <b>Figura 2 - Utilização da interface ServicoRepository pela classe ServicoService</b>
</figcaption>
<br>

### Modelagem UML

<div align="justify">
Para melhor representar o funcionamento do padrão GRASP de baixo acoplamento adotado no projeto, foi modelado um diagrama UML exemplificando a utilização da interface ServiceRepository por parte da classe de serviço intitulada ServicoService.
</div>

[<div align="center"><img src="../../img/padroes/baixo-acoplamento.png"></div>](../../img/padroes/baixo-acoplamento.png)
<figcaption align='center'>
    <b>Figura 3 - Exemplo de uso de interface pela classe ServicoService</b>
    <br>
    <small>Autores: Rafaella Junqueira e Kalebe Lopes</small>
</figcaption>
<br>

## Referências
<br>

Universidade Federal de Uberlândia. **Padrões GRASPs** Disponível em [http://www.facom.ufu.br/~bacala/ESOF/05a-Padr%C3%B5es%20GRASP.pdf](http://www.facom.ufu.br/~bacala/ESOF/05a-Padr%C3%B5es%20GRASP.pdf). Acesso em 12 de março de 2021.