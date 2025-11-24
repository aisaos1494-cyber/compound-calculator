<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Калькулятор сложного процента</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            max-width: 500px;
            margin: 40px auto;
            padding: 20px;
            background: #f8f8f8;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        h2 {
            text-align: center;
        }
        label {
            font-weight: bold;
        }
        input {
            width: 100%;
            padding: 10px;
            margin: 6px 0 15px 0;
            border: 1px solid #aaa;
            border-radius: 6px;
        }
        button {
            width: 100%;
            padding: 12px;
            background: #009688;
            color: white;
            border: none;
            border-radius: 6px;
            font-size: 16px;
            cursor: pointer;
        }
        button:hover {
            background: #00796b;
        }
        #result {
            margin-top: 20px;
            padding: 15px;
            background: #fff;
            border: 1px solid #ccc;
            border-radius: 6px;
            font-size: 18px;
        }
    </style>
</head>
<body>

<h2>Калькулятор сложного процента</h2>

<label>Начальный капитал (₽):</label>
<input type="number" id="principal" placeholder="Например: 10000">

<label>Годовая процентная ставка (%):</label>
<input type="number" id="rate" placeholder="Например: 12">

<label>Количество лет:</label>
<input type="number" id="years" placeholder="Например: 5">

<label>Период начисления процентов:</label>
<select id="period">
    <option value="12">Ежемесячно</option>
    <option value="4">Ежеквартально</option>
    <option value="1">Ежегодно</option>
    <option value="365">Ежедневно</option>
</select>

<button onclick="calculate()">Рассчитать</button>

<div id="result"></div>

<script>
function calculate() {
    let P = parseFloat(document.getElementById("principal").value);
    let r = parseFloat(document.getElementById("rate").value) / 100;
    let t = parseFloat(document.getElementById("years").value);
    let n = parseFloat(document.getElementById("period").value);

    if (isNaN(P)  isNaN(r)  isNaN(t)) {
        document.getElementById("result").innerHTML = "Заполните все поля!";
        return;
    }

    let A = P * Math.pow((1 + r / n), n * t);
    A = A.toFixed(2);

    document.getElementById("result").innerHTML =
        "Итоговая сумма: <b>" + A + " ₽</b>";
}
</script>

</body>
</html>
