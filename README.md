# lanches
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>

<body>
    <h1>LANCHONETE TRABALHO</h1>
    <p id="texto"></p>
    <ul id="lista"></ul>
    <input id="input" type="text"/>
    <button onclick="adicionarItem()">adicionar item</button>
    <p>O tempo de espera é de 20 minutos</p>
    <script>


        let lista = []
        function adicionarItem(produto) {
            let produtoimput=document.getElementById("input")
            lista.push(produtoimput.value)
            mostrarlista(lista)
        }
        alert('BEM VINDO')
        var texto = document.getElementById("texto")
        texto.innerText = 'Ola oque gostaria de pedir'


        function mostrarlista(lista) {


            let listaEL = document.getElementById("lista")
            let conteudo = ""
            lista.forEach(Comida => {
                conteudo += '<li>' + Comida + '</li>'
            })
            listaEL.innerHTML = conteudo
        }
        mostrarlista(lista)



    </script>
</body>

</html>
