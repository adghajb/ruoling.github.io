````html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body {
            /* Flex是Flexible Box的缩写意为弹性盒子,设置后子元素的float、clear和vertical-align属性将失效 */
            display: flex;
            /* 让元素沿垂直主轴从上到下垂直排列 */
            flex-direction: column;
            /* 设置弹性盒子元素在主轴（横轴）方向上的对齐方式 */
            justify-content: center;
            /*  设置弹性盒子元素在侧轴（纵轴）方向上的对齐方式。 */
            align-items: center;
            background-color: #000;
            /* vh相对于视窗的高度 */
            min-height: 100vh;
        }

        a {
            position: relative;
            padding: 10px 30px;
            margin: 45px 0;
            color: #21ebff;
            text-decoration: none;
            font-size: 20px;
            /* 设置字母大写 */
            text-transform: uppercase;
            transition: 0.5s;
            overflow: hidden;
            /* -webkit-box-reflect: below 1px linear-gradient(transparent,#0003); */
        }

        a:hover {
            background-color: #21ebff;
            color: #111;
            box-shadow: 0 0 50px #21ebff;
            transition-delay: 0.5s;
        }

        a:nth-child(1) {
            /* 色相旋转 */
            filter: hue-rotate(115deg);
        }

        a:nth-child(3) {
            filter: hue-rotate(270deg);
        }

        a:hover::after,
        a:hover::before {
            width: 100%;
            height: 100%;
            transition-delay: 0s;
        }

        a::after,
        a::before {
            content: "";
            position: absolute;
            width: 10px;
            height: 10px;
            transition: 0.5s;
            transition-delay: 0.5s;
        }


        a::after {
            bottom: 0;
            right: 0;
            border-bottom: 2px solid #21ebff;
            border-right: 2px solid #21ebff;
        }

        a::before {
            top: 0;
            left: 0;
            border-top: 2px solid #21ebff;
            border-left: 2px solid #21ebff;
        }
    </style>
</head>

<body>
    <a href="#">button</a>
    <a href="#">button</a>
    <a href="#">button</a>
</body>

</html>
````
