


```html

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="css/style.css">
<style type="text/css">
    *{
        padding:0;
        margin:0px;
    }
    body{
        font-size:16px;
        color:#673929;
    }
    #container{
        width:900px;
        margin:0 auto;
    }
    #header{
        height:220px;
        margin-bottom:5px;
        position:relative;
    }
    #icon-list{
        position:absolute;
        top:170px;
        right:30px;
        width:130px;
        height:30px;
        /*font-size:0;*/
    }
    #nav{
        height:30px;
        line-height:30px;
        margin:5px;
        background-color:#09c;
        font:18px/30px;
        color:#fff;
        letter-spacing:2px;
        text-align:center;
    }
    a:link{
        color:#fff;
        text-decoration:none;
    }
    a:visited{
        color:#fff;
        text-decoration:none;
    }
    a:hover{
        color:yellow;
        text-decoration:none;
    }
    a:active{
        color:yellow;
        text-decoration:none;
    }
    #main{
        background-color:#000;
        height:2050px;
    }
    #aside{
        float:left;
        width:300px;
        height:500px;
        background-color:#6cf;
        text-align:center;
        font-size:14px;
    }
    #aside{
        margin:20px;
    }
    #imglist{
        width:130px;
        margin:0 auto;
    }
    .pol{
        width:85px;
        padding:10px;
        background-color:#eee;
        border:1px solid #bfbfbf;
        box-shadow:2px 2px 4px #aaa;
        border-radius:5px;
    }
    #imglist img{
        width:85px;
        height:95px;
        margin:0 auto;
    }
    .rotate-1eft{
        -webkit-transform:rotate(7deg);
        -ms-transform:rotate(7deg);
        -o-transform:rotate(7deg);
        transform:rotate(7deg);
    }
    .rotate-right{
        -webkit-transform:rotate(-7deg);
        -ms-transform:rotate(-7deg);
        -o-transform:rotate(-7deg);
        transform:rotate(-7deg);
    }
    #content{
        float:right;
        width:595px;
        height:2050px;
        margin-bottom:5px;
        background-color:#cff;
    }
    .subcon{
        width:570px;
        margin:10px auto;
        clear:both;
    }
    .subcon img{
        margin:5px;
        padding:5px;
        float:left;
        border:1px dashed #000;
    }
    .subcon .subtext{
        width:60%;
        float:left;
        margin:5px;
    }
    .subcon h2{
        margin:5px;
    }
    .subcon p{
        font:16px/2em;
    }
    #footer{
        height:60px;
        line-height:60px;
        background-color:#6cf;
        clear:both;
        text-align:center;
    }
    #1-fix{
        position:fixed;
        top:100px;
        left:5px;
    }
</style>
</head>
<body>
    <div id="container">
        <div id="header">
            <p><img src="web/coffee1.jpg" alt=""></p>
            <div id="icon-list">
                <img src="web/coffee1.jpg" alt=""> 
                <img src="web/coffee1.jpg" alt="">
                <img src="web/coffee1.jpg" alt="">
                <img src="web/coffee1.jpg" alt="">
            </div>
        </div>
        <div id="nav">
            <a href="#">咖啡MENU</a>
            <a href="#">咖啡COOK</a>
            <a href="#">咖啡STORV</a>
            <a href="#">咖啡NEWS</a>
            <a href="#">咖啡PARTY</a>
        </div>
        <div id="main">
            <div id="aside">
                <h2>咖啡MENU</h2>
                <table>
                    
                </table>
                <div id="imglist">
                    <div class="pol rotate-left"><img src="web/coffee1.jpg" alt=""></div>
                    <div class="pol rotate-right"><img src="web/coffee1.jpg" alt=""></div> 
                    <div class="pol rotate-left"><img src="web/coffee1.jpg" alt=""></div>
                    <div class="pol rotate-right"><img src="web/coffee1.jpg" alt=""></div>
                </div>
            </div>
            <div id="content">
                <div class="subcon">
                    <img src="web/coffee1.jpg" alt="">
                    <div class="subtext">
                        <h2>拿铁</h2>
                        <p></p>
                    </div>
                </div>
                <div class="subcon">
                    <img src="web/coffee1.jpg" alt="">
                    <div class="subtext">
                        <h2>卡布奇诺</h2>
                        <p></p>
                    </div>
                </div>
                <div class="subcon">
                    <img src="web/coffee1.jpg" alt="">
                    <div class="subtext">
                        <h2>摩卡</h2>
                        <p></p>
                    </div>
                </div>
                <div class="subcon">
                    <img src="web/coffee1.jpg" alt="">
                    <div class="subtext">
                        <h2>浓缩咖啡</h2>
                        <p></p>
                    </div>
                </div>
            </div>
        </div>
        <div id="footer">
            <p>web前端开发</p>
        </div>
    </div>
<div>
    <img src="" alt="">
</div>
</body>
</html>


```


