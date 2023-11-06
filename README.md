<!DOCTYPE html>
<html>
<head>
    <title>Quer ser feliz comigo para sempre?</title>
    <style>
        #container {
            text-align: center;
            padding: 50px;
        }
    </style>
</head>
<body>
<div id="container">
    <h1>Quer ser feliz comigo para sempre?</h1>
    <button id="simButton">Sim</button>
    <button id="naoButton">Não</button>
</div>

<script>
    const simButton = document.getElementById("simButton");
    const naoButton = document.getElementById("naoButton");

    naoButton.addEventListener("mouseover", function() {
        const newX = Math.random() * (window.innerWidth - naoButton.clientWidth);
        const newY = Math.random() * (window.innerHeight - naoButton.clientHeight);
        naoButton.style.position = "absolute";
        naoButton.style.left = newX + "px";
        naoButton.style.top = newY + "px";
    });

    simButton.addEventListener("click", function() {
        alert("Eu te amo!");
    });
</script>
</body>
</html>
