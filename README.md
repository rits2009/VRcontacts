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
            position: relative;
        }
        .contact:hover, .contact:active {
            transform: scale(1.05);
        }
        .contact span {
            font-size: 16px;
        }
        .masked-num {
            color: #ddd !important;
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
    <a href="tel:+918856093580" class="contact person1" data-full-num="+91 88560 93580">
        Ritwik Jarulkar<br><span class="masked-num">+91 ***** 3580</span>
    </a>
    <a href="tel:+917038252813" class="contact person2" data-full-num="+91 70382 52813">
        Vijay Mahanur<br><span class="masked-num">+91 ***** 2813</span>
    </a>
    <a href="https://vrmedirent.in/" target="_blank" class="website">Visit VR Medirent Website</a>
    <p style="color:#666; font-size:14px; margin-top:30px;">Tap to dial • Works on all phones</p>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const contacts = document.querySelectorAll('.contact');
            contacts.forEach(contact => {
                contact.addEventListener('click', function(e) {
                    // Optional: Briefly show full number on tap before dialing (for reassurance)
                    const span = this.querySelector('span');
                    const fullNum = this.getAttribute('data-full-num');
                    if (fullNum && span) {
                        span.textContent = fullNum;
                        span.classList.remove('masked-num');
                        // Reset after short delay (dialing happens instantly)
                        setTimeout(() => {
                            span.textContent = span.textContent.replace(/(\+91\s)\d{5}/, '$1*****');
                            span.classList.add('masked-num');
                        }, 500);
                    }
                });
            });
        });
    </script>
</body>
</html>
