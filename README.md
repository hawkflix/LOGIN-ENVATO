<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Acesso</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background-color: #0d0d0d;
      display: flex;
      justify-content: center;
      align-items: center;
    }
    button {
      background-color: #00cc66;
      color: white;
      border: none;
      padding: 20px 40px;
      font-size: 1.2em;
      border-radius: 10px;
      cursor: pointer;
      transition: 0.3s ease;
    }
    button:hover {
      background-color: #00aa55;
    }
  </style>
</head>
<body>
  <button onclick="acessar()">Acessar Ferramentas</button>

  <script>
    function acessar() {
      // Altere aqui o link sempre que quiser atualizar
      window.location.href = 'https://app.toolzbuy.com/page/ele';
    }
  </script>
</body>
</html>
