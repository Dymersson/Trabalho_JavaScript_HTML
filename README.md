# Trabalho_JavaScript_HTML
<!DOCTYPE html>
<html>
<head>
  <title>Orçamentação</title>
  <style>
    body {
        display: flex;
        flex-direction: column;
        align-items: center
    }
    h1 {
        text-align: center;
    }
    .produto-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      margin-top: 40px;
    }

    .produto {
      width: 180px;
      padding: 5px;
      border: 1px solid #ddd;
      border-radius: 1px;
      text-align: center;
    }

    .produto img {
      width: 100px;
      height: 100px;
      object-fit: cover;
      margin-bottom: 10px;
    }

    .produto p {
      margin: 0;
    }
  </style>
</head>
<body>
  <h1>Orçamentação de Produtos Loja Online</h1>

  <form action="processar.php" method="POST">
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome" required><br>

    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required><br>

    <div class="produto-container">
      <div class="produto">
        <img src="https://cdn.dooca.store/117/products/bolsa-feminina-rosa_640x640+fill_ffffff.jpg?v=1626967527&webp=0" alt="Produto 1">
        <p>Bolsa Feminina</p>
        <p>R$ 319,90</p>
        <label for="quantidade1">Quantidade:</label>
        <input type="number" id="quantidade1" name="quantidade1" min="0"><br>
      </div>

      <div class="produto">
        <img src="https://cdn.shoppub.io/cdn-cgi/image/w=1000,h=1000,q=80,f=auto/usereise/media/uploads/produtos/foto/ulfezzoa/5-1.jpg" alt="Produto 2">
        <p>Tênis Masculino Whisky</p>
        <p>R$ 199,90</p>
        <label for="quantidade2">Quantidade:</label>
        <input type="number" id="quantidade2" name="quantidade2" min="0"><br>
      </div>

      <div class="produto">
        <img src="https://cdn.awsli.com.br/600x700/809/809422/produto/76981748/c121db68d8.jpg" alt="Produto 3">
        <p>Calça Jegger Masculina</p>
        <p>R$ 149,90</p>
        <label for="quantidade3">Quantidade:</label>
        <input type="number" id="quantidade3" name="quantidade3" min="0"><br>
      </div>

      <div class="produto">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRd5NbYvtExvZzITZn-_u3arRlemQ1zg5YrhA&usqp=CAU" alt="Produto 4">
        <p>Gargantilha Dourada</p>
        <p>R$ 99,90</p>
        <label for="quantidade4">Quantidade:</label>
        <input type="number" id="quantidade4" name="quantidade4" min="0"><br>
      </div>

      <div class="produto">
        <img src="https://www.safira.com.br/cdn/imagens/produtos/det/anel-de-ouro-18k-com-citrino-oval-e-pontos-de-luz-em-topazios-brancos-cde382007d99554ccc63f27bc1209dbe.jpg" alt="Produto 5">
        <p>Anel de Ouro</p>
        <p>R$ 249,90</p>
        <label for="quantidade5">Quantidade:</label>
        <input type="number" id="quantidade5" name="quantidade5" min="0"><br>
      </div>
    </div>

    <input type="submit" value="Calcular valor">
  </form>
</body>
</html>
