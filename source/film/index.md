---
title: “电影发明以后，人类的生命至少比以前延长了三倍”
date: 2024-08-30 11:31:42
tags: ["电影", "生命"]
password: 20240809
message: 请在密码框中输入密码以查看视频
wrong_pass_message: 密码错误，请重新输入
---
<head>
  <link href="https://vjs.zencdn.net/8.16.1/video-js.css" rel="stylesheet" />
  <!-- 如果需要支持 IE8 (Video.js 版本7之前) -->
  <!-- <script src="https://vjs.zencdn.net/ie8/1.1.2/videojs-ie8.min.js"></script> -->

  <style>
    /* 默认样式 */
    .video-js {
      left: 70px;
      width: 800px;
      height: 500px;
    }

    /* 针对手机设备的样式调整 */
    @media screen and (max-width: 1300px) {
      .video-js {
        width: 100%;
        height: 0;
        left: 0;
        padding-top: 56.25%; /* 16:9 比例 */
        position: relative;
      }
      .video-js iframe {
        position: absolute;
        top: 0;
        width: 100%;
        height: 100%;
      }
    }
  </style>
</head>

<body>
  <video
    id="my-video"
    class="video-js"
    controls
    preload="auto"
    poster="./Picbase/JCL.webp"
    data-setup="{}"
  >
    <source src="https://hls.luoyangdonghui.de/hls/Mjs7Bst2v38D1T6oBShFSLkxWzWWweAl809.m3u8" type="application/x-mpegURL" />
    <source src="./filmbase/test.mp4" type="video/mp4" />
    <p class="vjs-no-js">
      Love U Forever
      <a href="https://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
    </p>
  </video>

  <script src="https://vjs.zencdn.net/8.16.1/video.min.js"></script>
</body>
