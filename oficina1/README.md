# Oficina-Fiap

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
DOC HTML

<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <!-- google fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Fjalla+One&family=Varela+Round&display=swap" rel="stylesheet">

    <!-- CDN font awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"
        integrity="sha512-iecdLmaskl7CVkqkXNQ/ZH/XLlvWZOJyj7Yy7tcenmpD1ypASozpmT/E0iPtmFIB46ZmdtAc9eNBvH0H/ZpiBw=="
        crossorigin="anonymous" referrerpolicy="no-referrer" />

    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Oficina Web</title>
    <link rel="stylesheet" href="./css/style.css">

</head>

<body>
    <h1>Oficina Web</h1>

    <div class="cards">

        <!-- .card-item*3 -->
        <div class="card-item">
            <i class="fa-solid fa-robot icone"></i> <!-- icone de robo-->
            <h2>Robô</h2>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </p>
            <a href="" class="btn">Veja mais</a>
        </div>


        <div class="card-item">
            <i class="fa-solid fa-laptop-medical icone"></i> <!-- icone de saude-->
            <h2>Saúde</h2>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </p>
            <a href="" class="btn">Veja mais</a>
        </div>


        <div class="card-item">
            <i class="fa-solid fa-rocket icone"></i> <!-- icone de espaco-->
            <h2>Viajem</h2>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </p>
            <a href="" class="btn">Veja mais</a>
        </div>

    </div>
    </div>


</body>

</html>
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

DOC CSS

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Varela Round', sans-serif;
}

h1 {
    color: #db143c;
    font-size: 40px;
    text-align: center; /* centralizar texto */
    margin: 40px 0; /* margen superior e inferior */
}

.cards {
    width: 80%; /* ocupado 80% da tela */
    margin: auto; /* automaticamente sera centralizado */
    display: flex;
    justify-content: center; /* centralizar verdicalmente */
    align-items: center; /* centralizar horizontalmente */
    gap: 10px; /* espaço interno entre os elementos */
    flex-wrap: wrap; /* nao estourar a tela quando for menor */
}

.card-item{
    width: 30%;
    border: 1px solid #db143c; 
    border-radius: 5px; /* curva das bordas */
    text-align: center; /* textos centralizados */
    height: 350px; /* altura do card */
    padding: 5px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    transition: .3s; /* transição dos cards aparecerem */

}

.card-item:hover{
    transform: scale(1.1); /* zoom ao passar o mouse em cima do card */
}


.icone{
    font-size: 50px;
    color: #db143c;
    margin-bottom: 30px 0;
    transition: .2s;
}

.icone:hover{
    transform: rotate(360deg)
}

.card-item h2{
    font-size: 30px;
    margin-bottom: 20px;
}

.card-item p{
    font-weight: 500;
    margin-bottom: 30px; /* distancia do texto pro botão do link */
}

.btn{
    text-decoration: none;
    border: 2px solid #db143c;
    background-color: #db143c;
    color: #afff;
    font-weight: 800; /* negrito */
    padding: 8px 30px; /* tamanho da borda */
    border-radius: 70px; /* arredondando a borda */
    transition: .2s; /* demora da transição ao passar o mouse */
}

.btn:hover{ /* ao passar o mouse */
    background-color: transparent;
    color: #db143c;
}

@media(max-width:500px){
    .card-item{
        width: 80%;
    }
}


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
LINKS UTILIZADOS

https://fonts.google.com/specimen/Varela+Round?preview.size=35&preview.text=Oficina%20Web&preview.text_type=custom
https://fontawesome.com/icons/rocket?f=classic&s=solid
https://cdnjs.com/libraries/font-awesome
