<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Conexão Campo e Cidade</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #f0f8ff;
      color: #333;
      font-size: 18px;
    }

    header {
      background: linear-gradient(to right, #1e3c72, #2a5298);
      color: white;
      text-align: center;
      padding: 60px 30px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    }

    .header-container h1 {
      font-size: 42px;
      margin-bottom: 20px;
    }

    .header-container p {
      font-size: 22px;
      font-weight: 300;
    }

    nav {
      background-color: #dbe9f4;
      text-align: center;
      padding: 15px 0;
    }

    nav a {
      margin: 0 15px;
      text-decoration: none;
      color: #1e3c72;
      font-weight: bold;
      font-size: 20px;
    }

    nav a:hover {
      text-decoration: underline;
    }

    section {
      max-width: 900px;
      margin: auto;
      padding: 40px 20px;
    }

    h2 {
      color: #1e3c72;
      font-size: 32px;
      margin-bottom: 20px;
    }

    button {
      background-color: #1e3c72;
      color: white;
      border: none;
      padding: 12px 20px;
      font-size: 18px;
      margin-top: 20px;
      border-radius: 8px;
      cursor: pointer;
    }

    button:hover {
      background-color: #16345e;
    }

    .quiz {
      margin-top: 30px;
      background-color: #eef6ff;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }

    .quiz p {
      margin-bottom: 10px;
      font-size: 18px;
    }

    .quiz input {
      margin-right: 10px;
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: #2a5298;
      color: white;
    }
  </style>
</head>
<body>

<header>
  <div class="header-container">
    <h1>🌾🌆 Campo & Cidade Conectados</h1>
    <p>Do alimento à tecnologia, celebramos a união desses dois mundos!</p>
  </div>
</header>

<nav>
  <a href="#contexto">Contexto</a>
  <a href="#problemas">Problemas</a>
  <a href="#solucoes">Soluções</a>
</nav>

<section id="contexto">
  <h2>🌱 Contexto Geral</h2>
  <p>
    O campo é a origem da vida: é de lá que vem os alimentos, o ar puro e a tranquilidade da natureza.
    Já a cidade traz oportunidades, inovação e acesso a serviços. Embora pareçam mundos diferentes,
    eles se complementam mais do que imaginamos.
  </p>
  <p>
    A conexão entre campo e cidade é essencial para uma sociedade equilibrada. Quando esses espaços se conectam,
    criam um ciclo de cooperação onde todos ganham: produtos de qualidade chegam às cidades, enquanto a tecnologia
    e a educação chegam ao campo.
  </p>
  <p>
    Festejar essa relação é reconhecer a importância de cada ambiente e valorizar quem constrói a base de tudo.
  </p>
</section>

<section id="problemas">
  <h2>⚠️ Problemas na Relação</h2>
  <p>
    Apesar da importância dessa conexão, existem muitos desafios: a desigualdade entre campo e cidade é visível.
    Enquanto a cidade cresce com tecnologia, o campo muitas vezes sofre com falta de estrutura, educação e saúde.
  </p>
  <p>
    Outro problema é a desvalorização do trabalhador rural. Muitos desconhecem a origem dos alimentos e a realidade
    do campo, gerando distanciamento e preconceito.
  </p>
  <p>
    Além disso, o êxodo rural — quando jovens deixam o campo para buscar oportunidades nas cidades — ameaça
    a continuidade da produção agrícola e o desenvolvimento rural.
  </p>
</section>

<section id="solucoes">
  <h2>💡 Soluções e Caminhos</h2>
  <p>
    A principal solução está na valorização mútua: levar educação, saúde e internet ao campo e, ao mesmo tempo,
    aproximar o cidadão urbano da realidade rural com feiras, visitas escolares, e conteúdos educativos.
  </p>
  <p>
    Incentivar políticas públicas que integrem os dois mundos é essencial: estradas de qualidade, transporte,
    incentivo à agricultura familiar e programas de cooperação são algumas formas práticas.
  </p>
  <p>
    Só assim vamos construir uma sociedade mais equilibrada e justa — onde o campo e a cidade caminhem juntos.
  </p>

  <div class="quiz">
    <h3>🧠 Quiz Interativo</h3>
    <p>Qual dessas ações ajuda a aproximar o campo da cidade?</p>
    <label><input type="radio" name="resposta" value="1"> Construir mais prédios nas cidades</label><br/>
    <label><input type="radio" name="resposta" value="2"> Ignorar o trabalho do campo</label><br/>
    <label><input type="radio" name="resposta" value="3"> Incentivar feiras de produtores locais</label><br/>
    <button onclick="verificarResposta()">Verificar Resposta</button>
    <p id="feedback"></p>
  </div>
</section>

<footer>
  Agrinho 2025
</footer>

<script>
function verificarResposta() {
  const resposta = document.querySelector('input[name="resposta"]:checked');
  const feedback = document.getElementById('feedback');

  if (!resposta) {
    feedback.textContent = "Por favor, escolha uma opção!";
    feedback.style.color = "orange";
  } else if (resposta.value === "3") {
    feedback.textContent = "🎉 Correto! Feiras fortalecem a relação entre campo e cidade.";
    feedback.style.color = "green";
  } else {
    feedback.textContent = "❌ Ops! Essa ação não ajuda na conexão. Tente novamente.";
    feedback.style.color = "red";
  }
}
</script>

</body>
</html>
