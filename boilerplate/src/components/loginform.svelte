<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login</title>
    <style>
        .container {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .login-box {
            width: 400px; /* Fixed width for the container */
            background: linear-gradient(to left, #312d2d, #565353);
            padding: 2em;
            border-radius: 1em;
            box-shadow: 0 0 2em rgba(0, 0, 0, 0.2);
            text-align: center; /* Center the content */
            animation: slide-in 0.5s ease-out;
        }

        form {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        form input[type="text"],
        form input[type="password"] {
            background: none;
            border: none;
            border-bottom: 0.1em solid #DDD;
            color: #ffffff;
            padding: 1em;
            margin: 1em;
            width: 80%;
            font-size: 1.6em;
            transition: all 0.3s ease-out;
            animation: fade-in 0.5s ease-out;
        }

        form input[type="text"]:focus,
        form input[type="password"]:focus {
            outline: none;
            border-bottom: 0.1em solid #BBB;
        }

        form button {
            background: linear-gradient(to bottom right, #EC407A, #AB47BC);
            color: #FFF;
            border: none;
            padding: 1em 2em;
            border-radius: 1em;
            font-size: 1.6em;
            margin: 2em auto; /* Center the button */
            cursor: pointer;
            box-shadow: 0 0 2em rgba(0, 0, 0, 0.2);
            transition: all 0.3s ease-out;
            animation: bounce 1.5s infinite;
        }

        form button:hover {
            background: linear-gradient(to bottom right, #FF4081, #BA68C8);
            box-shadow: 0 0 3em rgba(0, 0, 0, 0.4);
        }

        @keyframes slide-in {
            from {
                transform: translateY(5em);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
        }

        @keyframes fade-in {
            from {
                opacity: 0;
                transform: translateY(2em);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% {
                transform: translateY(0);
            }
            40% {
                transform: translateY(-1em);
            }
            60% {
                transform: translateY(-1em);
            }
        }
    </style>
</head>

<body>
<div class="container">
    <div class="login-box">
        <form>
            <h1>Login</h1>
            <input type="text" placeholder="Username" required />
            <input type="password" placeholder="Password" required />
            <button type="submit">Login</button>
        </form>
    </div>
</div>
</body>

</html>
