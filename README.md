<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>



  <style>
    #screen {
      width: 9999px;
      height: 9999px;
      animation: 8s donghua infinite;
    }

    /**css 定义风格 animation甚至一个轮回8s 4张图片**/

    #screen img {
      float: left;

    }

    /**名为tv中的图片只显示173*180的 也就是一张图片多余的隐藏起来**/
    #tv {
      width: 173px;
      height: 180px;
      overflow: hidden;
    }

    /**关键帧 对于donghua中的图片每一个显示8s的1/4**/
    @keyframes donghua {
      0% {}

      25% {
        transform: translateX(0px);
      }

      50% {
        transform: translateX(-173px);
      }

      75% {
        transform: translateX(-346px);
      }

      100% {
        transform: translateX(-519px);
      }

    }
  </style>
</head>

<body>
  <div id="tv">
    <div id="screen">
      <img src="OC.jpg">
      <img src="OIC.jpg">
      <img src="OIP-C.jpg">
      <img src="PP.jpg">
    </div>
  </div>
</body>

</html>
