<!DOCTYPE html>
<html>
<head>
    <title>Found This Strange File...</title>
    <style>
        body {
            background-color: black;
            color: lime;
            font-family: monospace;
            padding: 20px;
        }
        .hidden {
            display: none;
        }
        button {
            background: lime;
            color: black;
            border: none;
            padding: 10px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <h1>You stumbled upon something...</h1>
    <p>Click the button to reveal a hidden message:</p>
    <button onclick="reveal()">Reveal</button>
    <p id="message" class="hidden">The first clue is: Check clue1.txt in this repository!</p>

    <script>
        function reveal() {
            document.getElementById('message').classList.remove('hidden');
        }
    </script>
</body>
</html>