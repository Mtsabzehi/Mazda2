<html lang="fa">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hashashin's Life</title>
    <style>
        body {
            font-family: 'Tahoma', Arial, sans-serif;
            background: url('https://biaupload.com/do.php?imgf=org-8323b74512921.jpg') no-repeat center center fixed;
            background-size: cover;
            margin: 0;
            padding: 0;
            direction: rtl; 
            text-align: right;
            color: #ffffff;
        }
        .container {
            max-width: 900px;
            margin: 160px auto;
            background: #0000009a;
            padding: 50px;
            border-radius: 20px;
            box-shadow: 0 0 50px #00000080;
            position: relative;
            overflow: hidden;
        }
        h1, h2 {
            color: #ff9300;
            text-align: center;
        }
        p {
            line-height: 1.8;
            font-size: 18px;
            color: #ffab34;
        }
        .pdf-container {
            margin-top: 20px;
            text-align: center;
        }
        iframe {
            width: 100%;
            height: 500px;
            border-radius: 10px;
            border: 2px solid #ffffff;
        }
        .download-btn {
            display: block;
            text-align: center;
            background: #ff9300;
            color: #ffffff;
            padding: 12px 20px;
            border-radius: 8px;
            text-decoration: none;
            font-size: 18px;
            font-weight: bold;
            margin-top: 15px;
            transition: 0.3s;
        }
        .download-btn:hover {
            background: #000000;
            color: #ff9300;
        }
        .language-buttons {
            text-align: center;
            margin-bottom: 20px;
        }
        .lang-btn {
            background: #ff9300;
            color: white;
            padding: 8px 16px;
            border: none;
            border-radius: 7px;
            font-size: 16px;
            cursor: pointer;
            margin: 7px;
            transition: 0.3s;
        }
        .lang-btn:hover {
            background: #000000;
            color: #ff9300  ;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="language-buttons">
            <button class="lang-btn" onclick="translateText('fa')">🇮🇷 فارسی</button>
            <button class="lang-btn" onclick="translateText('en')">🇬🇧 English</button>
            <button class="lang-btn" onclick="translateText('ar')">🇸🇦 العربية</button>
        </div>
        <h1 id="title">عنوان مقاله:</h1>
        <h2 id="subtitle">زندگی نامه و داستان کامل حشاشین</h2>
        <p id="description">
            این PDF به شما کمک و اطلاعاتی می‌دهد که بتوانید درباره زندگی‌نامه حسن صباح، بنیان‌گذار فرقه اسماعیلیه، اطلاعات کسب کنید.
        </p>
        <div class="pdf-container">
            <a href="https://biaupload.com/do.php?filename=org-fcbe8e4ad7a11.pdf" class="download-btn" download id="downloadText">📥 دانلود مقاله</a>
        </div>
    </div>
    <script>
        function translateText(lang) {
            const translations = {
                fa: {
                    title: "عنوان مقاله:",
                    subtitle: "زندگی نامه و داستان کامل حشاشین",
                    description: "این PDF به شما کمک و اطلاعاتی می‌دهد که بتوانید درباره زندگی‌نامه حسن صباح، بنیان‌گذار فرقه اسماعیلیه، اطلاعات کسب کنید.",
                    downloadText: "📥 دانلود مقاله"
                },
                en: {
                    title: ":   Article Title",
                    subtitle: "The Full Story of the Hashashin",
                    description: ".This PDF provides you with information about the life of Hassan Sabbah, the founder of the Ismaili sect",
                    downloadText: "📥 Download Article"
                },
                ar: {
                    title: "عنوان المقال:",
                    subtitle: "القصة الكاملة للحشاشين",
                    description: "يوفر لك هذا الملف معلومات عن حياة حسن صباح، مؤسس الطائفة الإسماعيلية.",
                    downloadText: "📥 تحميل المقال"
                }
            };
            document.getElementById("title").textContent = translations[lang].title;
            document.getElementById("subtitle").textContent = translations[lang].subtitle;
            document.getElementById("description").textContent = translations[lang].description;
            document.getElementById("downloadText").textContent = translations[lang].downloadText;
        }
    </script>

</body>
</html>
