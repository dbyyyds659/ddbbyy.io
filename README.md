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
      <img src="https://tse4-mm.cn.bing.net/th/id/OIP-C.oISYAs_TW3QQfP7KKf23MQAAAA?w=173&h=180&c=7&r=0&o=5&pid=1.7
      ">
      <img src="https://tse1-mm.cn.bing.net/th/id/OIP-C.X7dHUsgYc8hdwZQcVPH3YwAAAA?w=173&h=180&c=7&r=0&o=5&pid=1.7
      ">
      <img src="https://tse1-mm.cn.bing.net/th/id/OIP-C.BB2jro7mNeVD7SXeEUIBegAAAA?w=173&h=180&c=7&r=0&o=5&pid=1.7
      ">
      <img src="https://tse4-mm.cn.bing.net/th/id/OIP-C._seZfNgc8zA17aub-5hw7AAAAA?w=173&h=180&c=7&r=0&o=5&pid=1.7
      ">
    </div>
  </div>
</body>

</html>
