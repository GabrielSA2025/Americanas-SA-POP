<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tutorial Sistema - Americanas S.A</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background-color: #fff;
      color: #333;
    }
    header {
      background-color: #e60000;
      color: white;
      padding: 1rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
    header img {
      height: 40px;
    }
    nav {
      background: #f8f8f8;
      padding: 0.5rem;
      text-align: center;
    }
    nav button {
      background-color: #e60000;
      color: white;
      border: none;
      padding: 0.6rem 1rem;
      margin: 0 5px;
      cursor: pointer;
      border-radius: 5px;
    }
    nav button:hover {
      background-color: #cc0000;
    }
    .content {
      padding: 1.5rem;
      display: none;
    }
    .active {
      display: block;
    }
    img.tutorial-img {
      max-width: 100%;
      margin-top: 1rem;
      border: 1px solid #ccc;
    }
    a {
      color: #e60000;
    }
  </style>
</head>
<body>
  <header>
    <h1>Tutorial do Sistema - Americanas S.A</h1>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/86/Americanas_logo_2021.svg/512px-Americanas_logo_2021.svg.png" alt="Logo Americanas">
  </header>

  <nav>
    <button onclick="showTab('tutorial1')">Acessar o Sistema</button>
    <button onclick="showTab('tutorial2')">Gerar Relatório</button>
    <button onclick="showTab('tutorial3')">Suporte</button>
  </nav>

  <div id="tutorial1" class="content active">
    <h2>Como acessar o sistema</h2>
    <p>Para acessar o sistema, entre com seu login corporativo pelo site <a href="#">sistema.americanas.com</a>.</p>
    <img class="tutorial-img" src="https://via.placeholder.com/800x400?text=Login+do+Sistema" alt="Tela de login">
  </div>

  <div id="tutorial2" class="content">
    <h2>Como gerar relatório</h2>
    <p>No menu superior do sistema, clique em "Relatórios" e selecione o tipo desejado.</p>
    <img class="tutorial-img" src="https://via.placeholder.com/800x400?text=Relat%C3%B3rios" alt="Tela de relatório">
  </div>

  <div id="tutorial3" class="content">
    <h2>Suporte e ajuda</h2>
    <p>Em caso de dúvidas, contate o suporte pelo e-mail <a href="mailto:suporte@americanas.com">suporte@americanas.com</a> ou pelo ramal 1234.</p>
    <img class="tutorial-img" src="https://via.placeholder.com/800x400?text=Suporte" alt="Suporte">
  </div>

  <script>
    function showTab(id) {
      const tabs = document.querySelectorAll('.content');
      tabs.forEach(tab => tab.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }
  </script>
</body>
</html>
