<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PortFolio</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@500&display=swap');

.back{
    background-color: rgb(0, 0, 0);
    height: 100vw;
    margin: 8px;
    border-radius: 15px;
}
::-webkit-scrollbar{
    width: .01px;
}
.TopContainer{
    display: grid;
    height: auto;
    border-radius: 15px 15px 0px 0px;
    grid-template-areas: 
    'left right';
}
.box1{
    grid-area: left;
    height: auto;
    width: 50%;
}
.box2{
    grid-area: right;
    width: 62%;
    height: 375px;
    right: 16px;
    overflow: hidden;
    border-top-right-radius: 15px;
    content: '';
    background-image: url('hero.jpg');
    position: absolute;
}
.blackbox{
    background-image: linear-gradient(rgba(255, 255, 255, 0),black);
    height: 377px;
    width: 70%;
    right: .2px;
    position: relative;
    width: auto;
}
.blackboxbefore{
    background-image: linear-gradient(-90deg,rgba(255, 255, 255, 0),black);
    height: 377px;
    width: 69%;
    top: -100%;
    right: 1px;
    margin-top: -2px;
    position: relative;
    width: auto;
}
.textcontainer{
    align-items: center;
    justify-content: center;
}
.text1{
    margin-left: 15%;
    margin-top: 10.5%;
    color: white;
    position: relative;
    font-size: 300%;
    font-family: 'Poppins', sans-serif;
}
.text2{
    color:rgb(48, 18, 156);
    margin-left: 15%;
    font-family: 'Poppins', sans-serif;
    font-size: 450%;
    margin-bottom: 13px;
}
.text3{
    color: white;
    margin-left: 15%;
    margin-bottom: 12%;
    font-size: 130%;
    font-family: 'Poppins', sans-serif;
    letter-spacing: 5px;
}
.SecondContainer{
    margin-top: 5.5%;
    display: grid;    
    justify-content: center;
    grid-gap: 40px;
    overflow: hidden;
    height: 200px;
    overflow: scroll;
    grid-template-areas: 
    'left leftsec middle rightSec right';
}
.black{
    opacity: 70%;
    height: 150px;
    width: 250px;
    border-radius: 10px;
    transition: all .6s;    
}
.black:hover{
    opacity: 100%;
    position: relative;
    height: 165px;
    width: 265px;
    cursor: pointer;
}
.box01{
    grid-area: left;
    background-image: url('8401.jpg');
    background-size: cover;
    background-repeat: no-repeat;
}
.box02{
    grid-area: leftsec;
    background-image: url('graduate.jpg');
    background-size: cover;
    background-repeat: no-repeat;
}
.box03{
    grid-area: middle;
    background-image: url('avatar.jpg');
    background-size: cover;
    background-repeat: no-repeat;
}
.box04{
    grid-area: rightSec;
    background-image: url('school.jpg');
    background-size: cover;
    background-repeat: no-repeat;
}
.box05{
    grid-area: right;
    background-image: url('mail.jpg');
    background-size: cover;
    background-repeat: no-repeat;
}
.scroll{
    text-align: center;
    width: 100%;
}
.svgfile{
    width: 30px;
    position: relative;
    top: -20px;
    animation: scrollsvg 1.2s infinite;
    animation-timing-function: ease;
    animation-direction: alternate-reverse;
}

@keyframes scrollsvg {
    0%{
        top: -20px;
    }
    100%{
        top: 5px;
    }
}
.scrollClick:hover{
    cursor: pointer;
}

    </style>
</head>
<body>
    <div class="back">
        <div class="TopContainer">
            <div class="box1">
                <div class="textcontainer">
                    <div class="text1">This is me</div>
                    <div class="text2">Sukanta</div>
                    <div class="text3">A Web Developing Enthuciast</div>
                </div>
            </div>
            <div class="box2">
                <div class="blackbox"></div>
                <div class="blackboxbefore"></div>
            </div>
        </div>
        <div class="SecondContainer">
                <div class="black box01"></div>
                <div class="black box02"></div>
                <div class="black box03"></div>
                <div class="black box04"></div>
                <div class="black box05"></div>
        </div>
        <section class="scroll">
           <a class="scrollClick" href="#"><img src="down-arrow-svgrepo-com.svg" class="svgfile"></img></a>
        </section>
    </div>
</body>
</html>
