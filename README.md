<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional Home Page</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f8f9fa;
            color: #333;
        }

        header {
            background-color: #007BFF;
            color: #fff;
            padding: 20px;
            text-align: center;
            font-size: 24px;
        }

        nav {
            background-color: #eee;
            padding: 10px 0;
        }

        ul {
            list-style: none;
            margin: 0;
            padding: 0;
            display: flex;
            width:100%;
            justify-content: center;
        }

        li {
            margin: 0 20px;
        }

        a {
            text-decoration: none;
            color: #007BFF;
            font-weight: bold;
            font-size: 18px;
            transition: color 0.3s ease-in-out;
        }

        a:hover {
            color: #0056b3;
        }

        main {
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
            background-color: #fff;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
        }
    </style>
</head>
<body>

    <header>
       Gladiator Tools
    </header>

    <nav>
        <ul>
         <li><a href="file:///C:/Users/i.fekrouni/Desktop/si/main.html" onclick="goToPage('page1.html')">Home </a></li>
         <li><a href="https://gladiatordesign1.github.io/spf-tool-v2.github.io/" onclick="goToPage('page1.html')">Spf Record Maker</a></li>
           <li><a href="file:///C:/Users/i.fekrouni/Desktop/si/matmat.html" onclick="goToPage('page1.html')">spf Collect</a></li>
           <li><a href="file:///C:/Users/i.fekrouni/Desktop/si/matched%202.html" onclick="goToPage('page2.html')">Matching servers</a></li>
         <li><a href="file:///C:/Users/i.fekrouni/Desktop/si/server%20to%20line.html" onclick="goToPage('page2.html')">One line </a></li>
         <li><a href="file:///C:/Users/i.fekrouni/Desktop/si/duplicate%20-%20Copy.html" onclick="goToPage('page2.html')">Duplicate Domain Counter</a></li>
         <li><a href="file:///C:/Users/i.fekrouni/Desktop/si/open%20links3.html" onclick="goToPage('page2.html')">Open links</a></li>
           <!-- Add more pages as needed -->
       </ul>
   </nav>

    <main>
        <!-- Content will be loaded here -->
    </main>

    <script>
        function goToPage(page) {
            // Load content into the main section
            fetch(page)
                .then(response => response.text())
                .then(data => document.querySelector('main').innerHTML = data)
                .catch(error => console.error('Error loading page:', error));
        }
    </script>

</body>
</html>
