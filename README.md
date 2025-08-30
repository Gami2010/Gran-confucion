<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>La Doble Vida de Pi: Numeral, Constante y Símbolo</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400;0,700;1,400&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Lora', serif;
            background-color: #f8f9fa;
            color: #212529;
            line-height: 1.8;
            margin: 0;
            padding: 25px;
            display: flex;
            justify-content: center;
        }
        .container {
            max-width: 900px;
            width: 100%;
            background-color: #ffffff;
            border-radius: 10px;
            padding: 40px 50px;
            box-shadow: 0 5px 25px rgba(0, 0, 0, 0.07);
        }
        h1 {
            font-family: 'Playfair Display', serif;
            font-size: 2.8em;
            text-align: center;
            color: #343a40;
            margin-bottom: 20px;
        }
        p {
            font-size: 1.1em;
            text-align: justify;
            margin-bottom: 1.5em;
        }
        .interactive-container {
            display: flex;
            gap: 25px;
            margin: 35px 0;
        }
        .card {
            flex: 1;
            padding: 25px;
            border: 2px solid #ced4da;
            border-radius: 10px;
            cursor: pointer;
            transition: all 0.3s ease-in-out;
            text-align: center;
        }
        .card:hover, .card.active {
            border-color: #007bff;
            box-shadow: 0 6px 25px rgba(0, 123, 255, 0.15);
            transform: translateY(-8px);
        }
        .card h2 {
            font-family: 'Playfair Display', serif;
            font-size: 3.5em;
            margin: 0 0 10px 0;
            color: #0056b3;
        }
        .card .subtitle {
            font-family: 'Lora', serif;
            font-weight: bold;
            font-size: 1.1em;
            color: #495057;
            margin: 0;
        }
        .explanation {
            display: none;
            margin-top: 35px;
            animation: fadeIn 0.8s ease;
        }
        .explanation.visible {
            display: block;
        }
        h3 {
            font-family: 'Playfair Display', serif;
            font-size: 2em;
            color: #343a40;
            border-bottom: 2px solid #007bff;
            padding-bottom: 10px;
            margin-top: 1.5em;
        }
        h4 {
            font-family: 'Playfair Display', serif;
            font-size: 1.4em;
            color: #495057;
            margin-top: 1.5em;
        }
        code, .formula-box {
            font-family: 'Courier New', Courier, monospace;
            background-color: #e9ecef;
            padding: 3px 6px;
            border-radius: 4px;
            font-size: 1em;
        }
        .formula-box {
            display: block;
            padding: 20px;
            margin: 20px 0;
            text-align: center;
            font-size: 1.3em;
            white-space: nowrap;
            overflow-x: auto;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 25px;
        }
        th, td {
            border: 1px solid #dee2e6;
            padding: 12px;
            text-align: left;
        }
        th {
            background-color: #f8f9fa;
            font-family: 'Lora', serif;
            font-weight: bold;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(15px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>La Doble Vida de Pi: Numeral, Constante y Símbolo</h1>
        <p>El alfabeto griego es una fuente inagotable de símbolos para la ciencia, pero ninguna letra genera tanta confusión como Pi. Ver el símbolo <strong>Π</strong> y asociarlo inmediatamente con la constante 3.14159... es un error tan común como comprensible. La realidad es que la misma letra ha sido usada en contextos radicalmente diferentes a lo largo de la historia de las matemáticas. Haz clic en las tarjetas para desentrañar esta fascinante historia.</p>

        <div class="interactive-container">
            <div class="card" id="card-attic">
                <h2>Π</h2>
                <p class="subtitle">El Numeral Antiguo</p>
            </div>
            <div class="card" id="card-modern">
                <h2>π y Π</h2>
                <p class="subtitle">Los Símbolos Modernos</p>
            </div>
        </div>

        <!-- EXPLICACIÓN DEL MUNDO ANTIGUO -->
        <div class="explanation" id="explanation-attic">
            <h3>Π: El Símbolo del "Cinco" en la Antigua Grecia</h3>
            <p>En el sistema de numeración ático, o herodiánico, usado en la Antigua Grecia desde el siglo VII a.C., los símbolos se escogían por el principio de acrofonía: usar la primera letra del nombre del número. En este contexto, <strong>Π</strong> era simplemente un numeral, un jeroglífico para una cantidad.</p>
            <ul>
                <li><strong>Π</strong> es la primera letra de <strong>Πέντε (Pente)</strong>, que significa "cinco".</li>
                <li><strong>Δ</strong> es la primera letra de <strong>Δέκα (Deka)</strong>, que significa "diez".</li>
                <li><strong>Η</strong> es la primera letra de <strong>Ηεκατόν (Hekaton)</strong>, que significa "cien".</li>
            </ul>
            <h4>Ejemplos en la práctica</h4>
            <p>Este sistema era aditivo, similar al romano. Para escribir un número, se combinaban los símbolos necesarios. Por ejemplo, el número <strong>28</strong> se escribía:</p>
            <div class="formula-box">ΔΔΠΙΙΙ</div>
            <p>Que se descompone en (10 + 10) + 5 + (1 + 1 + 1). Este sistema era funcional para el comercio y los registros, pero carecía de la flexibilidad del sistema arábigo: no tenía cero y hacía la multiplicación y división extremadamente complejas, siendo completamente incapaz de representar números irracionales.</p>
        </div>

        <!-- EXPLICACIÓN DEL MUNDO MODERNO -->
        <div class="explanation" id="explanation-modern">
            <h3>π y Π: El Alfabeto Griego como Caja de Herramientas</h3>
            <p>Las matemáticas modernas reutilizaron el alfabeto griego, pero no como numerales, sino como <strong>símbolos para conceptos abstractos</strong>. El significado de la letra ya no proviene del nombre de un número, sino de una idea matemática clave.</p>
            
            <h4>π Minúscula: La Constante de la Geometría</h4>
            <p>El uso de <strong>π (pi minúscula)</strong> para la constante ~3.14159... fue popularizado en el siglo XVIII. Se eligió porque es la primera letra de la palabra griega <strong>περίμετρος (perimetros)</strong>, que significa "perímetro" o "circunferencia". Representa la relación universal entre la circunferencia de un círculo y su diámetro.</p>
            
            <h4>π en Fórmulas Fundamentales</h4>
            <p>Hoy, π es una de las constantes más importantes de toda la ciencia, apareciendo en innumerables fórmulas:</p>
            <div class="formula-box">C = 2πr &nbsp;&nbsp;|&nbsp;&nbsp; A = πr² &nbsp;&nbsp;|&nbsp;&nbsp; V = (4/3)πr³</div>
            <p>Incluso aparece en la que es considerada la ecuación más bella de las matemáticas, la Identidad de Euler, que conecta cinco constantes fundamentales:</p>
            <div class="formula-box">e<sup>iπ</sup> + 1 = 0</div>
            
            <h4>Un Patrón General: El Caso de Sigma (Σ)</h4>
            <p>La reutilización de letras griegas es un patrón. Tomemos como ejemplo <strong>Sigma (Σ)</strong>. En la numeración ática no tenía valor, pero en matemáticas modernas, <strong>Σ (sigma mayúscula)</strong> es el símbolo universal de la <strong>Sumatoria</strong>. Se eligió por ser la primera letra de la palabra <strong>Σύνολο (Sýnolo)</strong>, que significa "suma" o "total".</p>
            <div class="formula-box">∑<sub>n=1</sub><sup>4</sup> n = 1 + 2 + 3 + 4 = 10</div>
            
            <h4>El Regreso de la Π Mayúscula: La Productoria</h4>
            <p>Aquí es donde la historia se vuelve aún más interesante. Las matemáticas modernas también encontraron un uso para la <strong>Π (Pi mayúscula)</strong>. Siguiendo la misma lógica que con Sigma, se eligió <strong>Π</strong> para representar la <strong>Productoria</strong>, es decir, la multiplicación sucesiva de una serie de términos. La elección se debe a que la palabra "Producto" también tiene un sonido inicial similar a "Pi".</p>
            <p>Mientras que Σ suma, Π multiplica:</p>
            <div class="formula-box">∏<sub>n=1</sub><sup>4</sup> n = 1 × 2 × 3 × 4 = 24</div>

            <h3>Tabla Resumen: La Triple Identidad de Pi</h3>
            <p>La próxima vez que veas una letra griega en una ecuación, recuerda que es parte de un rico lenguaje simbólico. La letra Pi es el mejor ejemplo de cómo un mismo símbolo puede tener significados tan distintos en diferentes épocas del pensamiento matemático.</p>
            <table>
                <thead>
                    <tr>
                        <th>Símbolo</th>
                        <th>Contexto</th>
                        <th>Significado</th>
                        <th>Ejemplo</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td><strong>Π</strong></td>
                        <td>Numeración Ática (Antigua)</td>
                        <td>El número entero <strong>Cinco</strong> (de <em>Pente</em>)</td>
                        <td>ΔΠ = 15</td>
                    </tr>
                    <tr>
                        <td><strong>π</strong></td>
                        <td>Matemáticas Modernas</td>
                        <td>La constante <strong>~3.14159...</strong> (de <em>Perimetros</em>)</td>
                        <td>A = πr²</td>
                    </tr>
                    <tr>
                        <td><strong>Π</strong></td>
                        <td>Matemáticas Modernas</td>
                        <td>El operador <strong>Productoria</strong> (multiplicación)</td>
                        <td>∏<sub>n=1</sub><sup>3</sup> n = 6</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>

    <script>
        const cardAttic = document.getElementById('card-attic');
        const cardModern = document.getElementById('card-modern');
        const explanationAttic = document.getElementById('explanation-attic');
        const explanationModern = document.getElementById('explanation-modern');
        const cards = [cardAttic, cardModern];
        const explanations = [explanationAttic, explanationModern];

        function toggleActive(selectedIndex) {
            explanations.forEach((exp, index) => {
                if (index === selectedIndex) {
                    exp.classList.add('visible');
                    cards[index].classList.add('active');
                } else {
                    exp.classList.remove('visible');
                    cards[index].classList.remove('active');
                }
            });
        }

        cardAttic.addEventListener('click', () => toggleActive(0));
        cardModern.addEventListener('click', () => toggleActive(1));
    </script>

</body>
</html>
