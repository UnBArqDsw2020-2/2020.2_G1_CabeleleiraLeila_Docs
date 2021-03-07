# <center>Diagrama de Pacotes
<br>

### Histórico de versão

|Data | Versão | Descrição | Autor(es)
| -- | -- | -- | -- |
| 01.03.2021 | 0.1 | Criação do documento | Isabella Carneiro |
| 01.03.2021 | 0.2 | Adição da introdução | Rafaella Junqueira |
| 01.03.2021 | 0.3 | Adição da metodologia | Rafaella Junqueira |
| 02.03.2021 | 0.4 | Adição do diagrama de pacotes Backend | Rafaella Junqueira, Lucas Lopes,<br>Isabella Carneiro, Geraldo Victor,<br>Kalebe Lopes |
| 04.03.2021 | 0.4 | Revisão do documento e sugestão de mudanças | Erick Giffoni |

### Participantes
* Isabella Carneiro
* Rafaella Junqueira
* Lucas Lopes Pereira
* Geraldo Victor
* Kalebe Lopes
* Erick Giffoni (Revisão)

### Introdução
<div align="justify"><br>
Um Diagrama de Pacotes atua como complemento do Diagrama de Classes, tratando-se de um diagrama estático que permite organizar o sistema como se representasse uma visão em módulos. Um diagrama de pacotes é composto de pacotes e relacionamentos entre pacotes, ou seja, é a representação de um grupo de classes ou outros elementos que se relacionam uns com os outros através de uma relação de dependência.
<br><br>
O pacote é um meio disponibilizado pela UML para organizar os diversos elementos ou modelos em grupos e nele podem ser incluídas classes, interfaces, componentes, diagramas ou até outros pacotes. Já a relação de dependência indica que um item depende da especificação de outro item. Essa relação entre pacotes pode ser classificada em cinco tipos de dependência:<br><br>
</div>

- **Uso:** um pacote/elemento precisa de outro para ter sua definição e implementação completa;
- **Acesso:** um pacote necessita acessar as funções de outro pacote;
- **Importação:** funcionalidade importada de um pacote para outro;
- **Abstração:** relaciona dois elementos que representam a mesma ideia mas em níveis de abstração diferentes;
- **Disponibilização:** mostra a implementação de um artefato em um alvo de implementação.

<div align="justify">

Diagramas de pacotes são interessantes pois fornecem uma visão clara da estrutura hierárquica dos variados elementos UML dentro de um determinado sistema. Esses diagramas podem simplificar diagramas de classes complexos, criando elementos visuais organizados. 
</div><br>

### Metodologia
<br>
<div align="justify">

A modelagem do diagrama de pacotes deste projeto foi realizada utilizando a ferramenta [Lucidchart](https://www.lucidchart.com/pages/pt) durante a reunião entre os integrantes do grupo, e consiste em representar a relação de dependência em termos de uso, acesso e importação de pacotes. A diagramação foi feita seguindo princípios de arquitetura limpa e boas práticas utilizadas para separação de pacotes em aplicações comerciais.
</div>

### Diagrama de Pacotes
<br>

<!-- **Diagrama v2** -->

<!-- [<div align="center"><img src="../../img/modelagem/estatica/NOMEDAIMAGEM"></div>](../../img/modelagem/estatica/NOMEDAIMAGEM)
<figcaption align='center'>
    <b>Figura 1 - </b>
    <br>
    <small>Autores: </small>
</figcaption>
<br> -->

**Diagrama v1**

[<div align="center"><img src="../../img/modelagem/estatica/pacotes-backend.svg"></div>](../../img/modelagem/estatica/pacotes-backend.svg)
<figcaption align='center'>
    <b>Figura 2 - Diagrama de Pacotes Backend</b>
    <br>
    <small>Autores: Rafaella Junqueira, Lucas Lopes, Isabella Carneiro, Geraldo Victor, Kalebe Lopes</small>
</figcaption>
<br>


### Referências 
<br>
SERRANO, Milene. **Modelagem - Diagrama de Pacotes**, 2021. Material apresentado na Disciplina de Arquitetura e Desenho de Software do curso de engenharia de software da UnB, FGA. Acesso em: 01 de março de 2021.

RIBEIRO, Antônio. **Glossário UML - Diagrama de Pacotes**, 2021. Disponível em: [https://homepages.dcc.ufmg.br/~amendes/GlossarioUML/glossario/conteudo/pacotes/diagrama_de_pacotes.html](https://homepages.dcc.ufmg.br/~amendes/GlossarioUML/glossario/conteudo/pacotes/diagrama_de_pacotes.html) Acesso em: 01 de merço de 2021.

Lucidchart. **Tudo sobre diagramas de pacotes UML**. Disponível em: [https://www.lucidchart.com/pages/pt/diagrama-de-pacotes-uml](https://www.lucidchart.com/pages/pt/diagrama-de-pacotes-uml) Acesso em: 01 de março de 2021.
