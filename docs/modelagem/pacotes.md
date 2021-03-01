# <center>Diagrama de Pacotes
<br>

### Histórico de versão

|Data | Versão | Descrição | Autor(es)
| -- | -- | -- | -- |
| 01.03.2021 | 0.1 | Criação do documento | Isabella Carneiro|
| 01.03.2021 | 0.2 | Adição da introdução| Rafaella Junqueira|
| 01.03.2021 | 0.3 | Adição da metodologia | Rafaella Junqueira |

### Participantes
* Isabella Carneiro
* Rafaella Junqueira

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
A modelagem do diagrama de pacotes deste projeto foi realizada utilizando a ferramenta [Lucidchart](https://www.lucidchart.com/pages/pt) e consiste em representar apenas a relação de dependência em termos de uso e de acesso das classes, conforme podem ser acessadas no documento de [Diagrama de Classes](modelagem/classes.md).
<br><br>
A primeira versão do diagrama foi realizada de forma remota com a contribuição dos integrantes feita de forma escrita. Posteriormente, foi realizada uma reunião entre os integrantes para discussão do que fora modelado e prposição de melhorias para o diagrama, dando origem à versão final do artefato. 


### Resultado
<!-- <div align="justify"> -->
    
<!-- </div><br> -->

### Referências 
<br>
SERRANO, Milene. **Modelagem - Diagrama de Pacotes**, 2021. Material apresentado na Disciplina de Arquitetura e Desenho de Software do curso de engenharia de software da UnB, FGA. Acesso em: 01 de março de 2021.

RIBEIRO, Antônio. **Glossário UML - Diagrama de Pacotes**, 2021. Disponível em: [https://homepages.dcc.ufmg.br/~amendes/GlossarioUML/glossario/conteudo/pacotes/diagrama_de_pacotes.html](https://homepages.dcc.ufmg.br/~amendes/GlossarioUML/glossario/conteudo/pacotes/diagrama_de_pacotes.html) Acesso em: 01 de merço de 2021.

Lucidchart. **Tudo sobre diagramas de pacotes UML**. Disponível em: [https://www.lucidchart.com/pages/pt/diagrama-de-pacotes-uml](https://www.lucidchart.com/pages/pt/diagrama-de-pacotes-uml) Acesso em: 01 de março de 2021.