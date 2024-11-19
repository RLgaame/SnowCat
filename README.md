<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Snow the Cat</title>
    <link rel="shortcut icon" href="favicon.ico" type="image/x-icon">
    <style>

        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400..900&display=swap');

          /* Definindo a animação do texto piscando */
          @keyframes piscarTexto {
            0% { opacity: 1; }
            50% { opacity: 0; }
            100% { opacity: 1; }
        }

        body{
    
            background-repeat: no-repeat;
            background-image: linear-gradient(rgb(255, 255, 255), rgb(134, 180, 240));
            background-size: cover;      /* Faz a imagem cobrir toda a tela */
            background-position: center; /* Centraliza a imagem */
            background-attachment: fixed; /* A imagem permanece fixa quando você rola a página */
            height: 100%;                 /* Garante que o corpo ocupe 100% da altura da janela */
            margin: 0;                    /* Remove margens do body */
            padding: 0;                   /* Remove o padding do body */
            box-sizing: border-box;       /* Garante que o padding e border não afetem as dimensões */

        

        }
        

        /* Resetando margens e padding */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Estilo do fundo do site */
        .gamer-board {
            width: 100%;
            min-height: 100vh; /* Usando altura mínima total da tela */
            margin: 0 auto;
            position: relative;
            background-attachment: fixed;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            padding-bottom: 10px; /* Adicionando espaçamento para a borda não sobrepor o conteúdo */
        }

        /* Estilo da pessoa */
        .pessoa img {
            max-width: 100%; /* Responsivo para largura da tela */
            height: auto; /* Manter a proporção */
            max-width: 150px; /* Largura máxima da imagem */
            transform: scale(1.7) translateY(-45px); /* Suspende a imagem um pouco para cima */
            mix-blend-mode: multiply;

        }

        /* Estilo do botão */
       

        a:hover {
            color: rgb(252, 174, 174);

        }

        /* Estilo do link */
        a {
            font-family: "Orbitron", sans-serif;
            text-decoration: none;
            font-style: italic;
            font-size: 40px;
            color: rgb(0, 110, 255);
            animation: piscarTexto 1s infinite; /* Animação de piscar no texto */

        }

        /* Estilo para telas pequenas (como smartphones) */
        @media (max-width: 600px) {
            .gamer-board {
                min-height: 100vh; /* Garante que a altura mínima seja 100vh, mesmo em telas pequenas */
                padding: 20px;
            }

            .pessoa img {
                max-width: 120px; /* Ajustando o tamanho da imagem em telas pequenas */
            }

            button {
                font-size: 14px; /* Ajustando o tamanho da fonte do botão */
                padding: 12px 24px; /* Ajustando o tamanho do botão */
                width: 100%; /* O botão vai ocupar toda a largura disponível */
            }
        }


        .snowflake {
    position: absolute;
    top: -10px; /* Começa acima da tela */
    background-color: rgb(253, 253, 253);
    width: 10px;
    height: 10px;
    border-radius: 50%;
    opacity: 0.8;
    animation: snow 5s linear infinite;
}

/* Criando diferentes animações para os flocos */
.snowflake:nth-child(1) {
    left: 10%;
    animation-duration: 6s;
    animation-delay: 0s;
}

.snowflake:nth-child(2) {
    left: 30%;
    animation-duration: 8s;
    animation-delay: 1s;
}

.snowflake:nth-child(3) {
    left: 50%;
    animation-duration: 7s;
    animation-delay: 2s;
}

.snowflake:nth-child(4) {
    left: 70%;
    animation-duration: 9s;
    animation-delay: 3s;
}

.snowflake:nth-child(5) {
    left: 90%;
    animation-duration: 6s;
    animation-delay: 4s;
}

/* Animação dos flocos caindo */
@keyframes snow {
    0% {
        transform: translateY(0);
        opacity: 0.8;
    }
    100% {
        transform: translateY(100vh);
        opacity: 0.5;
    }
}
    </style>
</head>
<body>

    <div class="gamer-board">
        <div class="pessoa">
            <img src="pessoa.gif" alt="Pessoa">
        </div>
            <a href="teste.html"><strong>Play</strong></a>    
    </div>

    <div class="body">
        <img src="mount-everest-8297059_640.webp" alt=""  width="1000px" height="auto">
        <div class="snowflake"></div>
        <div class="snowflake"></div>
        <div class="snowflake"></div>
        <div class="snowflake"></div>
        <div class="snowflake"></div>
        <div class="snowflake"></div>
    </div>


</body>
</html>
