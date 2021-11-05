![Hi! I'm Raymundo Mora (1)](https://user-images.githubusercontent.com/92943544/140455801-b87ee727-bb4c-4645-9bf7-f4fc4609c155.gif)
# About Me 
![Alt text](./assets/loading/index.html)

# Socials
<a href="https://www.instagram.com/theraymundomora/"><img src="https://user-images.githubusercontent.com/92943544/140460116-71fa1625-18f6-4f6f-9844-9d72308b45c1.png" style="width:82px; height:86px" title="Instagram" alt="Instagram"></a> 
<a href="https://www.linkedin.com/in/raymundo-mora/"><img src="https://user-images.githubusercontent.com/92943544/140461482-aa8e1275-c852-489a-897a-64da462987df.png" style="width:101.12962963px; height:86px" title="LinkedIn" alt="LinkedIn"></a>

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ellipsis Loading - Sagar Developer</title>
    <style>
        body {
            background-color: #efefef;
            text-align: center;
        }

        .container {
            width: 200px;
            height: 200px;
            display: inline-block;
            overflow: hidden;
            margin-top: 200px;
        }

        .loader {
            width: 100%;
            height: 100%;
            position: relative;
            transform: translateZ(0) scale(1);
            backface-visibility: hidden;
            transform-origin: 0 0;
        }

        .loader div {
            position: absolute;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            transform: translate(80px, 80px) scale(1);
            background: #5be1d1;
            box-sizing: content-box;
            animation: loading 1s infinite cubic-bezier(0, 0.5, 0.5, 1);
        }

        .loader div:nth-child(1) {
            background: #a260f4;
            transform: translate(148px, 80px) scale(1);
            animation: loading-r 0.25s infinite cubic-bezier(0, 0.5, 0.5, 1), loading-c 1s infinite step-start;
        }

        .loader div:nth-child(2) {
            animation-delay: -0.25s;
            background: #5be1d1;
        }

        .loader div:nth-child(3) {
            animation-delay: -0.5s;
            background: #a260f4;
        }

        .loader div:nth-child(4) {
            animation-delay: -0.75s;
            background: #f8b26a;
        }

        .loader div:nth-child(5) {
            animation-delay: -1s;
            background: #ed296d;
        }

        @keyframes loading {
            0% {
                transform: translate(12px, 88px) scale(0);
            }

            25% {
                transform: translate(12px, 88px) scale(0);
            }

            50% {
                transform: translate(12px, 88px) scale(1);
            }

            75% {
                transform: translate(80px, 88px) scale(1);
            }

            100% {
                transform: translate(148px, 88px) scale(1);
            }
        }

        @keyframes loading-r {
            0% {
                transform: translate(148px, 88px) scale(1);
            }

            100% {
                transform: translate(148px, 88px) scale(0);
            }
        }

        @keyframes loading-c {
            0% {
                background: #5be1d1;
            }

            25% {
                background: #ed296d;
            }

            50% {
                background: #f8b26a;
            }

            75% {
                background: #a260f4;
            }

            100% {
                background: #5be1d1;
            }
        }
    </style>
</head>

<body>
    <div class="container">
        <div class="loader">
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
        </div>
    </div>
</body>

</html>
        
