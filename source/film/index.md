---
title: “电影发明以后，人类的生命至少比以前延长了三倍”
date: 2024-08-30 11:31:42
tags: ["电影", "生命"]
password: 20240809
message: 请在密码框中输入密码以查看视频
wrong_pass_message: 密码错误，请重新输入
---
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DPlayer Example</title>
    <!-- DPlayer CSS -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/dplayer/dist/DPlayer.min.css">
</head>
<body>
    <!-- DPlayer Container -->
    <div id="dplayer"></div>
    <!-- DPlayer JS -->
    <script src="https://cdn.jsdelivr.net/npm/dplayer/dist/DPlayer.min.js"></script>
    <!-- Initialize DPlayer -->
    <script>
        const dp = new DPlayer({
            container: document.getElementById('dplayer'),
            video: {
                url: './filmbase/test.mp4'
            },
        });
    </script>
</body>
</html>
