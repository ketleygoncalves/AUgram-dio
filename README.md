## DESAFIO DIO

### Recriando a página inicial do Instagram 

Seguindo os passos da Dev Gabriela, consegui recriar a página inicial do Instagram utilizando HTML e CSS FLEXBOX.

Eu sou apaixonada por animais, e para dar um toque mais pessoal ao desafio utilizei meu conhecimento como design criativo e criei algumas imagens para fazer o **AUgram**, uma rede para os apaixonados por pet.

![Alt](https://i.pinimg.com/564x/1d/f0/28/1df028ba95e22c64d4c8684fffd76c1a.jpg)

* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    text-decoration: none;
    font-family: sans-serif;
    font-size: 14px;
}

body {
    width: 100%;
    min-height: 100vh;
    background-color: #d3d3d3;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
}

.augram-wrapper {
    display: flex;
    align-items: center;
    justify-content: start;
    width: 60%;
    height: 100vh;

}

.augram-phone {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 50%;
}

.augram-phone img {
    height: 25rem;
}

.augram-continue {
    display: flex;
    align-items: center; 
    justify-content: space-around; 
    flex-direction: column;
    width: 50%;
    min-height: 34rem;
}

.group {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-direction: column;
    background-color: #fff;
    width: 80%;
    padding: 1.3rem 0;
    border: 1px solid lightgrey;
}

.group:nth-child(1) {
    min-height: 19rem;

}

.augram-logo {
    height: 3rem;
}

.profile-photo {
    display: flex;
    justify-items: center;
    align-items: center;
    border-radius: 50%;
    overflow: hidden;

}

.profile-photo img {
    height: 6rem;
}

.augram-login {
    background-color: #0095f6;
    color: #fff;
    padding: 8px;
    border-radius: 4px;
}

.augram-logout {
    color: #0095f6;
    margin-top: 1rem;
}

.not-account {
    color: rgb(160, 160, 160);
}

.link-blue {
    color: #0095f6
}
.get-the-app {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 100%;
    padding: 1.3rem 0;

}

.download {
    display: flex;
    width: 100%;
    justify-content: space-evenly;
    align-items: center;
    padding: 1rem;
}

.app-download {
    height: 3rem;
    width: 15rem;
    background-size: cover;
}

.app-download:nth-child(1) {
    background-image: url('./img/app.png');    
}

.app-download:nth-child(2) {
    background-image: url('./img/play.png');
}

footer {
    position: fixed;
    bottom: 0;
    width: 100%;
}

.footer{
    text-align: center;
    color: black;
}

.kg-logo {
    height: 3rem;
}

@media (max-width: 1024px){
    .augram-wrapper {
        width: 50%;
    }
}

@media (max-width: 650px) {
    body {
        background-color: #fff;
    }
    .augram-wrapper {
        width: 50%;
    }

    .augram-phone {
    display: none;
    }

    .augram-continue{
        width: 100%;
    }

    .group {
        border: 1px solid transparent;
    }
}
