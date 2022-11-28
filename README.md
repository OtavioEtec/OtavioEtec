<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link REL="SHORTCUT ICON" HREF="/favicon.ico">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-icon-57x57.png">
    <link rel="apple-touch-icon" sizes="60x60" href="/apple-icon-60x60.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-icon-72x72.png">
    <link rel="apple-touch-icon" sizes="76x76" href="/apple-icon-76x76.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-icon-114x114.png">
    <link rel="apple-touch-icon" sizes="120x120" href="/apple-icon-120x120.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-icon-144x144.png">
    <link rel="apple-touch-icon" sizes="152x152" href="/apple-icon-152x152.png">
    <link rel="apple-touch-icon" sizes="180x180" href="/apple-icon-180x180.png">
    <link rel="icon" type="image/png" sizes="192x192"  href="/android-icon-192x192.png">
    <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
    <link rel="icon" type="image/png" sizes="96x96" href="/favicon-96x96.png">
    <link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
    <link rel="manifest" href="/manifest.json">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="msapplication-TileImage" content="/ms-icon-144x144.png">
    <meta name="theme-color" content="#ffffff">
    <title>Matrícula Escolar</title>
    <link rel="stylesheet" href="CSS/style.css" />    
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />    
    <link
      href="https://fonts.googleapis.com/css2?family=Lato:ital,wght@0,100;0,300;0,400;0,700;0,900;1,100;1,300;1,400;1,700;1,900&display=swap"
      rel="stylesheet"  />
  </head>
  <body>
    <div class="container">
      <div id="cadastro-container">
        <h2>Matricula</h2>
        <form id="cad-form">
          <div class="cad-inputs">
            <div class="cad-control">
              <label for="Name">Nome:</label>
              <input
                type="text"
                name="Name"
                id="Name"
                placeholder="Exemplo: Gabriel Henrique Cardoso"
                required
              />
            </div>
            <div class="cad-control">
              <label for="Sexy">Sexo:</label>
              <input
                type="text"
                name="Sexy"
                id="Sexy"
                placeholder="Exemplo: Male or female"
                required
              />
            </div>
            <div class="cad-control">
              <label for="BirthDate">Data de Nascimento:</label>
              <input
                type="text"
                name="BirthDate"
                id="BirthDate"
                placeholder="Exemplo: 01/01/2000"
                required
              />
            </div>
            <div class="cad-control">
              <label for="Cpf">CPF:</label>
              <input
                type="text"
                name="Cpf"
                id="Cpf"
                placeholder="Exemplo: 737.760.030-65"
                required
              />
            </div>
          </div>
          <div class="cad-control">
            <label for="City">Cidade: </label>
            <input type="text" name="City" id="City"
            placeholder="Exemplo: Catanduva" required/>
          </div>
          <div class="cad-control">
            <label for="state">Estado: </label>
            <input type="text" name="state" id="state"
            placeholder="Exemplo: Minas Gerais" required/>
          </div>
          <div class="cad-control">
            <label for="email">Email: </label>
            <input type="text" name="email" id="email"
            placeholder="Exemplo: Josémanuel@gmail.com" required/>
          </div>
          <div class="cad-control">
            <label for="rg">Rg: </label>
            <input type="text" name="rg" id="rg"
            placeholder="Exemplo: 33.994.170-4" required/>
          </div>
          <div class="action-control">
            <button id="troca-btn"><a href="file:///E:/Lucas%20trembolona%20e%20Otavio%20Dura/PW1/AVALIA%C3%87%C3%82O/TROCAR.html">Professor ou Cordenador?Clique aqui</button></a>
            <button id="enter-btn">Novo</button>
            <button id="clear-btn">Salvar</button>
            <button id="alterar-btn">Alterar</button>
            <button id="del-btn">Excluir</button>
            <button id="consulta-btn">Consulta</button>
          </div>
        </form>
      </div>    
      <div id="Dados-container" class="hide">
        <p id="SingUp">Cadastrado: <span></span></p>
        <h3>Confira os seus Dados</h3>
        <div id="Dados">
          <div class="DadosDaTabela">
            <h4>Nome: </h4>
            <h4>Sexo: </h4>
            <h4>Data de Nascimento: </h4>
            <h4>CPF: </h4>
          </div>
        </div>
        <button id="back-btn">Alterar</button>
      </div>
    </div>
  </body>
</html>

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Lato", sans-serif;
  }
  
  body {
    background-color: #090e22;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    color: #fff;
  }
  
  .hide {
    display: none  !important;
  }
  
  .container {
    min-width: 400px;
    min-height: 400px;
    background-color: #1d1e33;
    padding: 2rem;
  }
  
  /* CADASTRO ALUNO */
  #cadastro-container h2 {
    text-align: center;
    margin-bottom: 2rem;
  }
  
  .cad-inputs {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }

.cad-control {
    display: flex;
    flex: 1;
    flex-direction: column;
    margin-bottom: 1rem;
    
}

.cad-control label {
    font-weight: bold;
    margin-bottom: 0.6rem;
   color: #ccc;  
}

.cad-control input{
    padding: 1rem 0.5rem;

} 

.action-control{
    display: flex;
    justify-content: space-between;
    margin-top: 2rem;
    gap: 1rem;

}

button {
    text-transform: uppercase;
    padding: 1rem 1.5rem;
    background-color: tomato;
    border: none;
    color:#fff;
    cursor: pointer;
    opacity: 0.9;
    flex: 1; 

}

#del-btn {
  background-color: #444;
}

#Dados-container {
    text-align: center;
}

#SingUp {
    font-size: 1.4rem;
    color: #ccc;

}

#Dados-container h3 {
    margin-bottom: 1rem;
    color: #dfdfdf;

}

#Dados-conatiner {
    display: flex;
    flex-direction: column;
}
