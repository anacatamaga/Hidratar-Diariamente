Aqui podes calcular a quantidade mínima de água necessária no teu dia a dia  

<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora de Hidratação</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 20px;
        }
        input, button {
            margin: 10px;
            padding: 10px;
            font-size: 16px;
        }
    </style>
</head>
<body>
    <h1>Calculadora de Hidratação</h1>
    <p>Insere o teu peso (em kg) para descobrir quanta água deves beber por dia:</p>
    <input type="number" id="peso" placeholder="Peso em kg">
    <button onclick="calcularAgua()">Calcular</button>
    <p id="resultado"></p>

    <script>
        function calcularAgua() {
            const peso = document.getElementById('peso').value;
            if (peso) {
                const aguaDiaria = peso * 35; // 35 ml por kg
                document.getElementById('resultado').innerText = `Deves beber cerca de ${aguaDiaria} ml de água por dia.`;
            } else {
                document.getElementById('resultado').innerText = "Por favor, insere o teu peso.";
            }
        }
    </script>
</body>
</html>
