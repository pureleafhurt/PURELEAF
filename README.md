<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PURELEAF</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #1a1a1a;
            color: white;
            text-align: center;
            padding: 20px;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
            background-color: #282828;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .buttons {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(45%, 1fr));
            gap: 10px;
            margin-top: 20px;
        }
        .button {
            padding: 8px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 14px;
            text-align: center;
        }
        .button:hover {
            background-color: #45a049;
        }
        .chat-box {
            margin-top: 20px;
            background-color: #333;
            border-radius: 10px;
            padding: 10px;
            max-height: 200px;
            overflow-y: auto;
            box-shadow: inset 0 4px 6px rgba(0, 0, 0, 0.2);
        }
        .chat-message {
            background-color: #4CAF50;
            color: white;
            padding: 10px;
            margin: 5px 0;
            border-radius: 5px;
            text-align: left;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>WITAJ NA STRONIE 🌿PURE LEAF!</h1>
        <p>Zapamiętaj link tej strony, dzięki temu nigdy nie stracisz z nami kontaktu. Wszystkie potrzebne informacje znajdziesz pod odpowiednimi przyciskami poniżej.</p>
        <p>Aby sprawdzić naszą ofertę, złożyć zamówienie lub przejrzeć opinie klientów – kliknij w odpowiedni przycisk.</p>

        <div class="buttons">
            <button class="button" onclick="addChatMessage('🔶 Pełną ofertę znajdziesz na kanale TeleGuard podanym niżej')">📜Oferta</button>
            <button class="button" onclick="addChatMessage('🔶 TeleGuard: S9MDYLZ2M 🔹 SIGNAL: @purefedor.53')">📞Kontakt</button>
            <button class="button" onclick="addChatMessage('Opinie klientów')">📚Opinie klientów</button>
            <button class="button" onclick="addChatMessage('🔶 Wybierz produkty z naszej oferty a nastepnie napisz do nas wybrany produkt oraz ilość. Podaj kod paczkomatu. Płatność: Blik, Crypto. Paczkę tworzymy na nasze konto InPost, a Ty otrzymujesz tylko kod QR do odbioru paczki.')">📦Jak złożyć zamówienie?</button>
            <button class="button" onclick="addChatMessage('🔶 Płatność: Blik, Crypto.')">💵Metody płatności</button>
            <button class="button" onclick="addChatMessage('🔶 Jeśli zamówisz do godziny 13:00, Twoja paczka na 100% zostanie wysłana tego samego dnia. 🚀')">📲Jaki jest czas dostawy?</button>
        </div>

        <div class="chat-box" id="chatBox">
        </div>

        <p>Dodatkowo zapraszamy do kontaktu w wiadomościach prywatnych na wybranych platformach:</p>
        <p><a href="https://signal.me/#eu/Z4uVY-ZL_QXxDM3ouiYSwBJ3Cubgg8hkXTZlkufDTpSn7wvqYJ5AbZ3fHdU3ChtS" target="_blank">Signal</a></p>
        <p><a href="https://tele.gd/C-OEFITO1VJ" target="_blank">TeleGuard</a></p>

        <p>Dziękujemy za zaufanie i zapraszamy do współpracy! 💝</p>
    </div>

    <script>
        function addChatMessage(message) {
            const chatBox = document.getElementById('chatBox');
            const messageElement = document.createElement('div');
            messageElement.className = 'chat-message';
            messageElement.textContent = message;
            chatBox.appendChild(messageElement);
            chatBox.scrollTop = chatBox.scrollHeight;
        }
    </script>
</body>
</html>
