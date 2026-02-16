<html lang="en">
<head>
    <title>Choose Contact to Call</title>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body { 
            font-family: Arial, sans-serif; 
            text-align: center; 
            padding: 50px 20px; 
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            margin: 0;
            min-height: 100vh;
        }
        h1 { 
            color: #333; 
            font-size: 24px;
            margin-bottom: 40px;
        }
        .contact { 
            display: block; 
            margin: 25px auto; 
            padding: 20px 40px; 
            font-size: 20px; 
            color: white; 
            text-decoration: none; 
            border-radius: 15px; 
            max-width: 350px;
            box-shadow: 0 8px 16px rgba(0,0,0,0.2);
            transition: transform 0.2s;
        }
        .contact:hover, .contact:active {
            transform: scale(1.05);
        }
        .website { 
            display: block; 
            margin: 25px auto; 
            padding: 15px 30px; 
            font-size: 18px; 
            color: white; 
            text-decoration: none; 
            border-radius: 15px; 
            max-width: 350px;
            box-shadow: 0 8px 16px rgba(0,0,0,0.2);
            transition: transform 0.2s;
            background: #FF9800;
        }
        .website:hover, .website:active {
            transform: scale(1.05);
        }
        .person1 { background: #4CAF50; }
        .person2 { background: #2196F3; }
        @media (max-width: 480px) {
            h1 { font-size: 20px; }
            .contact, .website { font-size: 18px; padding: 18px 35px; }
        }
    </style>
</head>
<body>
    <h1>Choose who to call:</h1>
    <a href="tel:+918856093580" class="contact person1">Ritwik Jarulkar<br><span style="font-size:16px;">+91 88560 93580</span></a>
    <a href="tel:+917038252813" class="contact person2">Vijay Mahanur<br><span style="font-size:16px;">+91 70382 52813</span></a>
    <a href="https://vrmedirent.in/" target="_blank" class="website">Visit VR Medirent Website</a>
    <p style="color:#666; font-size:14px; margin-top:30px;">Tap to dial • Works on all phones</p>
</body>
</html>
