<p align='center'>
  <img width="70%" src="../../img/logos/logo1.png">
  </img>
</p>

## Cabeleleila Leila

O Salão da Cabeleleira Leila é uma aplicação que visa facilitar o  gerenciamento de um salão de beleza por meio do cadastro de clientes e agendamento dos serviços oferecidos pelo estabelecimento.

A aplicação permitirá que o cliente consulte os tipos de serviços prestados e seus respectivos preços, consulte a agenda de cada especialidade e os horários livres. Além de permitir que o cliente acesse o perfil dos profissionais que atuam no local.   

## Membros da equipe
<div class="members">
  <div class="member">
    <p>Rafaella Junqueira</p>
    <img src="img/equipe/rafaella.jpeg">
  </div>
  <div class="member">
    <p>Isabella Carneiro</p>
    <img src="img/equipe/isabella.jpeg">
  </div>
  <div class="member">
    <p>Erick Giffoni</p>
    <img src="img/equipe/erick.jpeg">
  </div>
  <div class="member">
    <p>Geraldo Victor</p>
    <img src="img/equipe/geraldo.jpeg">
  </div>
</div>
<div class="members">
   <div class="member">
    <p>Lucas Lopes Pereira</p>
    <img src="img/equipe/lucas.jpeg">
  </div>
  <div class="member">
    <p>Bruna Almeida</p>
    <img src="img/equipe/bruna.jpeg">
  </div>
  <div class="member">
    <p>Kalebe Lopes</p>
    <img src="img/equipe/kalebe.jpeg">
  </div>
  <div class="member">
    <p>Damarcones Porto</p>
    <img src="img/equipe/damarcones.jpeg">
  </div>
</div>
   
<style>
  .members {
    display: flex; 
    flex-direction: row;
  }
  .member img {
    position: relative;
    width: 640px;
    opacity: 1;
    border-style: solid;
    border-radius: 640px;
    border-width: 1px; 
    border-color: rgba(0,0,0,0.3);
    z-index: 3;
    transition: opacity 0.5s !important;
  }
  .member img:hover {
    opacity: 0.4;
    z-index: 1;
  }
  .member p:hover  + img {
    opacity: 0.4;
    z-index: 1;
  }
  
 .member {
   display: flex;
   margin: 20px;
   justify-content: center;
  }
 
 .member p {
    position: absolute;
    transform: translate(0, 4.8em);
    z-index: 2;
    color: #fff;
    font-weight: bold;
    font-family: Montserrat;
  }
 
  h2, p {
    font-family: Montserrat !important;
    font-weight: 500;
  }

  h3 {
    font-family: Montserrat !important;
    font-weight: bold;
  }
</style>
