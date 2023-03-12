# PArcial1
trabalho de matemática parcial 1 grupo 34
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mega Sena</title>
    <link rel="stylesheet" href="estilo.css">
</head>
<body>
    <div class="box">
        <h1></h1>
        <h2></h2>
        <h3></h3>
        <h4></h4>
        <h5></h5>
        <h6></h6>
        <button>Sortear</button>
    </div>

    <script src="app.js"></script>
</body>
</html>

*{
    padding: o;
    margin: 0;
    box-sizing: content-box;
    font-family: "Arial";
}

body{
    background-color: plum;
    width: 100%;
    min-height: 100vh;
    display: grid;
    place-items: center;
}

div.box{
    min-width: 1000px;
    background-color: rgb(78, 3, 3);
    border-radius: 100px;
    padding: 100px;
    text-align: center;
}

div.box h1{
font-size: 22pt;
color: rgb(255, 255, 255);
margin: 15px 0;
}

div.box h2{
    font-size: 22pt;
    color: rgb(255, 255, 255);
    margin: 15px 0;
}

div.box h3{
      font-size: 22pt;
      color: rgb(255, 255, 255);
      margin: 15px 0;
}

div.box h4{
    font-size: 22pt;
    color: rgb(255, 255, 255);
    margin: 15px 0;
}

div.box h5{
    font-size: 22pt;
    color: rgb(255, 255, 255);
    margin: 15px 0;
}

div.box h6{
    font-size: 22pt;
    color: rgb(255, 255, 255);
    margin: 15px 0;
}

div.box button{
font-size: 16pt;
padding: 10px 15px;
border: 0;
border-radius: 5px;
background-color: plum;
color: rgb(78, 10, 10);
cursor: pointer;
}
const botaoSortear = document.querySelector("div.box button") 
var numeroSorteado = document.querySelector("div.box h1")
var numeroSorteado2 = document.querySelector("div.box h2")
var numeroSorteado3 = document.querySelector("div.box h3")
var numeroSorteado4 = document.querySelector("div.box h4")
var numeroSorteado5 = document.querySelector("div.box h5") 
var numeroSorteado6 = document.querySelector("div.box h6")

var roleta = []

for(i =01;i <= 60; i++){
    roleta.push(i)
}

botaoSortear.addEventListener("click", () => {
    numeroSorteado.innerHTML = "Primeiro Número Sorteado:" + roleta[Math.floor(Math.random() * roleta.length)] 
    numeroSorteado2.innerHTML = "Segundo Número Sorteado:" + roleta[Math.floor(Math.random() * roleta.length)]
    numeroSorteado3.innerHTML = "Terceiro Número Sorteado:" + roleta[Math.floor(Math.random() * roleta.length)]
    numeroSorteado4.innerHTML = "Quarto Número Sorteado:" + roleta[Math.floor(Math.random() * roleta.length)]
    numeroSorteado5.innerHTML = "Quinto Número Sorteado:" + roleta[Math.floor(Math.random() * roleta.length)]  
    numeroSorteado6.innerHTML = "Sexto Número Sorteado:" + roleta[Math.floor(Math.random() * roleta.length)]
   
})
