<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Fenerbahçe - Résultats</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f0f8ff;
      color: #002868;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #002868;
      color: #ffd700;
      padding: 20px;
      text-align: center;
    }

    h1 {
      margin: 0;
    }

    .container {
      width: 90%;
      max-width: 800px;
      margin: auto;
      padding: 20px;
      background: white;
      border-radius: 10px;
      box-shadow: 0 0 10px #ccc;
      margin-top: 30px;
    }

    label {
      display: block;
      margin-top: 10px;
    }

    input, select {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    button {
      background-color: #002868;
      color: white;
      border: none;
      padding: 10px 15px;
      margin-top: 15px;
      border-radius: 5px;
      cursor: pointer;
    }

    table {
      width: 100%;
      margin-top: 30px;
      border-collapse: collapse;
    }

    th, td {
      padding: 10px;
      border: 1px solid #ccc;
      text-align: center;
    }

    th {
      background-color: #ffd700;
      color: #002868;
    }

    footer {
      text-align: center;
      padding: 20px;
      margin-top: 40px;
      background-color: #002868;
      color: #ffd700;
    }
  </style>
</head>
<body>

<header>
  <h1>Fenerbahçe SK - Résultats de Match</h1>
</header>

<div class="container">
  <h2>Ajouter un Résultat</h2>
  <form id="resultForm">
    <label>Date :</label>
    <input type="date" id="date" required>

    <label>Adversaire :</label>
    <input type="text" id="opponent" placeholder="Galatasaray, Beşiktaş..." required>

    <label>Domicile ou Extérieur :</label>
    <select id="location">
      <option value="Domicile">Domicile</option>
      <option value="Extérieur">Extérieur</option>
    </select>

    <label>Score :</label>
    <input type="text" id="score" placeholder="Ex: 3 - 1" required>

    <button type="submit">Ajouter</button>
  </form>

  <h2>Matchs enregistrés</h2>
  <table id="resultsTable">
    <tr>
      <th>Date</th>
      <th>Adversaire</th>
      <th>Lieu</th>
      <th>Score</th>
    </tr>
  </table>
</div>

<footer>
  &copy; 2025 Fenerbahçe Spor Kulübü - Tous droits réservés
</footer>

<script>
  const form = document.getElementById("resultForm");
  const table = document.getElementById("resultsTable");

  form.addEventListener("submit", function(e) {
    e.preventDefault();

    const date = document.getElementById("date").value;
    const opponent = document.getElementById("opponent").value;
    const location = document.getElementById("location").value;
    const score = document.getElementById("score").value;

    const newRow = table.insertRow(-1);

    newRow.innerHTML = `
      <td>${date}</td>
      <td>${opponent}</td>
      <td>${location}</td>
      <td>${score}</td>
    `;

    form.reset();
  });
</script>

</body>
</html><!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Fenerbahçe - Résultats</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f0f8ff;
      color: #002868;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #002868;
      color: #ffd700;
      padding: 20px;
      text-align: center;
    }

    h1 {
      margin: 0;
    }

    .container {
      width: 90%;
      max-width: 800px;
      margin: auto;
      padding: 20px;
      background: white;
      border-radius: 10px;
      box-shadow: 0 0 10px #ccc;
      margin-top: 30px;
    }

    label {
      display: block;
      margin-top: 10px;
    }

    input, select {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    button {
      background-color: #002868;
      color: white;
      border: none;
      padding: 10px 15px;
      margin-top: 15px;
      border-radius: 5px;
      cursor: pointer;
    }

    table {
      width: 100%;
      margin-top: 30px;
      border-collapse: collapse;
    }

    th, td {
      padding: 10px;
      border: 1px solid #ccc;
      text-align: center;
    }

    th {
      background-color: #ffd700;
      color: #002868;
    }

    footer {
      text-align: center;
      padding: 20px;
      margin-top: 40px;
      background-color: #002868;
      color: #ffd700;
    }
  </style>
</head>
<body>

<header>
  <h1>Fenerbahçe SK - Résultats de Match</h1>
</header>

<div class="container">
  <h2>Ajouter un Résultat</h2>
  <form id="resultForm">
    <label>Date :</label>
    <input type="date" id="date" required>

    <label>Adversaire :</label>
    <input type="text" id="opponent" placeholder="Galatasaray, Beşiktaş..." required>

    <label>Domicile ou Extérieur :</label>
    <select id="location">
      <option value="Domicile">Domicile</option>
      <option value="Extérieur">Extérieur</option>
    </select>

    <label>Score :</label>
    <input type="text" id="score" placeholder="Ex: 3 - 1" required>

    <button type="submit">Ajouter</button>
  </form>

  <h2>Matchs enregistrés</h2>
  <table id="resultsTable">
    <tr>
      <th>Date</th>
      <th>Adversaire</th>
      <th>Lieu</th>
      <th>Score</th>
    </tr>
  </table>
</div>

<footer>
  &copy; 2025 Fenerbahçe Spor Kulübü - Tous droits réservés
</footer>

<script>
  const form = document.getElementById("resultForm");
  const table = document.getElementById("resultsTable");

  form.addEventListener("submit", function(e) {
    e.preventDefault();

    const date = document.getElementById("date").value;
    const opponent = document.getElementById("opponent").value;
    const location = document.getElementById("location").value;
    const score = document.getElementById("score").value;

    const newRow = table.insertRow(-1);

    newRow.innerHTML = `
      <td>${date}</td>
      <td>${opponent}</td>
      <td>${location}</td>
      <td>${score}</td>
    `;

    form.reset();
  });
</script>

</body>
</html>
