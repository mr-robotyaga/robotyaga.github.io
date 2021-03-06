<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Happy New Year</title>
    <link rel="shortcut icon" href="tree" type="image/x-icon">
    <meta name="viewport" content="width=device-width, initial-scale=1">
</head>
<style>
    * {
        padding: 0;
        margin: 0;
        box-sizing: border-box;
        font-family: "Bal";
    }

    body {
        background: url(back.jpg);
        min-height: 100vh;
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center center;
    }

    .main {
        display: flex;
        justify-content: center;
        align-items: center;
        min-height: 100vh;
        width: 100%;
        background: url(https://i.gifer.com/3sjl.gif);
        background-position: center center;
        background-repeat: repeat;
        background-size: 65px;
        padding-left: 20px;
        padding-right: 20px;
    }

    .countdown {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .container {
        max-width: 1280px;
    }

    .title {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
    }

    .title__main {
        font-size: 90px;  
        margin: auto;
        color: white;
        display: flex;
        justify-content: center;
        align-items: center;
        padding-left: 30px;
        padding-right: 30px;
        -webkit-text-shadow: 11px 0px 0px rgb(255,0,28);
        -moz-text-shadow: 11px 0px 0px rgb(255,0,28);
        text-shadow: 11px 0px 0px rgb(255,0,28);
    }

    .title__year {
        font-size: 170px;
        height: 200px;
        margin: 0 auto;
        color: white;
        -webkit-text-shadow: 11px 0px 0px rgb(255,0,28);
        -moz-text-shadow: 11px 0px 0px rgb(255,0,28);
        text-shadow: 11px 0px 0px rgb(255,0,28);
        display: flex;
        justify-content: center;
        align-items: flex-end;
    }

    .timer__item {
        width: 230px;
        height: 230px;
        background-color: red;
        margin: 0 20px;
        font-size: 120px;
        color: white;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-content: center;
        align-items: center;
        -webkit-box-shadow: 11px 0px 0px 0px white;
        -moz-box-shadow: 11px 0px 0px 0px white;
        box-shadow: 11px 0px 0px 0px white;
        transition: 0.5s;
        cursor: pointer;
    }

    .timer__item:hover {
        color: rgb(255,0,28);
        background-color: white;
        -webkit-box-shadow: 11px 0px 0px 0px rgb(255,0,28);
        -moz-box-shadow: 11px 0px 0px 0px rgb(255,0,28);
        box-shadow: 11px 0px 0px 0px rgb(255,0,28);
    }

    .timer__item:hover ~ div {
        -webkit-text-shadow: 6px 0px 0px white;
        -moz-text-shadow: 6px 0px 0px white;
        text-shadow: 6px 0px 0px white;
        color: rgb(255,0,28);
    }

    .countdown__subtitle {
        display: flex;
        justify-content: center;
        align-content: center;
        align-items: center;
        font-size: 50px;
        color: white;
        -webkit-text-shadow: 6px 0px 0px rgb(255,0,28);
        -moz-text-shadow: 6px 0px 0px rgb(255,0,28);
        text-shadow: 6px 0px 0px rgb(255,0,28);
        padding: 10px 0;
        transition: 0.5s;
    }

    .img-container {
        width: 200px;
    }

    .img-container img {
        position: fixed;
        bottom: -5px;
        right: 50%;
        width: 350px;
        transform: translateX(50%);
    }

    @font-face {
        font-family: "Bal";
        src: url('Bal.ttf');
    }

    @media screen and (max-width: 1440px) {
        .timer__item {
            width: 200px;
            height: 200px;
        }

        .img-container img {
            width: 310px;
        }
    }

    @media screen and (max-width: 1224px) {
        .title__main {
            font-size: 80px;
        }

        .title__year {
            font-size: 160px;
            height: 170px;
        }

        .timer__item {
            width: 165px;
            height: 165px;
            font-size: 90px;
        }

        .countdown__subtitle {
            font-size: 40px;
        }
    }

    @media screen and (max-width: 1024px) {
        .img-container {
            width: 130px;
        }

        .title__main {
            width: 495px;
            line-height: 75px;
            margin-bottom: 10px;
            font-size: 80px;
            -webkit-text-shadow: 7px 0px 0px rgb(255,0,28);
            -moz-text-shadow: 7px 0px 0px rgb(255,0,28);
            text-shadow: 7px 0px 0px rgb(255,0,28);
        }

        .title__year {
            font-size: 140px;
            height: 155px;
            -webkit-text-shadow: 8px 0px 0px rgb(255,0,28);
            -moz-text-shadow: 8px 0px 0px rgb(255,0,28);
            text-shadow: 8px 0px 0px rgb(255,0,28);
        }

        .timer__item {
            width: 118px;
            height: 118px;
            font-size: 60px;
            -webkit-box-shadow: 7px 0px 0px 0px white;
            -moz-box-shadow: 7px 0px 0px 0px white;
            box-shadow: 7px 0px 0px 0px white;
        }

        .countdown__subtitle {
            font-size: 30px;
            -webkit-text-shadow: 4px 0px 0px rgb(255,0,28);
            -moz-text-shadow: 4px 0px 0px rgb(255,0,28);
            text-shadow: 4px 0px 0px rgb(255,0,28);
        }

        .timer__item:hover {
            -webkit-box-shadow: 7px 0px 0px rgb(255,0,28);
            -moz-box-shadow: 7px 0px 0px rgb(255,0,28);
            box-shadow: 7px 0px 0px rgb(255,0,28);
        }

        .timer__item:hover ~ div {
            -webkit-text-shadow: 4px 0px 0px white;
            -moz-text-shadow: 4px 0px 0px white;
            text-shadow: 4px 0px 0px white;
        }
    }

    @media screen and (max-width: 768px) {
        .countdown {
            flex-wrap: wrap;
            position: relative;
        }

        .countdown__item {
            width: 50%;
        }

        .title__main {
            width: 332px;
            line-height: 60px;
            margin-top: 10px;
            margin-bottom: 10px;
            font-size: 50px;
        }

        .countdown__subtitle {
            font-size: 30px;
            width: 140px;
        }

        .timer__item {
            margin: 0 0 0 10px;
        }

        .countdown__item:nth-child(5) {
            display: flex;
            flex-direction: column;
            align-items: flex-end;
        }

        .countdown__item:nth-child(5) .timer__item {
            margin-right: 10px;
        }

        .countdown__item:nth-child(2) {
            display: flex;
            flex-direction: column;
            align-items: flex-end;
        }

        .countdown__item:nth-child(2) .timer__item {
            margin-right: 10px;
        }

        .img-container {
            width: 0;
        }

        .img-container img {
            width: 350px;
            position: absolute;
            bottom: 0px;
        }
    }

    @media screen and (max-width: 425px){
        .img-container img {
            width: 250px;
        }

        .countdown {
            padding: 0 10px;
        }
    }

    

    
</style>
<body>
    <script type="text/javascript">

            function timer() {
            var nowDate = new Date();
            var achiveDate = new Date(2021, 0, 0);     
            var result = (achiveDate - nowDate) + 1000;
            var seconds = Math.floor((result / 1000) %60);
            var minutes = Math.floor((result/ 1000/ 60) %60);
            var hours = Math.floor((result/ 1000/ 60/ 60) %24);
            var days = Math.floor(result/ 1000/ 60/ 60/ 24);
            if (seconds < 10) seconds = '0' + seconds;
            if (minutes < 10) minutes = '0' + minutes;
            if (hours < 10) hours = '0' + hours;
            if (days < 10) days = '0' + days;      
            document.getElementById('days').innerText = days;    
            document.getElementById('hours').innerText = hours;    
            document.getElementById('minutes').innerText = minutes;    
            document.getElementById('seconds').innerText = seconds;  
                if (result < 0) {
                document.getElementById('days').innerText = "00";    
                document.getElementById('hours').innerText = "00";    
                document.getElementById('minutes').innerText = "00";    
                document.getElementById('seconds').innerText = "00"; 
            } 
            setTimeout(timer, 0);
        }
        window.onload = function() {
            timer();
        }
        
    </script>
    <div class="main">
        <div class="container">
            <div class="title">
                <h1 class="title__main">Countdown to New Year</h1>
                <div class="title__year">2021</div>
            </div>    
            <div class="countdown">
                <div class="countdown__item">
                    <div class="timer__item" id="days"></div>  
                    <div class="countdown__subtitle">days</div>             
                </div>
                <div class="countdown__item">
                    <div class="timer__item" id="hours"></div>  
                    <div class="countdown__subtitle">hours</div>             
                </div>
                <div class="img-container">
                    <img src="https://i.gifer.com/ZAc2.gif" alt="">
                </div>
                <div class="countdown__item">
                    <div class="timer__item" id="minutes"></div>  
                    <div class="countdown__subtitle">minutes</div>             
                </div>
                <div class="countdown__item">
                    <div class="timer__item" id="seconds"></div>  
                    <div class="countdown__subtitle">seconds</div>             
                </div>
            </div>
        </div>
    </div>              
</body>
</html>
