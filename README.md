[submarine.html](https://github.com/user-attachments/files/34859492/submarine.html)Creative Coding 1 WiSe26/27 <br>
Eine Github Seite von Marie Späth <br>
<br>
[Mein Prototyp.docx](https://github.com/user-attachments/files/33597824/Mein.Prototyp.docx)
<br>


https://github.com/user-attachments/assets/a133fff7-0b66-4c57-af10-ce5023496950


<br>
Mein nachgestellte Instagramseite auf Figma <br> 
https://www.figma.com/community/file/1701290130011390542
<br>
<br>
Hier mein Internetseite.<br>
Das mit dem Icon erstellen hat an sich Funktioniert, allerdings konnte ich es noch nicht so einstellen, damit es eine Funktion hat. <br>
[Instagram.html](https://github.com/user-attachments/files/34553950/Instagram.html)
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Instagram</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1 class="Instagram">Instagram</h1>
<p>Willkommen auf meiner Seiter. Ich bin Marie. ^^</p>
<br>

    <div class="post">
    <img src="bilder/ich vor haustuere.jpg" alt="Mein bild" class="post-bild">
    <img src="bilder/Herz schwarz.svg" alt="gefaellt mir" class="like-icon">
    </div>

    <div class="post">
    <img src="bilder/Tedy schlaeft auf mir.jpg" alt="Mein bild" class="post-bild">
    <img src="bilder/Herz schwarz.svg" alt="gefaellt mir" class="like-icon">
    </div>

    <div class="post">
    <img src="bilder/VfB mit Hoeness.jpg" alt="mein bild" class="post-bild">
    <img src="bilder/Herz schwarz.svg" alt="gefaellt mir" class="like-icon">
    </div>

    <div class="post">
    <img src="bilder/Autogram mit Peter und Astrid.jpg" alt="mein bild" class="post-bild">
    <img src="bilder/Herz schwarz.svg" alt="gefaellt mir" class="like-icon">
    </div>

    <script src="script.js"></script>
</body>
</html>

<br>
<br>
<br>

Hier ist meine Codierung für mein U-Boot. <br>
<br>

[Uploading submarine.html<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>U-Boot</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>    
    <img src="submarine assets-02.png" class="background">
    
    <div class="blasen">
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
    </div>

    <img src="submarine assets-01.png" class="submarine-container">
   
    <div class="submarine-container">
        <div class="scheinwerfer"></div>
    </div>

    <img src="submarine assets-03.png" class="turbine">

    <audio controls loop>
        <source src="tiefsee coding.wav" type="audio/wav">
    </audio>

</body>

</html>…]()


 <br>
 <br>
 <br>

Ich füge einfach mal mein CSS auch hinzu, falls dies benötigt wird. <br>
<br>
[style.css](https://github.com/user-attachments/files/34859390/style.css)
body{
    padding: 0%;
}
img{
    position: absolute;

}

.background{
    width: 100%;
    height: 100%;
}

.submarine-container{
    position: absolute;
    top: calc((100% - 500px)/2);
    left: calc((100% - 500px)/2);
    
    animation: float 3s linear infinite;
}

.turbine{
    top: calc(45% - 39px/2);
    left: calc(50% - 188px/2);
    animation: engineRotation 2s linear infinite, float 3s linear infinite;
}

@keyframes engineRotation {
    0% {
        transform: rotate(0);
    }
    100% {
        transform: rotate(360deg);
    }
}

@keyframes float {
    0% {
        translate: 0 0;
    }

    25% {
        translate: 0 -20px;
    }

    75% {
        translate: 0 20px;
    }

    100% {
        translate: 0 0;
    }
}

.scheinwerfer {
    position: relative;
    width: 250px;
    height: 100px;
    top: 355px;
    left: 420px;
    background: linear-gradient(to right, rgba(176, 224, 239, 0.82), transparent);
    clip-path: polygon(0 40%, 100% 0, 100% 100%, 0 60%);
    z-index: 0;
    pointer-events: none;
    transform: rotate(43deg);
}

.blasen span{
    position: absolute;
    left: calc((85% - 300px)/2);
    top: calc((110% - 100px)/2);
    width: 30px;
    height: 30px;
    border: 2px solid rgba(148, 219, 240, 0.82);
    border-radius: 50%;
    animation: blasenBewegung 3.7s linear infinite;
    background: radial-gradient(circle at 38% 35%, rgba(230, 210, 255, 0.9)5%, transparent 35%); 
}

.blasen span:nth-child(2){
    left: calc((125% - 170px)/2);
    top: calc((120% - 90px)/2);
    width: 12px;
    height: 12px;
    border: 2px solid rgba(148, 219, 240, 0.82);
    border-radius: 50%;
    animation: blasenBewegung 5s linear infinite;
}

.blasen span:nth-child(3){
    left: calc((75% - 220px)/2);
    top: calc((115% - 100px)/2);
    width: 15px;
    height: 15px;
    border: 2px solid rgba(148, 219, 240, 0.82);
    border-radius: 50%;
    animation: blasenBewegung 3s linear infinite;
}

.blasen span:nth-child(4){
    left: calc((85% - 210px)/2);
    top: calc((100% - 120px)/2);
    width: 20px;
    height: 20px;
    border: 2px solid rgba(148, 219, 240, 0.82);
    border-radius: 50%;
    animation: blasenBewegung 4s linear infinite;
}

.blasen span:nth-child(5){
    left: calc((105% - 240px)/2);
    top: calc((110% - 140px)/2);
    width: 25px;
    height: 25px;
    border: 2px solid rgba(148, 219, 240, 0.82);
    border-radius: 50%;
    animation: blasenBewegung 3.5s linear infinite;
}

.blasen span:nth-child(6){
    left: calc((85% - 260px)/2);
    top: calc((110% - 180px)/2);
    width: 15px;
    height: 15px;
    border: 2px solid rgba(148, 219, 240, 0.82);
    border-radius: 50%;
    animation: blasenBewegung 3s linear infinite;
}

.blasen span:nth-child(7){
    left: calc((85% - 220px)/2);
    top: calc((120% - 230px)/2);
    width: 25px;
    height: 25px;
    border: 2px solid rgba(148, 219, 240, 0.82);
    border-radius: 50%;
    animation: blasenBewegung 3.5s linear infinite;
}



@keyframes blasenBewegung{
    from{
        transform: translateX(0);
    }

    to{
        transform: translateX(-700px);
    }
}
<br>
<br>
