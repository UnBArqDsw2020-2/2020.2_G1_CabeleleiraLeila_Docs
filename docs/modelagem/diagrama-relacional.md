# <center> Diagrama Relacional
<br>

### Histórico de versão

|Data | Versão | Descrição | Autor(es)
| -- | -- | -- | -- |
| 07.03.2021 | 0.1 | Criação do documento | Erick Giffoni |

### Participantes

* Erick Giffoni 
* Kalebe Lopes
 

## Introdução
<div align="justify">
to-do 
</div><br>

## Metodologia
<div align="justify">

to-do
</div><br>

## Modelo Entidade-Relacionamento (ME-R)
<br>

Tendo como referência o nosso Diagrama de Classes e nosso Diagrama de Agregação e Composição, temos:

### Entidades

- PESSOA <br>
- AUTENTICACAO <br>
- SERVICO <br>
- CLIENTE <br>
- PEDIDO <br>
- FUNCIONARIO <br>
- ESPECIALIDADE <br>

### Atributos 

- PESSOA (<u>idPessoa</u>, <u>emailAutenticacao</u>, nome, dataNascimento, telefone, cpf) <br>

- AUTENTICACAO (<u>login</u>, senha, email, {permissao}) <br>

- SERVICO (<u>idServico</u>, descricao, valor) <br>

- CLIENTE (idCliente, {interesses}, observacao) <br>

- PEDIDO (idPedido, valor, data, confirmado, atendimento) <br>

- FUNCIONARIO (idFuncionario, diaDisponivel, turnoAtendimento, foto) <br>

- ESPECIALIDADE (idEspecialidade, nome, descricao) <br>

 
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
<br>
to-do

## Diagrama Lógico de Dados (DLD)
<br>
to-do


## Referências
<br>

PRESSMAN, Roger S. **Engenharia de Software: uma abordagem profissional.** 7a edição, Porto Alegre, AMGH, 2011.

RISSOLI, Vandor Roberto Vilardi. **Sistemas de Bancos de Dados.** Disciplina ministrada<br>
na Universidade de Brasília para o curso de Engenharia de Software.