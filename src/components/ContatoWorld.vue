<template>
  <div class="container-geral-contato">
    <div class="container-container">
      <div class="container-contato">
        <div class="contato-1">
          <div class="container-form">
            <div class="titulo-tradicional">
              <h2 class="titulo-geral-tradicional">
                Preencha os dados abaixo corretamente e assim que possível lhe
                daremos retorno:
              </h2>
            </div>
            <!-- ESSE action SERIA PARA ENVIAR O FORMULARIO PARA O EMAIL SOLICITADO -->
            <form
              class="form"
              method="POST"
              action="https://formsubmit.co/caique_ocastro@hotmail.com "
              enctype="multipart/form-data"
            >
              <!-- ESSE input NAME:_NEXT PAGINA DE OBRIGADO POR ENVIAR  -->
              <input
                type="hidden"
                name="_next"
                value="http://localhost:8081/"
              />
  
              <!-- ESSE input NAME:_CC SERIA PARA ENVIAR COM COPIA PARA O EMAIL SOLICITADO -->
              <input type="hidden" name="_cc" value="caique.teste@teste.com" />
  
              <label class="nome">Nome</label>
              <input type="text" name="name" placeholder="Nome" />
  
              <label class="nome">E-mail</label>
              <input type="email" name="email" placeholder="E-mail" />
  
              <label class="nome">Telefone</label>
              <input type="text" name="phone" placeholder="Telefone" />
  
              <label class="nome"
                >Reclamaço, Sugestão, Elogio e/ou Informação</label
              >
              <textarea
                name="message"
                placeholder="Mensagem"
                cols="10"
                rows="5"
              ></textarea>
  
              <div class="btns">
                <a href="/"
                  ><button class="btn-exp"><strong>ENVIAR</strong></button></a
                >
              </div>
            </form>
          </div>
        </div>
        <div class="container-cell">
          <div class="cell">
            <h1 class="titulo-geral-tradicional-1">Faça seu pedido por WhatsApp</h1>
  
            <div class="botao-whats">
              <a
                class="link-links"
                href="https://www.whatsapp.com/?lang=pt_BR"
                target="_blank"
                rel="noopener noreferrer"
                ><ion-icon class="icons-1" name="logo-whatsapp"></ion-icon
                ><button class="botao-link">(11) 00000-0000</button></a
              >
            </div>
            <div class="ligar">
              <h1 class="ligue">OU LIGUE :</h1>
            <p class="tell">(11) 0000-0000</p>
            </div>
          </div>
        </div>
    </div>
    </div>

    <footer class="footer">
      <div class="container-footer">
        <div class="pizzaria">
          <h1 class="logo"><strong>Pizzaria do Bairro</strong></h1>
          <p class="enderecos">
            <strong>R. Dr. Alexandre Gutierrez, 312, São Paulo</strong>
          </p>
          <p class="enderecos"><strong>– SP, 80240-130.</strong></p>
          <h3 class="horarios">
            <strong>Segunda à Sexta, das 09h00 às 19h00.</strong>
          </h3>
        </div>
        <div class="redes">
          <a href="https://www.instagram.com/accounts/login/" target="_blank" rel="noopener noreferrer"
            ><ion-icon class="icons-icons" name="logo-instagram"></ion-icon
          ></a>
          <a href="https://www.facebook.com/login/" target="_blank" rel="noopener noreferrer"
            ><ion-icon class="icons-icons" name="logo-facebook"></ion-icon
          ></a>
        </div>
      </div>
    </footer>
  </div>
</template>
<style src="./CSS/Contato.css"></style>