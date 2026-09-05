# surpriseu<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>اولین سالگرد ازدواجمان</title>
    <style>
        body {
            margin: 0;
            padding: 20px;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #fdfcf0;
            font-family: 'Tahoma', sans-serif;
            overflow: hidden;
            text-align: center;
        }

        .container {
            max-width: 600px;
        }

        h1 {
            font-size: 2.2rem;
            color: #4a4a4a;
            margin-bottom: 20px;
            animation: fadeIn 2s ease-in;
            line-height: 1.6;
        }

        p {
            font-size: 1.2rem;
            color: #6b6b6b;
            line-height: 1.8;
            margin-bottom: 30px;
            animation: fadeIn 3s ease-in;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        #playButton {
            padding: 12px 30px;
            font-size: 1.1rem;
            background-color: #d4a373;
            color: white;
            border: none;
            border-radius: 30px;
            cursor: pointer;
            transition: 0.3s;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
        }

        #playButton:hover {
            background-color: #bc8a5f;
            transform: scale(1.05);
        }
    </style>
</head>
<body
    <div class="container" id="content">
        <h1 id="titleText">اولین سالگرد با هم بودنمون مبارک... ❤️</h1>
        <p id="descText">  یک سال از روزی که دست‌هامون رو توی دست هم گذاشتیم گذشت.<b
            مرسی که در کنار تمام بالا و پایین‌ها، پناه‌می و با حضور قشنگت به زندگی‌ام دلگرمی میدی.<br>  این اولین سالگرد، تازه شروع قشنگی‌های مسیرمونه...
        <button id="playButtoonclick="playMusic()">پخش موزیک خاطره‌مون 🎵</button>
    </div>

    <!-- فایل موسیقی -->
    <audio id="myAudio">
        <source src="music.mp3" type="audio/mpeg">
        مرورگر شما از پخش موسیقی پشتیبانی نمی‌کند.
    </audio>

    <script>
        function playMusic() {
            var audio = document.getElementById("myAudio");
            var btn = document.getElementById("playButton");
            
            audio.play();
            
            // مخفی کردن دکمه و زیباتر کردن فضا بعد از کلیک
            btn.style.display = "none";
            
            // تغییر متن برای تاثیرگذاری بیشتر
            document.getElementById("titleText").innerHTML = "همیشه کنارت می‌مونم... 💍";
            document.getElementById("descText").innerHTML = "تا ابد و یک روز، عاشقتم عشق من.";
        }
    </script>

</body>
</html>
