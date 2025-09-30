<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>Typed.js</title>
    <script src="https://unpkg.com/typed.js@2.1.0/dist/typed.umd.js"></script>
    <style>
        /* 给打字容器的包裹层加 flex，不影响 body 全局 */
        .typed-wrapper {
            min-height: 150px; 
            display: flex;
            justify-content: flex-start; /* 水平居左 */
            align-items: flex-end; /* 垂直居右 */
            padding-left: 10px;
            margin: 300px 0 0 0; /* 上下留空，和其他元素隔开 */
            width:100%;
            /*overflow-x: auto;
            overflow-y: hidden;*/
        }
        #element {
            font-size: 25px;
            color: #f0f0f0;
            text-shadow: 1px 0 0 #888,-1px 0 0 #888;/*描边*/
            font-weight: 300;/*字体粗细*/
            min-width: 500px;
            /*white-space: nowrap;*//*不换行*/
            margin-left: 10px;
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
                "The reason for the shining of the stars is that",
                "everyone can find his own star.",
                "In one of them I shall be laughing.",
                "And so it will be as if all the stars were laughing,",
                "when you look at the sky at night.",
                "The time you spent on your rose is what makes your rose so important.",
                "It is only with the heart that one can see rightly,",
                "what isessential is invisible to the eye.",
                "In the vast universe,",
                "Our life is about constantly discovering meaning.",
                "Live with dedication, no need to constantly strive and strive",
                "But in this journey,",
                "feel it with your heart",
                "From the small things around me",
                "Searching for the Meaning of Journey",
                "Robert Frost said,",
                "Two roads diverged in a wood,",
                "and I took the one less traveled by,",
                "and that has made all the difference.",
                "Are you alive or just existing?",
                "Carpe diem,",
                "Seize the day, boys.",
                "Make your lives extraordinary."
            ],
            typeSpeed: 30,
            startDelay: 600, 
            backSpeed: 20,
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