<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Simple Website</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Welcome to My Website</h1>
        <p>Your one-stop for cool content!</p>
    </header>
    <main>
        <section id="about">
            <h2>About Us</h2>
            <p>We provide amazing tutorials, projects, and ideas to enhance your web development skills.</p>
        </section>
        <section id="services">
            <h2>Our Services</h2>
            <ul>
                <li>Web Development</li>
                <li>SEO Optimization</li>
                <li>Content Creation</li>
            </ul>
        </section>
        <button id="actionButton">Click Me!</button>
        <p id="responseMessage" class="hidden">Thank you for clicking!</p>
    </main>
    <footer>
        <p>© 2024 My Simple Website. All rights reserved.</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>
/* General Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    line-height: 1.6;
    background-color: #f4f4f9;
}

/* Header Styles */
header {
    background: #333;
    color: #fff;
    padding: 10px 20px;
    text-align: center;
}

/* Main Content Styles */
main {
    padding: 20px;
}

section {
    margin: 20px 0;
}

h2 {
    color: #333;
}

/* Button Styles */
button {
    display: inline-block;
    background: #007BFF;
    color: #fff;
    padding: 10px 15px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 16px;
}

button:hover {
    background: #0056b3;
}

/* Response Message Styles */
.hidden {
    display: none;
    color: #28a745;
    font-weight: bold;
    margin-top: 10px;
}

/* Footer Styles */
footer {
    text-align: center;
    padding: 10px 0;
    background: #333;
    color: #fff;
    margin-top: 20px;
}
// Add interactivity to the button
document.getElementById("actionButton").addEventListener("click", function() {
    const responseMessage = document.getElementById("responseMessage");
    responseMessage.classList.remove("hidden");
    responseMessage.textContent = "You clicked the button! Have a great day!";
});
