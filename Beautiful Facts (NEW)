<!DOCTYPE html>
<html>
<head>
<title>Beautiful Life Facts</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

<style>
body {
    font-family: 'Poppins', sans-serif;
    text-align: center;
    background: linear-gradient(-45deg, #ff9a9e, #fad0c4, #fbc2eb, #a6c1ee);
    background-size: 400% 400%;
    animation: gradientBG 10s ease infinite;
    color: #333;
    padding: 40px;
}

.container {
    background: white;
    padding: 30px;
    border-radius: 20px;
    max-width: 400px;
    margin: auto;
    box-shadow: 0 15px 30px rgba(0,0,0,0.15);
    animation: fadeIn 1s ease;
}

h1 {
    color: #ff4b5c;
    margin-bottom: 5px;
}

#fact {
    font-size: 18px;
    margin: 20px 0;
    transition: 0.3s ease;
}

button {
    padding: 12px 22px;
    border: none;
    background: #ff4b5c;
    color: white;
    border-radius: 12px;
    cursor: pointer;
    font-size: 15px;
    transition: 0.3s ease;
    margin: 5px;
}

button:hover {
    background: #ff6f61;
    transform: scale(1.05);
}

button:active {
    transform: scale(0.95);
}

@keyframes fadeIn {
    from {opacity: 0; transform: translateY(20px);}
    to {opacity: 1; transform: translateY(0);}
}

@keyframes gradientBG {
    0% {background-position: 0% 50%;}
    50% {background-position: 100% 50%;}
    100% {background-position: 0% 50%;}
}
</style>

</head>

<body>

<h1>🌸 Beautiful Facts About Life</h1>
<p>By Oyin 💻✨</p>

<div class="container">
    <p id="fact">Click the button to discover something beautiful about life 💫</p>

    <button onclick="showFact()">✨ Show Fact</button>
    <button onclick="shareFact()">📤 Share</button>
</div>

<script>
const facts = [
    "You are unique—there’s no one else exactly like you 🌟",
    "Small progress every day leads to big results 💪",
    "Kindness always comes back in unexpected ways ❤️",
    "Your thoughts shape your reality 🧠",
    "Every day is a fresh start 🌅",
    "You are stronger than you think 💥",
    "Happiness can be found in simple things 😊",
    "Growth takes time—be patient with yourself 🌱"
];

let lastIndex = -1;

function showFact() {
    let random;

    do {
        random = Math.floor(Math.random() * facts.length);
    } while (random === lastIndex);

    lastIndex = random;

    const factText = document.getElementById("fact");
    factText.style.opacity = 0;

    setTimeout(() => {
        factText.innerText = facts[random];
        factText.style.opacity = 1;
    }, 200);
}

function shareFact() {
    const text = document.getElementById("fact").innerText;

    if (navigator.share) {
        navigator.share({
            title: "Beautiful Life Fact",
            text: text
        });
    } else {
        alert("Sharing not supported on this device.");
    }
}
</script>

</body>
</html>
