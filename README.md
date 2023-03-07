# HTML_acessandoatributo1

<!DOCTYPE html>
<html>

<head>
    <meta charset='UTF-8'>
    <title>Acessando Atributos #01</title>
    <link rel='stylesheet' href='css/estilo.css'>
</head>

<body class='conteudo exercicio'>
    <div>
        <a href='https://www.cod3r.com.br'>Cod3r</a>
    </div>
    <div id='primeiro'>
        <img src='http://files.cod3r.com.br/curso-web/logo-estreita.png' alt='logo'>
    </div>
    <script>
        const img = document.querySelector('img'); //pegar todas as propriedades da tag img
        console.log('getAttribute', img.getAttribute('src')) //pegar o atributo src 
        console.log('src',img.src); //pegar o atributo src  
        console.log('["src"]', img['src']) //pegar o atributo src 
        console.log('alt',img.alt); //pegar o atributo alt

        console.log("Elemento 'img'............")
        console.log("NodeTypes", img.nodeType);// retornar  tipo de node types
        console.log("NodeName", img.nodeName);// retornar nome do node

        const src = img.getAttributeNode('src');
        console.log("Atributo 'src'.......");
        console.log("NodeTypes", src.nodeType);// retornar tipo do node types
        console.log("NodeName", src.nodeName);// retornar nome do node
        console.log("NodeValue", src.nodeValue);// retornar valor do node

        const link = document.querySelector('a');
        console.log("Elemento 'a'.......")
        console.log('href', link.href);
        console.log('firstChild.nodeType', link.firstChild.nodeType);//
        link.firstChild.nodeValue= "novo Texto"
        link.innerHTML= 'Novo Texto2'

    </script>
</body>

</html>
