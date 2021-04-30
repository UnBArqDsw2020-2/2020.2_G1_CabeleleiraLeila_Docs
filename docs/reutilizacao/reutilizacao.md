# <center> Reutilização de Software
<br>

### Histórico de versão
  
|Data | Versão | Descrição | Autor(es)
| -- | -- | -- | -- |
| 28.04.2021 | 0.1 | Criação do documento | Isabella Carneiro |
| 28.04.2021 | 0.2 | Adição da Introdução | Isabella Carneiro |
| 30.04.2021 | 0.3 | Adição da introdução sobre Framework e Spring | Bruna Almeida<br>Damarcones Porto|
| 30.04.2021 | 0.4 | Adição da introdução sobre bibliotecas | Bruna Almeida<br>Damarcones Porto<br>Isabella Carneiro |
| 30.04.2021 | 0.5 | Adição das bibliotecas utilizadas no projeto | Bruna Almeida<br>Damarcones Porto |
<br>

## Introdução
<div align="justify">
A reutilização de software pode ser definida como o uso de softwares já existentes para construir outros. A adoção dessa prática contribui na melhoria da qualidade do software que será desenvolvido.
<br><br>
Neste documento serão apresentados as iniciativas de reutilização de software que foram utilizadas ao longo do desenvolvimento do projeto.
</div><br>

## Frameworks
<div align="justify">
Os frameworks são templates usados por desenvolvedores para criar os seus projetos e gerenciá-los de maneira mais ágil e prática. Eles funcionam como uma plataforma de desenvolvimento, e trazem uma série de ferramentas especiais, guias e outros componentes. Com diversos conceitos embutidos e códigos funcionais, o desenvolvedor só precisa preencher as lacunas e personalizar o código para adaptá-lo às necessidades do projeto que está sendo desenvolvido. O objetivo de uso dessa ferramenta é aplicar funcionalidades e estruturas já programadas para garantir mais produtividade e qualidade no desenvolvimento de um projeto. 
<br><br>
Como resultado, é possível entregar um app estável e de alta qualidade, e também economizar tempo de trabalho, já que a plataforma não exige que um código seja escrito do zero. Além disso, as ferramentas são feitas de forma aberta e podem se adaptar a diversas situações com facilidade. Uma das principais vantagens de se utilizar um Framework é a agilidade e economia do tempo. Afinal, essas ferramentas facilitam o desenvolvimento dos sistemas, permitindo que os programadores não percam tempo com funcionalidades mais básicas. 
<br><br>
No projeto Leila's, Frameworks foram utilizados tanto no Back-end quanto no Front-end, e serão detalhados seguidamente.
</div><br>

### Reutilização no BackEnd

#### Spring
<div align="justify"> 
O Spring é um framework de código aberto para plataformas Java. Com o objetivo de facilitar no desenvolvimento de aplicações, utilizando os conceitos de Inversão de Controle e Injeção de Dependências.
</div><br>

### Reutilização no FrontEnd



<br><br>

## Bibliotecas
<div align="justify">
Em programação, uma biblioteca é uma coleção de códigos voltados a resolver um determinado tipo de problema. A ideia da biblioteca é compartilhar soluções por meio de funções ou métodos. Desenvolvedores disponibilizam bibliotecas que possuem muitas funções prontas. Assim, outros programadores podem utilizá-las, permitindo que o desenvolvimento seja mais fácil e rápido.
<br><br>
Uma das grandes vantagens da criação de bibliotecas é que você pode utilizá-las em diferentes projetos. Essa prática vai ao encontro de um princípio muito importante de Clean Code: a divisão de responsabilidades. 
<br><br>
As principais bibliotecas utilizadas no código da aplicação Leila's serão descritas a seguir.
</div><br>

<div align="justify"><b>JWT:</b> JSON Web Token(JWT) é um método RCT 7519 padrão da indústria para realizar autenticação entre duas partes por meio de um token assinado que autentica uma requisição web. Esse token é um código em Base64 que armazena objetos JSON com os dados que permitem a autenticação da requisição. No projeto, essa biblioteca está sendo utilizada para autenticação de Login e serviços.</div><br>


<div align="justify"><b>SpringFox:</b> é uma ferramenta open source desenvolvida para integrar projetos Spring Boot com a especificação Swagger. A ferramenta fornece as anotações necessárias para a criação da documentação Swagger e uma interface amigável (SpringFox Swagger-UI) para expor as documentações da API Rest. No projeto, viabiliza os testes que simulam a utilização de um banco de dados, sem a necessidade de configurar propriamente um banco de dados.</div><br>

<div align="justify"><b>Swagger:</b>Trata-se de uma aplicação open source que auxilia desenvolvedores nos processos de definir, criar, documentar e consumir APIs REST. Em suma, o Swagger visa padronizar este tipo de integração, descrevendo os recursos que uma API deve possuir, como endpoints, dados recebidos, dados retornados, códigos HTTP e métodos de autenticação, entre outros. O Swagger está sendo utilizado para demonstrar os métodos de escrita e leitura da aplicação Leila's</div><br> 
<!-- Essas são as bibliotecas mais relevantes, acredito que só essas bastam -->


## Considerações finais


## Referências
DevMedia. **Frameworks e Padrões de Projeto**. Disponível em [https://www.devmedia.com.br/frameworks-e-padroes-de-projeto/1111](https://www.devmedia.com.br/frameworks-e-padroes-de-projeto/1111).

TRYBE. **Framework: o que é, como ele funciona e para que serve?**. Disponível em [https://blog.betrybe.com/framework-de-programacao/o-que-e-framework/](https://blog.betrybe.com/framework-de-programacao/o-que-e-framework/).

REVELO. **Framework: saiba como usar e quais são os mais populares**. Disponível em [https://blog.revelo.com.br/o-que-e-framework-exemplos-e-aplicacoes/](https://blog.revelo.com.br/o-que-e-framework-exemplos-e-aplicacoes/).

SOS. **O que são frameworks? Para que servem?**. Disponível em [https://www.sos.com.br/noticias/tecnologia/o-que-sao-frameworks-para-que-servem](https://www.sos.com.br/noticias/tecnologia/o-que-sao-frameworks-para-que-servem).

BE CODE. **Framework x Biblioteca x API. Entenda as diferenças!**. Disponível em [https://becode.com.br/framework-biblioteca-api-entenda-as-diferencas/](https://becode.com.br/framework-biblioteca-api-entenda-as-diferencas/).

TREINA WEB. **Qual a diferença entre Framework e Biblioteca?**. Disponível em [treinaweb.com.br/blog/qual-a-diferenca-entre-framework-e-biblioteca/](https://www.treinaweb.com.br/blog/qual-a-diferenca-entre-framework-e-biblioteca/).

DEVMEDIA. **Como o JWT funciona**. Disponível em [https://www.devmedia.com.br/como-o-jwt-funciona/40265](https://www.devmedia.com.br/como-o-jwt-funciona/40265).

TOTVS. **Documentação de APIs utilizando SpringFox**. Disponível em [https://tjf.totvs.com.br/docs/swagger-springfox](https://tjf.totvs.com.br/docs/swagger-springfox).

GR1D. **Desenvolvedor, saiba como swagger pode ajudar você**. Disponível em [gr1d.io/insurance/trends/post/desenvolvedor-saiba-como-swagger-pode-ajudar-voce-4a3b1b49c0](https://gr1d.io/insurance/trends/post/desenvolvedor-saiba-como-swagger-pode-ajudar-voce-4a3b1b49c0).




