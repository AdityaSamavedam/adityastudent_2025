<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aditya Samavedam's Blog</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            color: #333;
            margin: 0;
            padding: 0;
            transition: background-color 0.5s, color 0.5s;
        }

        header {
            background-color: #333;
            color: white;
            padding: 10px 20px;
            text-align: center;
            transition: background-color 0.5s;
        }

        h1 {
            margin: 0;
            font-size: 2.5em;
        }

        .content {
            padding: 20px;
        }

        a {
            color: limegreen;
            text-decoration: none;
        }

        a:hover {
            text-decoration: underline;
        }

        img {
            max-width: 100%;
            height: auto;
            display: block;
            margin: 20px 0;
            transition: transform 0.3s;
        }

        img:hover {
            transform: scale(1.1);
        }

        .about-me ul {
            list-style-type: none;
            padding: 0;
        }

        .about-me li {
            padding: 5px 0;
        }

        .highlight {
            color: fuchsia;
        }

        .dark-mode {
            background-color: #1a1a1a;
            color: #f0f0f0;
        }

        .dark-mode header {
            background-color: #000;
        }

        .dark-mode a {
            color: lightgreen;
        }

        .dark-mode button {
            background-color: #444;
            color: #f0f0f0;
        }

        .quote {
            font-style: italic;
            color: lime;
            margin-top: 20px;
        }

        button {
            padding: 10px 20px;
            margin: 20px 0;
            cursor: pointer;
            background-color: #333;
            color: white;
            border: none;
            transition: background-color 0.3s, transform 0.3s;
        }

        button:hover {
            background-color: limegreen;
            transform: scale(1.05);
        }
    </style>
</head>
<body>
    <header>
        <h1>🌟 Aditya Samavedam's Blog 🌟</h1>
        <button id="toggleDarkMode">Toggle Dark Mode</button>
    </header>
    <div class="content">
        <h2>Check out my <a href="https://github.com/AdityaSamavedam" target="_blank">Github page</a>!</h2>

        <h3>🌌 The Reykjavik Northern Lights are Beautiful 🌌</h3>
        <img src="./images/NorthernLights.jpg" alt="Northern Lights">

        <h3>🎨 My Freeform Picture 🎨</h3>
        <img src="./images/FreeformPicture.png" alt="Freeform Picture">

        <h3>🎓 About Me 🎓</h3>
        <div class="about-me">
            <ul>
                <li>Junior at <a href="https://en.wikipedia.org/wiki/Del_Norte_High_School_(San_Diego)" target="_blank" style="color:deepskyblue">Del Norte High School</a>.</li>
                <li><span class="highlight">Second Degree Black Belt in Taekwondo</span></li>
                <li>Codes mostly in <span style="color:gold">Python</span>, has worked with AI/ML.</li>
                <li>Has lived in <a href="https://www.youtube.com/watch?v=CNDI4WlJ8eo" target="_blank" style="color:darkorange">India</a> for 8 years.</li>
                <li>Aspires to major in <span style="color:mediumpurple">Computer Science</span>.</li>
                <li>Loves to <a href="https://www.youtube.com/@Pongfinity" target="_blank" style="color:red">watch Table Tennis</a>, and also plays it.</li>
                <li><span style="color:coral">Destroys</span> people at badminton.</li>
                <li>Loves to play <span style="color:tomato">Mario Kart Wii</span> and <span style="color:orangered">Brawl Stars</span>.</li>
            </ul>
        </div>
        <img src="./images/mario-kart.gif" alt="Mario Kart Wii GIF">
        <h3>Best song in the world: <a href="https://www.youtube.com/watch?v=xvFZjo5PgG0" target="_blank" style="color:turquoise">Click this link !!!</a></h3>
        <button id="quoteButton">Show Me a Motivational Quote</button>
        <div class="quote" id="quote"></div>
    </div>

    <script>
        // Dark Mode Toggle
        document.getElementById('toggleDarkMode').addEventListener('click', function() {
            document.body.classList.toggle('dark-mode');
        });

        // Motivational Quote Generator
        const quotes = [
            "Believe you can and you're halfway there.",
            "The only way to do great work is to love what you do.",
            "Success is not final, failure is not fatal: It is the courage to continue that counts.",
            "Don't watch the clock; do what it does. Keep going.",
            "The future belongs to those who believe in the beauty of their dreams."
        ];

        document.getElementById('quoteButton').addEventListener('click', function() {
            const randomQuote = quotes[Math.floor(Math.random() * quotes.length)];
            document.getElementById('quote').textContent = randomQuote;
        });

        // Alert for Best Song Link
        document.querySelector('a[href="https://www.youtube.com/watch?v=xvFZjo5PgG0"]').addEventListener('click', function(event) {
            alert("Get ready for the best song ever!");
        });
    </script>
</body>
</html>
