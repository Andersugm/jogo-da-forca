<div class="Menu">

    <div class="coluna">
        <div class="jogar">
            <a href="/jogo">Jogar</a>
        </div>
        
        <div class="sobre">
            <a href="/sobre">sobre</a>
        </div>
    </div>
    
</div>
<style>
    .Menu{
        background-image: url(fundo.gif.gif);
        height: 100%;
        position: absolute;
        width: 100%;
        background-size: cover;
    }
    .coluna{
        width: 250px;
        margin-left: 43%;
        margin-top: 25%;
        height: 170px;
    }
    
    .sobre{
        margin-top:10px;
        border: 3px solid black;
        text-align: center;
        border-radius: 30px;
        height: 70px;
        width: 200px;
        font-size: 35px;
        background-image: url(tecla2.png);
        background-size: cover;
        margin-left: 20%;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .jogar{
        border: 3px solid black;
        text-align: center;
        border-radius: 30px;
        width: 300px;
        height: 70px;
        font-size: 45px;
        background-image: url(tecla2.png);
        background-size: cover;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    a{
        text-decoration: none;
        color:orange;
        font-family: jogo da forca;
    }
    @font-face {
    
    font-family: 'jogo da forca' ;
    src: url('Sweet\ Scream\ Free.otf') format('opentype'),
    url('Sweet\ Scream\ Free.ttf') format('truetype');
    font-weight: normal;
    font-style: normal;
}
</style>