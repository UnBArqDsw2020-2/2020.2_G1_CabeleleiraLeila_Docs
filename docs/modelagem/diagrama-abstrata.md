# <center> Diagrama de Classes
<br>
    
## Histórico de versão
|Data | Versão | Descrição | Autor(es)
| -- | -- | -- | -- |
| 07.03.2021 | 0.1 | Criação do documento e adição dos textos | Kalebe
| 08.03.2021 | 0.2 | Diagrama de classe abstrata | Kalebe, Lucas
| 08.03.2021 | 0.3 | Adiciona introdução e metodologia | Kalebe, Lucas
| 08.03.2021 | 0.4 | Adiciona descrição| Kalebe, Lucas
| 08.03.2021 | 0.4 | Revisão do documento | Erick
| 08.03.2021 | 1.0 | Revisão do documento | Lucas

## Participantes
- Kalebe Lopes
- Lucas Lopes 
- Erick Giffoni (Revisão)

<br>

## Introdução
<p align="justify">
Uma classe abstrata é uma classe que serve de modelo para outras classes. Ou seja, ela sempre será uma superclasse genérica, e suas subclasses serão mais específicas.<br>
Já a classe concreta é uma classe que possui atributos, métodos e pode ser instanciada, ou seja, permite a criação de novos objetos a partir dela. A classe concreta pode ser herdada por outras classes. 

</p>

## Metodologia
Para a criação dos diagramas, a equipe responsável se reuniu virtualmente através da ferramenta Google Meet. Além disso, utilizamos a ferramenta STAR UML, a qual fornece uma interface amigável e funcionamento adequado para diagramas.
## Diagramas

No nosso diagrama a classe **Base** é nossa classe modelo, classe abstrata, que servirá para conter informações e propriedades comuns a todas outras classes do domínio da aplicação,  ao serem persistidas através de algum **ORM**,  podemos ter a versabilidade de alterar as propriedades de identificação comum e específicas de acordo com a documentação de SGBD distintos.

**Versão 1.0**

[<div align="center"><img hight="auto" width="auto" src="../../img/modelagem/estatica/abstrata.svg"></div>](../../img/modelagem/estatica/abstrata.svg)
<figcaption align='center'>
    <b>Figura 2: Diagrama de classe abstrata - v1.0 </b>
    <br>
    <small>Autores: Kalebe e Lucas</small>
</figcaption>
<br>

## Referências
<br>

**Conceitos de Orientação a Objetos/Classe Abstrata** Disponível em: [https://pt.wikiversity.org/wiki/Conceitos_de_Orienta%C3%A7%C3%A3o_a_Objetos/Classe_Abstrata](https://pt.wikiversity.org/wiki/Conceitos_de_Orienta%C3%A7%C3%A3o_a_Objetos/Classe_Abstrata#:~:text=Al%C3%A9m%20disso%2C%20ela%20n%C3%A3o%20pode,um%20m%C3%A9todo%20abstrato%2C%20sem%20corpo.). Acesso em 8 de março de 2021.

SERRANO, Milene. **Modelagem -  Classe Concreta & Abstrata & Sobrescrita & Sobrecarga**, 2021. Vídeo-aulas complementares apresentadas na Disciplina de Arquitetura e Desenho de Software do curso de engenharia de software da UnB, FGA. Acesso em: 25 de fevereiro de 2021.

