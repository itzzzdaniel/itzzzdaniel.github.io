```html
<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Dla Julki ❤️</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #12000a, #350018, #16000d);
            color: white;
            overflow-x: hidden;
        }

        .heart {
            position: fixed;
            bottom: -50px;
            color: #ff4f81;
            font-size: 25px;
            animation: fly 8s linear infinite;
            opacity: 0.7;
            z-index: 0;
        }

        @keyframes fly {
            0% {
                transform: translateY(0) rotate(0deg);
                opacity: 0;
            }

            20% {
                opacity: 0.8;
            }

            100% {
                transform: translateY(-110vh) rotate(360deg);
                opacity: 0;
            }
        }

        .hero {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 30px;
            position: relative;
            z-index: 1;
        }

        .hero h1 {
            font-size: clamp(50px, 10vw, 100px);
            color: #ff5c8a;
            text-shadow: 0 0 30px rgba(255, 92, 138, 0.7);
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0%, 100% {
                transform: scale(1);
            }

            50% {
                transform: scale(1.05);
            }
        }

        .hero h2 {
            font-size: clamp(25px, 5vw, 45px);
            margin-top: 15px;
        }

        .hero p {
            margin-top: 20px;
            font-size: 20px;
            color: #ffc2d1;
        }

        .scroll {
            margin-top: 60px;
            color: #ff8cab;
            animation: bounce 2s infinite;
        }

        @keyframes bounce {
            0%, 100% {
                transform: translateY(0);
            }

            50% {
                transform: translateY(10px);
            }
        }

        section {
            padding: 100px 20px;
            max-width: 1000px;
            margin: auto;
            position: relative;
            z-index: 1;
        }

        .title {
            text-align: center;
            font-size: 40px;
            margin-bottom: 50px;
            color: #ff7097;
        }

        .counter {
            text-align: center;
            background: rgba(255, 255, 255, 0.07);
            border: 1px solid rgba(255, 100, 150, 0.3);
            border-radius: 25px;
            padding: 40px;
            backdrop-filter: blur(10px);
            box-shadow: 0 0 30px rgba(255, 50, 100, 0.15);
        }

        .counter h3 {
            font-size: 25px;
            margin-bottom: 20px;
        }

        #timer {
            font-size: clamp(25px, 5vw, 45px);
            font-weight: bold;
            color: #ff7097;
        }

        .reasons {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 20px;
        }

        .reason {
            background: rgba(255,255,255,0.07);
            padding: 30px;
            border-radius: 20px;
            text-align: center;
            transition: 0.3s;
            border: 1px solid rgba(255, 100, 150, 0.2);
        }

        .reason:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 30px rgba(255, 50, 100, 0.25);
        }

        .reason span {
            font-size: 45px;
        }

        .reason h3 {
            margin: 15px 0;
            color: #ff7097;
        }

        .letter {
            background: rgba(255,255,255,0.08);
            padding: 40px;
            border-radius: 25px;
            line-height: 1.8;
            font-size: 18px;
            border: 1px solid rgba(255, 100, 150, 0.3);
        }

        .letter strong {
            color: #ff7097;
        }

        .surprise {
            text-align: center;
        }

        button {
            background: linear-gradient(135deg, #ff477e, #ff1654);
            color: white;
            border: none;
            padding: 18px 35px;
            border-radius: 50px;
            font-size: 18px;
            cursor: pointer;
            box-shadow: 0 0 25px rgba(255, 40, 100, 0.4);
            transition: 0.3s;
        }

        button:hover {
            transform: scale(1.08);
        }

        #message {
            margin-top: 30px;
            font-size: 25px;
            color: #ffb6c9;
            display: none;
        }

        footer {
            text-align: center;
            padding: 50px 20px;
            color: #ff9db5;
        }
    </style>
</head>

<body>

    <div class="heart" style="left:5%; animation-delay:0s;">❤️</div>
    <div class="heart" style="left:15%; animation-delay:2s;">💗</div>
    <div class="heart" style="left:30%; animation-delay:4s;">💕</div>
    <div class="heart" style="left:50%; animation-delay:1s;">❤️</div>
    <div class="heart" style="left:70%; animation-delay:3s;">💖</div>
    <div class="heart" style="left:85%; animation-delay:5s;">💗</div>
    <div class="heart" style="left:95%; animation-delay:2s;">❤️</div>


    <div class="hero">

        <h1>❤️</h1>

        <h2>Dla mojej Julki</h2>

        <p>
            Najpiękniejszej dziewczyny, jaką mogłem spotkać.
        </p>

        <div class="scroll">
            ↓ przewiń ↓
        </div>

    </div>


    <section>

        <h2 class="title">❤️ Razem ❤️</h2>

        <div class="counter">

            <h3>Jesteśmy razem już:</h3>

            <div id="timer">
                Ładowanie...
            </div>

        </div>

    </section>


    <section>

        <h2 class="title">Dlaczego Cię kocham?</h2>

        <div class="reasons">

            <div class="reason">
                <span>🥰</span>
                <h3>Twój uśmiech</h3>
                <p>
                    Potrafi poprawić mi humor nawet wtedy,
                    kiedy mam najgorszy dzień.
                </p>
            </div>

            <div class="reason">
                <span>❤️</span>
                <h3>Twoje serce</h3>
                <p>
                    Jesteś osobą, przy której mogę być
                    naprawdę sobą.
                </p>
            </div>

            <div class="reason">
                <span>🫶</span>
                <h3>Ty</h3>
                <p>
                    Po prostu Ty. I chyba właśnie tego
                    najbardziej nie da się opisać słowami.
                </p>
            </div>

            <div class="reason">
                <span>💞</span>
                <h3>Nas</h3>
                <p>
                    Kocham wszystkie nasze wspólne chwile
                    i chcę ich mieć jeszcze milion.
                </p>
            </div>

        </div>

    </section>


    <section>

        <h2 class="title">💌 Dla Ciebie</h2>

        <div class="letter">

            <p>
                Julka,
            </p>

            <br>

            <p>
                Chciałem zrobić Ci coś trochę innego niż zwykła
                wiadomość na telefonie.
            </p>

            <br>

            <p>
                Chcę żebyś wiedziała, że <strong>jesteś dla mnie naprawdę ważna</strong>.
                Uwielbiam nasze rozmowy, nasze wygłupy, wspólne chwile
                i nawet te momenty, kiedy się ze sobą droczymy.
            </p>

            <br>

            <p>
                Nie wiem, co przyniesie przyszłość, ale wiem jedno:
                <strong>chcę ją przeżywać razem z Tobą.</strong>
            </p>

            <br>

            <p>
                Kocham Cię ❤️
            </p>

            <br>

            <p>
                Twój ❤️
            </p>

        </div>

    </section>


    <section class="surprise">

        <h2 class="title">Mam coś dla Ciebie...</h2>

        <button onclick="showMessage()">
            Kliknij ❤️
        </button>

        <div id="message">
            Jesteś moją ulubioną osobą na całym świecie. ❤️
            <br><br>
            Kocham Cię Julka! 💕
        </div>

    </section>


    <footer>
        Zrobione specjalnie dla Julki ❤️
        <br>
        © 2026
    </footer>


    <script>

        // DATA ROZPOCZĘCIA ZWIĄZKU:
        // 15 LIPCA 2026

        const startDate = new Date("2026-07-15T00:00:00");


        function updateTimer() {

            const now = new Date();

            let difference = now - startDate;

            const days = Math.floor(
                difference / (1000 * 60 * 60 * 24)
            );

            difference %= (1000 * 60 * 60 * 24);

            const hours = Math.floor(
                difference / (1000 * 60 * 60)
            );

            difference %= (1000 * 60 * 60);

            const minutes = Math.floor(
                difference / (1000 * 60)
            );

            difference %= (1000 * 60);

            const seconds = Math.floor(
                difference / 1000
            );

            document.getElementById("timer").innerHTML =
                `${days} dni, ${hours} godzin, ${minutes} minut, ${seconds} sekund ❤️`;
        }


        setInterval(updateTimer, 1000);

        updateTimer();


        function showMessage() {

            document.getElementById("message").style.display = "block";

        }

    </script>

</body>
</html>
```