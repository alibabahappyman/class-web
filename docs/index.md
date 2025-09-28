<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>Typed.js</title>
    <script src="https://unpkg.com/typed.js@2.1.0/dist/typed.umd.js"></script>
    <link rel="stylesheet" href="./CSS/custom-fullscreen-video.css">
    <link rel="stylesheet" href="./CSS/pixel-font.css">
    <link rel="stylesheet" href="./CSS/font-family.css">
    <style>
        /* 给打字容器的包裹层加 flex，不影响 body 全局 */
        .typed-wrapper {
            min-height: 150px; 
            display: flex;
            justify-content: flex-start; /* 水平居左 */
            align-items: flex-end; /* 垂直居右 */
            padding-left: 50px;
            margin: 300px 0 0 0; /* 上下留空，和其他元素隔开 */
            width:100%;
            /*overflow-x: auto;
            overflow-y: hidden;*/
        }
        #element {
            font-size: 2rem;
            color: #f0f0f0;
            text-shadow: 1px 0 0 #888,-1px 0 0 #888;/*描边*/
            font-weight: 350;/*字体粗细*/
            min-width: 1000px;
            /*white-space: nowrap;*//*不换行*/
            /*margin: 0 auto;*/
            line-height: 1.6;
        }
    </style>
</head>
<body>
    <!-- 包裹层 -->
    <div class="typed-wrapper">
        <span id="element"></span>
    </div>
    <div class="fullscreen-video">
    <video 
        src="./images/littleprince3.mp4" autoplay muted loop playsinline>
    </video>
</div>
    <script>
        var typed = new Typed("#element", {
            strings: [
                "如果不去遍历世界，",
                "我们就不知道什么是我们精神和情感的寄托，",
                "但我们一旦遍历了世界，",
                "却发现我们再也无法回到那美好的地方去了。",
                "当我们开始寻求，",
                "我们就已经失去，",
                "而我们不开始寻求，",
                "我们根本无法知道自己身边的一切是如此可贵。",
                "审判自己比审判别人难多了。",
                "如果你成功地正确审判了自己，",
                "那么你就是一个真正的智者了。",
                "Robert Frost said,",
                "Two roads diverged in a wood,",
                "and I took the one less traveled by,",
                "and that has made all the difference.",
                "Are you alive or just existing?",
                "Carpe diem,",
                "Seize the day, boys.",
                "Make your lives extraordinary."
            ],
            typeSpeed: 100,
            startDelay: 600, 
            backSpeed: 60,
            smartBackspace: true,
            /*wordBreak: true;*//*单词差分。回退不破坏完整性*/
            shuffle: false,
            backDelay: 1500,
            fadeOut: false,
            loop: true,
            loopCount: Infinity,
            showCursor: true,
            cursorChar: "|",
            autoInsertCss: true,
            contentType: "html"
        });
    </script>
</body>
</html>