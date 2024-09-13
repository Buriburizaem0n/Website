---
title: Love U
date: 2024-08-30 11:11:04
tags:
---
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Love U</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background: linear-gradient(to right, #ff9a9e, #fecfef);
            font-family: 'Arial', sans-serif;
            display: flex;
            flex-direction: column;
            justify-content: center;
            min-height: 120vh;
        }
        .heartt {
            width: 120px;
            height: 120px;
            background-color: #e74c3c;
            position: relative;
            transform: translate(-50%, 0) rotate(-45deg); /* 平移让心形水平居中 */
            margin-bottom: 20px;
            animation: pulse 1s infinite;
            left: 50%; /* 使用百分比使心形居中 */
        }
        .heartt::before,
        .heartt::after {
            content: "";
            width: 120px;
            height: 120px;
            background-color: #e74c3c;
            border-radius: 50%;
            position: absolute;
        }
        .heartt::before {
            top: -60px;
            left: 0;
        }
        .heartt::after {
            left: 60px;
            top: 0;
        }
        .text {
            font-size: 4em;
            color: #ffffff;
            text-align: center;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
        }
        .text span {
            display: block;
            animation: bounce 2s infinite;
        }
        @keyframes pulse {
            0%, 100% {
                transform: scale(1) translate(-50%, 0) rotate(-45deg);
            }
            50% {
                transform: scale(1.1) translate(-50%, 0) rotate(-45deg);
            }
        }
        @keyframes bounce {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-10px);
            }
        }
    </style>
</head>
<body>
    <div class="heartt"></div>
    <div class="text">
        <span>I</span>
        <span>Love</span>
        <span>U</span>
    </div>
</body>
</html>
