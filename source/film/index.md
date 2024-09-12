---
title: “电影发明以后，人类的生命至少比以前延长了三倍”
date: 2024-08-30 11:31:42
tags: ["电影", "生命"]
password: ###
message: 请在密码框中输入密码以查看视频
wrong_pass_message: 密码错误，请重新输入
---
<head>
  <link href="https://vjs.zencdn.net/8.16.1/video-js.css" rel="stylesheet" />
  <script src="flv.min.js"></script>
  <!-- If you'd like to support IE8 (for Video.js versions prior to v7) -->
  <!-- <script src="https://vjs.zencdn.net/ie8/1.1.2/videojs-ie8.min.js"></script> -->

  <style>
    /* 默认样式 */
    .video-js {
      left: 70px;
      width: 800px;
      height: 500px;
    }

    /* 针对手机设备的样式调整 */
    @media screen and (max-width: 768px) {
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
  <video id="my-video" class="video-js" controls preload="auto" poster="./Picbase/JCL.webp">
    <source src="./filmbase/test.mp4" type="video/mp4">
  </video>
  <script>
    var videoElement = document.getElementById('my-video');
    // 检查 flv.js 支持情况
    if (flvjs.isSupported()) {
      var flvPlayer = flvjs.createPlayer({
        type: 'flv',
        url: '###'
      });
      flvPlayer.attachMediaElement(videoElement);
      flvPlayer.load();
      // 监听播放失败或流不可用的情况
      flvPlayer.on(flvjs.Events.ERROR, function(errorType, errorDetail) {
        console.error('FLV Error:', errorType, errorDetail);
        // 回退到 MP4 播放
        videoElement.src = './filmbase/test.mp4';
        videoElement.load();
        videoElement.play();
      });
      flvPlayer.play().catch(function(error) {
        console.error('FLV Play Error:', error);
        // FLV 播放失败时回退到 MP4
        videoElement.src = './filmbase/test.mp4';
        videoElement.load();
        videoElement.play();
      });
    } else {
      // 自动回退到 MP4 或 M3U8 源
      videoElement.load();
    }
  </script>

  <script src="https://vjs.zencdn.net/8.16.1/video.min.js"></script>
</body>
