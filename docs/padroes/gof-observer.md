# <center> GoF Observer
<br>
    
### Histórico de versão<br>

|Data | Versão | Descrição | Autor(es)|
| -- | -- | -- | -- |
| 07.04.2021 | 0.1 | Criação do documento | Bruna Almeida<br>Damarcones Porto<br>Isabella Carneiro<br>Lucas Lopes|

### Participantes

* Bruna Almeida
* Damarcones Porto
* Isabella Carneiro
* Lucas Lopes

### Introdução
<div align="justify">

O Observer é um padrão de projeto comportamental que permite que você defina um mecanismo de assinatura para notificar múltiplos objetos sobre quaisquer eventos que aconteçam com o objeto que eles estão observando.

O padrão de projeto (Design Pattern) Observer é um padrão comportamental que representa uma relação de 1-N (de um para muitos) entre objetos. Assim quando um objeto altera o seu estado os objetos dependentes serão notificados/informados/avisados e atualizados de forma automática.

Vantagens em usar o padrão Observer:

    Permite um acoplamento mínimo entre o Sujeito(Subjet) e o Observador(Observer)

        Pode reutilizar Sujeitos sem reutilizar os seus observadores e vice-versa;
        Os Observadores podem ser adicionados sem modificar o Sujeito;
        Todo sujeito conhece a sua lista de Observadores;
        O Sujeito não precisa conhecer a classe concreta de um observador, apenas que cada observador implementa a interface update();
        O Subjeito e Observador podem pertencer a diferentes camadas de abstração;

Quando usar o padrão Observer ?

    Quando uma modificação do estado de um objeto implica modificações em outros objetos;
    Quando um objeto deve ser capaz de notificar outros objetos, mas sem pressupostos sobre os objetos a serem notificados;
    Quando uma abstração possuir dois aspectos e um depende do outro;
    Quando não desejamos um forte acoplamento com os objetos que necessitam conhecer estas modificações;

O padrão Observer funciona como assinaturas de jornais e revistas, ou seja, temos uma editora que publica as edições e pessoas que assinam os jornais ou revistas dessa editora e sempre recebem as novas edições assim que elas são publicadas. Enquanto a pessoa é assinante ela continua recebendo as edições na sua casa. Se a pessoa cancelar a assinatura do jornal ou da revista ela para de receber as edições.

O padrão Observer funciona da mesma forma, no entanto, tem-se que a editora (que publica) é o chamado SUBJECT no Padrão Observer e os assinantes (que recebem as novas publicações) são os chamados OBSERVER.

Os OBSERVERs registram-se no SUBJECT para receber atualizações quando os dados do SUBJECT são alterados. Os OBSERVERs também podem cancelar o seu registro e dessa forma não receber mais nenhuma atualização do SUBJECT.


<br><br>



<br><br>



<br><br>

</div><br>

### Metodologia

<div align="justify">
A documentação e modelagem do padrão Observer foi desenvolvida a partir de uma reunião com alguns integrantes, na plataforma Discord. Além disso, o diagrama UML foi desenvolvido pelos integrantes através da plataforma <a href="https://app.diagrams.net/">Draw.io</a>.
</div><br>

### Aplicação no projeto
<div align="justify">


</div> <br>

### Modelagem UML
<div align="justify">

</div> <br>

### Referências


