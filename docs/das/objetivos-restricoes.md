# <center> Objetivos e Restrições arquiteturais
<br>
    
### Histórico de versão<br>

|Data | Versão | Descrição | Autor(es)|
| -- | -- | -- | -- |
| 16.04.2021 | 0.1 | Criação do documento | Kalebe Lopes |
| 18.04.2021 | 0.2 | Adição da introdução, objetivos e restrições | Damarcones Porto<br> Kalebe Lopes |


### Participantes

* Kalebe Lopes
* Damarcones Porto

### Introdução

<div align="justify">
<p>Os objetivos arquiteturais dizem respeito às metas mais significativas impostas à um projeto, ou seja, é tudo aquilo que satisfaz as necessidades, expectativas e desejos dos <i>Stakeholders</i>.</p>
<p>As restrições arquiteturais de um projeto referem-se aos fatores que limitam a execução da  aplicação. Em outras palavras, as restrições podem ser definidas como condições impostas ao sistema, para que este funcione de acordo com o esperado pelos <i>Stakeholders</i>. </p>
<p>Definir as restrições de um projeto é importante porque assegura a viabilidade do empreendimento e a satisfação dos <i>Stakeholders</i>. Quando um projeto é restringido por fronteiras claras, através de regras bem formuladas, há uma delimitação no campo de atuação do gerente de projetos.</p>
<p>Este documento tem por finalidade descrever os objetivos e restrições cabíveis ao projeto <i> Leila's</i>.</p>
</div>

### Objetivos e Restrições da arquitetura

#### Objetivos
<div align="justify">
<ul>

  <li><b>Escalabilidade: </b>O software deve tornar possível sua evolução e manutenção.</li>
  <li><b> Segurança: </b>A aplicação deve manter os dados de usuários em total segurança.</li>
  <li><b> Linguagem: </b>A aplicação deve conter um linguagem comum e de fácil entendimento para os usuários. </li>
  <li><b>Portabilidade: </b>A aplicação deve ser executada com desempenho igual ou similar nos navegadores Google Chrome e Mozila Firefox. </li>
  <li><b> Usabilidade: </b>A aplicação deve ser construída seguindo regras de usabilidade para atender a maioria dos usuários.</li>
  <li><b> Manutenibilidade: </b>A aplicação deve permitir manutenção e melhorias de maneira a não gerar custo e tempo muito acima do normal.</li>

</ul>
</div>

#### Restrições
<ul>
  <li><b>Tecnologias: </b>A aplicação deverá ser desenvolvida utilizando as seguintes ferramentas e tecnologias: 
    <ul>
        <li>Spring Boot: Framework escrito em Java para o desenvolvimento do back-end da aplicação</li>
        <li>AngularJS: Framework escrito em JavaScript para o desenvolvimento do front-end da aplicação Web. Possui fácil              integração com o bootstrap e permite a utilização do HTML.</li>
        <li>Typescript: Super conjunto do JavaScript, utilizado juntamente com o framework AngularJS na construção do front-            end</li>
        <li>Bootstrap: Framework de CSS que torna fácil a criação de elementos em websites. Agiliza a criação de páginas                esteticamente agradáveis, pois seus padrões de design seguem os princípios de usabilidade para interfacrs</li>
        <li>SQL: Banco de dados relacional que armazena os dados em tabelas. Utiliza a linguagem SQL para a manipulação                 dos dados</li>
        <li>Github: Controle de versionamento da aplicação.</li>
     </ul>
  </li>
  <li><b>Conectividade: </b>A aplicação necessitará de conexão com a internet para funcionar.</li>
  <li><b>Prazo: </b>A aplicação deverá ser finalizada na data estipulada para entrega final.</li>
  <li><b>Idioma: </b>A aplicação deve ser voltada para a linguagem Português-Brasil.</li>
  <li><b>Público alvo: </b>A aplicação deve atender usuários que desejam agendar serviços no salão <i>Leila's</i>.</li>
</ul>

## Referências

EUAX, **Restrições de um projeto: pare de confundir esse conceito de uma vez por todas!**. Disponível em [https://www.euax.com.br/2019/03/restricoes-de-um-projeto/](https://www.euax.com.br/2019/03/restricoes-de-um-projeto/). Acesso em 18 de abril de 2021.

ECS, **Goal and Constraints: An example**. Disponível em [https://www.ecs.csun.edu/~rlingard/COMP684/Example2SoftArch.htm](https://www.ecs.csun.edu/~rlingard/COMP684/Example2SoftArch.htm). Acesso em 18 de abril de 2021.
