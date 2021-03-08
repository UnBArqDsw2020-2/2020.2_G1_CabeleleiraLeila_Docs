# <center> Diagrama de Agregação e Composição
<br>

## Histórico de versão
|Data | Versão | Descrição | Autor(es)
| -- | -- | -- | -- |
| 26.02.2021 | 0.1 | Criação do documento | Erick Giffoni|
| 26.02.2021 | 0.2 | Adiciona a metodologia utilizada | Erick Giffoni|
| 26.02.2021 | 0.3 | Adiciona o diagrama na versão 1 | Erick Giffoni, Lucas Lopes|
| 26.02.2021 | 1.0 | Apresentação do resultado obtido na primeira versão| Erick Giffoni|
| 01.03.2021 | 1.1 | Reestrutura o documento com Introdução| Erick Giffoni|
| 01.03.2021 | 1.2 | Revisão e padronização do documento | Rafaella Junqueira |
| 03.03.2021 | 1.2 | Revisão do documento | Isabella Carneiro |

### Participantes

* Erick Giffoni
* Lucas Lopes Pereira
* Rafaella Junqueira (Revisão)
* Isabella Carneiro (Revisão)
<br>

## Introdução
<div align="justify"><br>

O Diagrama de Agregação e Composição representa como as diferentes classes de um projeto de software se relacionam. Dessa forma, ele se parece com a representação de relacionamentos entre entidades de um banco de dados, por exemplo, por meio do diagrama de entidade-relacionamento.

O foco não é mostrar com detalhes os métodos e os atributos de cada classe, mas sim deixar claro como elas se comunicam, como dependem umas das outras etc. Assim, ficam visíveis aspectos como modularidade, coesão e acoplamento.
</div><br>

## Metodologia
<br>
Para realizar esse diagrama para o projeto do sistema do Salão da Leila, nossa equipe baseou-se no Diagrama de Classes que fora previamente projetado. Houve uma renião virtual na qual nós fizemos a diagramação completa das agregações e das composições entre as classes existentes no referido projeto. O diagrama foi realizada utilizando a ferramenta [Diagrams.net](https://www.diagrams.net).<br>


## Resultado
<br>
Do que se trata esse Diagrama? A ideia é mostrar como as diferentes classes do sistema para o Salão da Leila se comportam entre si. Lembrando que tais classes foram previamente projetadas no [Diagrama de Classes](./diagrama-de-classes.md).

Veja abaixo como ficou a primeira versão desse diagrama em notação UML:
<br>

[<div align="center"><img width="auto" height="auto" src="../../img/modelagem/estatica/agregacao-composicao/diagramaAgregacaoComposicao.jpg"/></div>](../img/modelagem/estatica/agregacao-composicao/diagramaAgregacaoComposicao.jpg)

<figcaption align='center'>
    <b>Figura 1: Diagrama de Agregação e Composição</b>
    <br>
    <small>Autores: Erick Giffoni e Lucas Lopes Pereira</small>
</figcaption>
<br>

Para acesso do diagrama em nuvem, clique em [Diagrama de Agregação e Composição - v1](https://unbbr-my.sharepoint.com/:i:/g/personal/160010900_aluno_unb_br/EcwQ-rqfxWpKpvmscK5laT4BH3og0hySa9Y5mS5UDzF8eg?e=5BK3JS)

Nessa primeira versão, todas as classes que possuem alguma relação de agregação e/ou composição estão presentes no Diagrama. Tomemos como exemplo a classe 'Pedido'. Esta é composta por pelo menos 1 (um) 'Serviço', e é composta por somente 1 (um) 'Cliente'. 

Além disso, um 'Pedido' é agregado a 0 (zero) ou 1 (um) 'Funcionário', e essa mesma regra equivale para 'Horário'. Vale ressaltar que o Diagrama apresentado aqui pode sofrer modificações ao longo do projeto.

## Referências
<br>

PRESSMAN, Roger S. **Engenharia de Software: uma abordagem profissional.** 7a edição, Porto Alegre, AMGH, 2011.

SOMMERVILLE, Ian. **Engenharia de Software.** 9a edição, São Paulo, Pearson, 2011.

SERRANO, Milene. **Modelagem - Diagrama de Agregação e Composição**, 2021. Vídeo-aulas complementares apresentadas na Disciplina de Arquitetura e Desenho de Software do curso de engenharia de software da UnB, FGA. Acesso em: 26 de fevereiro de 2021.

