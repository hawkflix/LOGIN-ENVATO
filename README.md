<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Acesso Restrito</title>
  <style>
    body {
      margin: 0;
      font-family: sans-serif;
      background: #f0f0f0;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .login-box {
      background: white;
      padding: 30px;
      box-shadow: 0 0 12px rgba(0,0,0,0.1);
      border-radius: 8px;
      width: 100%;
      max-width: 360px;
    }

    .login-box h2 {
      margin-bottom: 20px;
      text-align: center;
    }

    input {
      width: 100%;
      padding: 12px;
      margin-bottom: 15px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }

    button {
      width: 100%;
      padding: 12px;
      background-color: #ff5733;
      color: white;
      border: none;
      border-radius: 4px;
      font-weight: bold;
      cursor: pointer;
    }

    button:hover {
      background-color: #e2461f;
    }

    .note {
      margin-top: 10px;
      font-size: 12px;
      color: #999;
      text-align: center;
    }
  </style>
</head>
<body>
  <div class="login-box">
    <h2>Acesso</h2>
    <form method="POST" action="https://toolzbuy.com/login">
      <input type="text" name="username" placeholder="Usuário ou E-mail" required />
      <input type="password" name="password" placeholder="Senha" required />
      <button type="submit">Entrar</button>
    </form>
    <div class="note">Acesso restrito às ferramentas autorizadas.</div>
  </div>
</body>
</html>
