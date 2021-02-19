# <center> Entrevista

### Histórico de versão
|Data | Versão | Descrição | Autor(es)
| -- | -- | -- | -- |
| 16.02.2021 | 0.1 | Criação do documento | [Kalebe Lopes](https://github.com/KalebeLopes), [Rafaella Junqueira](https://github.com/RafaellaJunqueira)|
| 17.02.2021 | 0.2 | Adição das perguntas | [Kalebe Lopes](https://github.com/KalebeLopes)|
| 17.02.2021 | 0.3 | Refatoração do documento | [Rafaella Junqueira](https://github.com/RafaellaJunqueira)|
| 18.02.2021 | 0.4 | Adição da entrevista 1 | [Kalebe Lopes](https://github.com/KalebeLopes)|
| 18.02.2021 | 0.5 | Adição da entrevista 2 | [Rafaella Junqueira](https://github.com/RafaellaJunqueira)|


## Introdução
<div align="justify">
A entrevista é uma técnica simples e direta para realizar a coleta de informações importantes sobre determinado assunto. A comunicação entre as partes interessadas é feita para determinar quais são os requisitos necessários para o desenvolvimento do sistema. 
<br><br>
As entrevistas possibilitam a coleta de informações qualitativas e podem ser classificadas como fechadas ou abertas. As entrevistas do tipo fechadas são baseadas em um conjunto pré-existente de perguntas, enquanto as do tipo abertas não têm um script predefinido, adaptando-se de acordo com o conhecimento do entrevistado.
<br><br>
De acordo com Barbosa e Silva (2010), entrevistas permite ao avaliador coletar dados detalhados e profundos das experiências individuais do grupo de foco. Essa abordagem permite a coleta de muitas informações e possui um formato flexível, que facilita o direcionamento da coleta de dados de acordo com o cenário do usuário
</div><br>

## Metodologia
<p align="justify">
Para entrevista desta fase do projeto, optamos por seguir o modelo de entrevista fechada, onde serão feitas várias perguntas pré-definidas com o objetivo de extrair dos stakeholders o máximo de informações importantes para o sistema.
<br><br> 
As perguntas foram listadas de acordo com os interesses dos entrevistadores a fim de conduzir o stakeholder no decorrer da entrevista e possibilitar uma futura comparação entre as respostas. Dado que o intuito desta entrevista é entender a visão dos prestadores de serviços da área de tratamentos de beleza, os participantes selecionados foram aqueles que encaixam-se no perfil de proprietários de estabelecimento de beleza, e não no perfil de cliente.
</p>
Foram acordados data e horário para as entrevistas, esclarecido seu propósito e como ela seria executada. Após o esclarecimento dos detalhes da pesquisa, foi apresentado um [Termo de Consentimento](../img/termo-consentimento.png) e, caso o participante estivesse de acordo, a entrevista era iniciada

<br>

## Perguntas

Número | Pergunta |
:--: | -- |
1 | Qual o nome do estabelecimento e localização? 
2| Quantas pessoas trabalham no estabelecimento? 
3| Quais os serviços prestados? 
4| Qual é a quantidade aproximada de clientes/mês? 
5| Os funcionários costumam ficar muito tempo no dia sem serviços agendados? 
6| Se a resposta anterior foi “sim”, em quais dias e horários isso ocorre com mais frequência?
7| Qual é o tempo médio de espera para ser atendido? 
8| Como é feito o registro de um serviço prestado?
10| Já houve erro do profissional ao executar um serviço? Se sim, qual foi o motivo?
11| Os clientes costumam escolher e esperar atendimento de algum profissional específico?  
12| Já aconteceu de clientes fazerem fila para serem atendidos? 
13| Se a resposta anterior foi “sim”, quantos clientes formaram a fila? Qual foi o tempo médio de atendimento?  
14| Algum cliente já saiu frustrado por ter que esperar muito tempo para ser atendido?
15| Atualmente, qual é a ordem de atendimento ao cliente? 
16| Existe alguém responsável por fazer a distribuição dos clientes entre os profissionais disponíveis? 
17| O estabelecimento já possui sistema de agendamento? Se sim, como funciona? 
18| O que não pode faltar em um sistema de agendamento? 
<br>

## Resultado das entrevistas
<br>

#### [Entrevista 1 - Elder Araújo dos Santos, 24 anos](entrevista1.md)
#### [Entrevista 2 - Mila Junia Silva](entrevista2.md)
<br>

## Requisitos elicitados
<br>

##### Legenda
| Abreviação | Significado |
|:---------: | --------- |
| EN         | Entrevista |
| BS         | Brainstorming |

<br>

| Número | Requisito |
|:-----: | --------- |
|EN01, [BS04](../base/brainstorming.md#requisitos-elicitados) | O visitante deve ser capaz de consultar horários e dias disponíveis |
|EN02, [BS06](brainstorming.md#requisitos-elicitados) | O visitante deve ser capaz ver a lista de funcionários |
|EN03, [BS08](brainstorming.md#requisitos-elicitados) | O visitante deve ser capaz de visualisar perfil do funcionário |
|EN04, [BS11](brainstorming.md#requisitos-elicitados) | O cliente deve poder receber e enviar notificação de atraso no agendamento |
|EN05, [BS12](brainstorming.md#requisitos-elicitados) | O cliente pode solicitar um agendamento ou reagendar um horário |
|EN06, [BS14](brainstorming.md#requisitos-elicitados) | O cliente pode solicitar um agendamento ou reagendar um horário |
|EN07, [BS15](brainstorming.md#requisitos-elicitados) | O administrador deve ser capaz de cadastrar serviços |
|EN08, [BS18](brainstorming.md#requisitos-elicitados) | O sistema deve ser capaz de gerenciar os serviços de filas de atendimento por funcionário |
|EN09, [BS20](brainstorming.md#requisitos-elicitados) | O sistema deve ser capaz de calcular o tempo de uma ordem de serviço |
|EN10, [BS22](brainstorming.md#requisitos-elicitados) | O sistema deve ser capaz de enviar notificação de agendamento de serviços |
|EN11, [BS23](brainstorming.md#requisitos-elicitados) | O sistema deve ser capaz de disponibilizar uma agenda de horários disponíveis |

<br>

## Considerações Finais

Todos os que participaram do [Brainstorming](brainstorming.md) frequentam, pelo menos 1 vez por mês, salões de beleza ou barbearias. Por esse motivo, já tínhamos em mente uma ideia de como esses estabelecimentos funcionam. <br>
Portanto, os requisitos elicitados entrevista serviram não só para validar os requisitos já elicitados no [Brainstorming](brainstorming.md) como também para reforçar o pensamento da equipe sobre o tema proposto.    

<br>

### Referências

<br>

* BARBOSA, Simone; DINIZ, Bruno. **Interação Humano-Computador**, Editora Elsevier, Rio de Janeiro, 2010.
* Stock. Disponível em: https://unbarqdsw.github.io/2020.1_G12_Stock/#/Project/Metodologias. Último acesso 18/02/2021.