!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="vewport" content="width=device-width, initial-scale=1.0">
    <title>Pingüino sobre Fondo de Nieve</title>
    <style>
       
        .container {
            position: relative;
            width: 500px; 
            height: 500px;
        }

     
        .snow-background {
            position: absolute;
            top: 0;
            left: 0;
            width: 500%;
            height: 500%;
            background-image: url(https://img.freepik.com/vector-gratis/ilustracion-diseno-plano-paisaje-invernal_23-2149167523.jpg);
            background-size: cover;
            background-position: center;
            z-index: 1;
        }
        .container {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #e0f7fa; 
        }

        
        .penguin {
            position: relative;
            width: 160px;
            height: 200px;
            background-color: #000;
            border-radius: 80px 80px 100px 100px;
        }

      
        .penguin::before {
            content: '';
            position: absolute;
            top: 30px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 130px;
            background-color: #fff;
            border-radius: 50%;
        }

       
        .eye {
            position: absolute;
            top: 40px;
            width: 20px;
            height: 20px;
            background-color: #fff;
            border-radius: 50%;
        }
        .eye.left {
            left: 45px;
        }
        .eye.right {
            right: 45px;
        }

        
        .eye::after {
            content: '';
            position: absolute;
            top: 4px;
            left: 5px;
            width: 10px;
            height: 10px;
            background-color: #000;
            border-radius: 50%;
        }

        
        .cheek {
            position: absolute;
            top: 70px;
            width: 15px;
            height: 15px;
            background-color: #fdd;
            border-radius: 50%;
        }
        .cheek.left {
            left: 30px;
        }
        .cheek.right {
            right: 30px;
        }

       
        .beak {
            position: absolute;
            top: 70px;
            left: 50%;
            transform: translateX(-50%);
            width: 20px;
            height: 15px;
            background-color: #ffcc00;
            border-radius: 50%;
        }
        .beak::before {
            content: '';
            position: absolute;
            top: 6px;
            left: 0;
            width: 20px;
            height: 15px;
            background-color: #ffcc00;
            border-radius: 50%;
        }

       
        .foot {
            position: absolute;
            bottom: 0;
            width: 30px;
            height: 20px;
            background-color: #ffcc00;
            border-radius: 50%;
        }
        .foot.left {
            left: 35px;
        }
        .foot.right {
            right: 35px;
        }

        
        .wing {
            position: absolute;
            top: 60px;
            width: 40px;
            height: 90px;
            background-color: #000;
            border-radius: 50%;
        }
        .wing.left {
            left: -20px;
            transform: rotate(-20deg);
        }
        .wing.right {
            right: -20px;
            transform: rotate(20deg);
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="penguin">
            <div class="eye left"></div>
            <div class="eye right"></div>
            <div class="cheek left"></div>
            <div class="cheek right"></div>
            <div class="beak"></div>
            <div class="wing left"></div>
            <div class="wing right"></div>
            <div class="foot left"></div>
            <div class="foot right"></div>
        </div>
    </div>
</body>
</html>
        
