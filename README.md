<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restaurant Menu</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 20px;
        }
        iframe {
            border: none;
        }
        button {
            margin: 5px;
            padding: 10px 20px;
            font-size: 16px;
        }
    </style>
</head>
<body>
    <h1>Restaurant Menu</h1>
    <div id="menu-container">
        <iframe src="YOUR_PDF_LINK_HERE" width="100%" height="600px"></iframe>
    </div>
    <h2>Translate Menu</h2>
    <div id="translate-container">
        <button onclick="translateMenu('en')">English</button>
        <button onclick="translateMenu('es')">Spanish</button>
        <button onclick="translateMenu('fr')">French</button>
        <!-- Add more languages as needed -->
    </div>
    <script>
        function translateMenu(lang) {
            const pdfUrl = 'YOUR_PDF_LINK_HERE'; // Original PDF URL
            window.open(`https://translate.google.com/translate?hl=&sl=auto&tl=${lang}&u=${pdfUrl}`, '_blank');
        }
    </script>
</body>
</html>
