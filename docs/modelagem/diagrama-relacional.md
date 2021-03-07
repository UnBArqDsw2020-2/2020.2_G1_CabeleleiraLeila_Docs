# <center> Diagrama Relacional
<br>

### Histórico de versão

|Data | Versão | Descrição | Autor(es)
| -- | -- | -- | -- |
| 07.03.2021 | 0.1 | Criação do documento | [Erick Giffoni](https://github.com/ErickGiffoni) |
| 07.03.2021 | 0.2 | Adição dos diagramas | [Kalebe Lopes](https://github.com/KalebeLopes) |
| 07.03.2021 | 1.0 | Adição da introdução, metodologia e comentários  | [Erick Giffoni](https://github.com/ErickGiffoni), <br> [Kalebe Lopes](https://github.com/KalebeLopes) |


### Participantes

* Erick Giffoni 
* Kalebe Lopes
 

## Introdução

É fundamental que um bom projeto de engenharia de software tenha um bom projeto de<br>
banco de dados. Nesse sentido, aqui apresentamos o ME-R, o DE-R e o DLD para o sistema<br>
do salão da Leila. <br>

ME-R, ou Modelo Entidade-Relacionamento, representa nosso banco de dados em um nível<br>
conceitual. Nele trazemos as representações de nossas entidades, os atributos de cada<br>
uma delas e, por fim, cada relacionamento existente entre as entidades.<br>

DE-R, ou Diagrama Entidade-Relacionamento, baseia-se no ME-R e traz uma representação,<br>
no formato de diagrama, sobre as entidades, os atributos e os relacionamentos. Esse diagrama<br>
fornece uma visão um pouco mais próxima do nível lógico.<br>

DLD, ou Diagrama Lógico de Dados, serve para especificar a um nível mais lógico as entidades,<br>
cada atributo com seus tipos (literal, inteiro, por exemplo), bem como os relacionamentos<br>
e as chaves de cada entidade - primárias ou estrangeiras.


<br>

## Metodologia
Utilizamos o Microsoft Word Online como ferramenta colaborativa para projetarmos o ME-R. O nosso time também fez reuniões para alinharmos as ideia e para trabalarmos em conjunto. <br> 
Já para a construção do DE-R e do DLD, escolhemos a ferramenta CASE brModelo, a qual fornece funcionamento adequado para isso. Mais ainda, em um momento inicial, a ferramenta whimsical também foi utilizada para o DE-R.

<br>

## Modelo Entidade-Relacionamento (ME-R)
<div align="justify">
Tendo como referência o nosso <a href="../classes"> Diagrama de Classes</a> e nosso <a href="../agregacao-composicao"> Diagrama de Agregação e Composição</a>, temos:
</div>

<br>

### Entidades

- PESSOA <br>
- AUTENTICACAO <br>
- SERVICO <br>
- CLIENTE <br>
- PEDIDO <br>
- FUNCIONARIO <br>
- ESPECIALIDADE <br>

### Atributos 

- PESSOA (<u>idPessoa</u>, <u>emailAutenticacao</u>, login, nome, dataNascimento, telefone, cpf) <br>

- AUTENTICACAO (<u>login</u>, senha, email, {permissao}) <br>

- SERVICO (<u>idServico</u>, descricao, valor) <br>

- CLIENTE (<u>idCliente</u>, emailAutenticacao, idPessoa, {interesses}, observacao) <br>

- PEDIDO (<u>idPedido</u>, idCliente, valor, data, confirmado) <br>

- FUNCIONARIO (<u>idFuncionario</u>, emailAutenticacao, idPessoa, diaDisponivel, turnoAtendimento, foto) <br>

- ESPECIALIDADE (<u>idEspecialidade</u>, idFuncionario nome, descricao) <br>

 
### Relacionamentos 
<br>

- PESSOA - tem - AUTENTICACAO 

      - Uma PESSOA faz uma AUTENTICACAO para usar a aplicação do Salão da Leila, e uma AUTENTICACAO é feita por uma PESSOA. <br>
      - Cardinalidade: 1:1 <br>

<br>

- PEDIDO - tem - SERVICO 

      - Um PEDIDO tem um ou mais SERVICO, e SERVICO pode estar relacionado a nenhum ou a vários PEDIDO. <br>
      - Cardinalidade: M:N <br>

<br>

- CLIENTE - faz - PEDIDO 

      - Um CLIENTE faz um ou vários PEDIDO, e um PEDIDO é feito por  apenas um cliente. <br>
      - Cardinalidade: 1:N <br>

<br>

- FUNCIONARIO  - realiza - PEDIDO 

      - Um FUNCIONARIO realiza nenhum ou vários PEDIDOS, e um PEDIDO é realizado por um ou vários FUNCIONARIOS <br>
      - Cardinalidade: M:N <br>

<br>

- FUNCIONARIO – possui –  ESPECIALIDADE 

      - Um FUNCIONARIO possui uma ou várias ESPECIALIDADES, e uma ESPECIALIDADE pertence a somente um FUNCIONARIO. <br>
      - Cardinalidade: N:M <br>

<br>

## Diagrama Entidade-Relacionamento (DE-R)

Para conseguirmos visualizar melhor o que fora definido anteriormente no ME-R, realizamos o DE-R para o sistema do salão da Leila, o qual encontra-se abaixo. Nele ficam visíveis as entidades, cada atributos delas, e os relacionamentos.


[![der](https://user-images.githubusercontent.com/44823367/110247730-75786a80-7f4c-11eb-85fd-35f4ef9cd6dd.jpg)](https://user-images.githubusercontent.com/44823367/110247730-75786a80-7f4c-11eb-85fd-35f4ef9cd6dd.jpg)
 
Tomemos como exemplo a entidade FUNCIONARIO, que é uma especialização da entidade PESSOA, ou seja, contém todos os atributos de PESSOA, além dos atributos específicos de um funcionário. <br><br>
O sistema do salão da leila funciona com base nos PEDIDOs. Dessa forma, o CLIENTE faz um ou vários PEDIDOs enquanto o FUNCIONARIO realiza esse(s) pedido(s).

## Diagrama Lógico de Dados (DLD)
<br>
O próximo passo a ser feito para projetarmos o banco de dados, após a realização do DE-R, é o Diagrama Lógico de Dados. Nele são mostrados mais detalhes à respeito das entidades, das chaves primárias e estrangeiras, dos atributos, relacionamentos etc. Veja abaixo o DLD para o sistema do salão da Leila.
<br><br>
[![der](https://user-images.githubusercontent.com/44823367/110247767-9ccf3780-7f4c-11eb-9d49-2fb22cd4afc7.jpg)](https://user-images.githubusercontent.com/44823367/110247767-9ccf3780-7f4c-11eb-9d49-2fb22cd4afc7.jpg)

O Diagrama Lógico de Dados representa todas as tabelas que serão implementadas no banco de dados. Ele especifica os atributos e chaves estrangeiras de cada tabela, além de informar sua cardidalidade.<br><br>
Tomemos como exemplo a tabela cliente que se relaciona com a tabela pedido. Por meio da chave primária do CLIENTE, a qual é repassada para o PEDIDO, conseguimos recuperar todos os PEDIDOs que determinado CLIENTE solicitou. 

## Referências
<br>

PRESSMAN, Roger S. **Engenharia de Software: uma abordagem profissional.** 7a edição, Porto Alegre, AMGH, 2011.

RISSOLI, Vandor Roberto Vilardi. **Sistemas de Bancos de Dados.** Disciplina ministrada<br>
na Universidade de Brasília para o curso de Engenharia de Software.