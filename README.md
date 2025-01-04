
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jeffinho Motos Serviços</title>
    <style>
        /* Estilo geral */
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            background-color: #000; /* Fundo preto */
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        /* Container principal */
        .container {
            text-align: center;
            max-width: 400px;
            padding: 20px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.5);
        }

        /* Logo */
        .logo img {
            max-width: 100%;
            height: auto;
            margin-bottom: 20px;
        }

        /* Input e botão */
        input[type="password"] {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: none;
            border-radius: 5px;
            background-color: #222;
            color: white;
            font-size: 16px;
            outline: none;
        }

        button {
            width: 100%;
            padding: 10px;
            background-color: #ff0000;
            color: white;
            font-size: 16px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: #cc0000;
        }

        /* Rodapé */
        .footer {
            margin-top: 10px;
            font-size: 12px;
            opacity: 0.8;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Logo -->
        <div class="logo">
            <img src="Cópia de Black Red Bold Minimalist Racing Gear Logo.svg" alt="Jeffinho Motos">
        </div>

        <!-- Campo de senha -->
        <input type="password" id="password" placeholder="Digite sua placa">

        <!-- Botão -->
        <button onclick="checkPassword()">Acessar</button>

        <!-- Rodapé -->
        <div class="footer">WhatsApp: (48) 99663-2003</div>
    </div>

    <script>
        function checkPassword() {
            const password = document.getElementById("password").value;

            // Senhas e URLs
            const redirects = {
                "MFQ8G23": "https://docs.google.com/document/d/176B5zqcJI0rbLohlK7oztTkRH7aVmohjZ1nhO_QvNGI/edit",
                "outraSenha": "https://site2.com"
            };

            // Verificar senha
            if (redirects[password]) {
                window.location.href = redirects[password];
            } else {
                alert("Senha inválida!");
            }
        }
    </script>
</body>
</html>
