# coursera-test
 coursera-test repository
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Father's Day!</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: #000;
            color: #fff;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }

        header {
            background-color: #4CAF50;
            color: white;
            text-align: center;
            padding: 2em 0;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        header h1 {
            margin: 0;
            font-size: 2.5em;
        }

        main {
            flex: 1;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .hero {
            text-align: center;
            margin-bottom: 40px;
        }

        .hero img {
            max-width: 50%;
            height: 50%;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .hero p {
            font-size: 1.2em;
            margin-top: 20px;
        }

        .memories {
            margin-bottom: 40px;
            width: 100%;
            max-width: 800px;
        }

        .memories h2 {
            text-align: center;
            margin-bottom: 20px;
            font-size: 2em;
        }

        .memory {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
            background-color: #333;
            border-radius: 10px;
            padding: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .memory img {
            width: 100px;
            height: 100px;
            border-radius: 10px;
            margin-right: 20px;
            object-fit: cover;
        }

        .memory p {
            margin: 0;
            font-size: 1em;
        }

        .message-form {
            text-align: center;
            width: 100%;
            max-width: 600px;
        }

        .message-form h2 {
            margin-bottom: 20px;
            font-size: 2em;
        }

        .message-form form {
            display: flex;
            flex-direction: column;
        }

        .message-form label {
            margin-bottom: 5px;
            font-weight: 600;
        }

        .message-form input, .message-form textarea {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 2px solid #ccc;
            border-radius: 5px;
            font-size: 1em;
            background-color: #444;
            color: #fff;
        }

        .message-form button {
            background-color: #4CAF50;
            color: white;
            padding: 10px;
            border: none;
            border-radius: 5px;
            font-size: 1em;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .message-form button:hover {
            background-color: #45a049;
        }

        footer {
            background-color: #4CAF50;
            color: white;
            text-align: center;
            padding: 10px 0;
            box-shadow: 0 -4px 8px rgba(0, 0, 0, 0.2);
        }
    </style>
</head>
<body>
    <header>
        <h1>Happy Father's Day!</h1>
    </header>
    <main>
        <section class="hero">
            <img src="Photo0157.jpg" alt="Father and Child">
            <p>Dear Dad, thank you for everything you do. You are the best!</p>
        </section>
        <section class="memories">
            <h2>Memories</h2>
            <div class="memory">
                <img src="Photo0157.jpg" alt="Memory 1">
                <p>A great day we spent together.</p>
            </div>
            <div class="memory">
                <img src="Photo0157.jpg" alt="Memory 2">
                <p>Our favorite vacation spot.</p>
            </div>
        </section>
        <section class="message-form">
            <h2>Send a Message</h2>
            <form id="messageForm">
                <label for="name">Your Name:</label>
                <input type="text" id="name" name="name" required>
                <label for="message">Your Message:</label>
                <textarea id="message" name="message" required></textarea>
                <button type="submit">Send</button>
            </form>
            <p id="formMessage"></p>
        </section>
    </main>
    <footer>
        <p>Contact me at: <a href="mailto:example@example.com">example@example.com</a></p>
        <p>Follow me on <a href="#">Social Media</a></p>
    </footer>
    <script>
        document.getElementById('messageForm').addEventListener('submit', function(event) {
            event.preventDefault();
            const name = document.getElementById('name').value;
            const message = document.getElementById('message').value;
            document.getElementById('formMessage').textContent = `Thank you, ${name}! Your message: "${message}" has been sent.`;
            this.reset();
        });
    </script>
</body>
</html>
