# Web-technologies-week-4-assignments-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Web Design</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
        }

        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
            background: #333;
            color: white;
        }

        .nav-menu {
            display: flex;
            list-style: none;
        }

        .nav-menu li {
            margin-left: 20px;
        }

        .nav-menu a {
            color: white;
            text-decoration: none;
        }

        .main-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            padding: 20px;
        }

        .text-column, .image-column {
            padding: 20px;
            background: #f4f4f4;
        }

        .image-column img {
            max-width: 100%;
            height: auto;
            transition: transform 0.3s;
        }

        .image-column img:hover {
            transform: scale(1.05);
        }

        footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
            background: #333;
            color: white;
        }

        .social-links a {
            color: white;
            margin-right: 15px;
            text-decoration: none;
        }

        /* Media Queries */
        @media (max-width: 600px) {
            header, footer {
                flex-direction: column;
                align-items: flex-start;
            }

            .nav-menu {
                flex-direction: column;
                margin-top: 10px;
            }

            .main-content {
                grid-template-columns: 1fr;
            }
        }

        @media (min-width: 601px) and (max-width: 1024px) {
            .main-content {
                grid-template-columns: 1fr;
            }
        }

        @media (min-width: 1025px) {
            header, footer {
                flex-direction: row;
            }

            .main-content {
                grid-template-columns: 1fr 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">MyLogo</div>
        <nav>
            <ul class="nav-menu">
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Services</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>
    
    <main class="main-content">
        <div class="text-column">
            <h1>Welcome to My Website</h1>
            <p>Dream, Achieve,Inspire.</p>
        </div>
        <div class="image-column">
            <img src="https://unsplash.com/photos/a-walkway-with-steps-leading-up-to-the-top-of-it-vpIx1LoVbuk" alt="Sample Image">
        </div>
    </main>

    <footer>
        <div class="social-links">
            <a href="#">Facebook</a>
            <a href="#">Twitter</a>
            <a href="#">Instagram</a>
        </div>
        <p>&copy; 2024 MyWebsite. All rights reserved.</p>
    </footer>
</body>
</html>
