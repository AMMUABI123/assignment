1.<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Change Background Color</title>
    <style>
        body {
            text-align: center;
            padding: 50px;
            font-family: Arial, sans-serif;
        }
        button {
            font-size: 16px;
            padding: 10px 20px;
            cursor: pointer;
        }
    </style>
</head>
<body>

    <button onclick="changeBackgroundColor()">Change Background Color</button>

    <script>
        function changeBackgroundColor() {
            const randomColor = '#' + Math.floor(Math.random() * 16777215).toString(16);
            document.body.style.backgroundColor = randomColor;
        }
    </script>

</body>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript Tasks</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px;
        }
        button {
            font-size: 16px;
            padding: 10px 20px;
            margin: 10px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <!-- Task 1: Change Background Color -->
    <button onclick="changeBackgroundColor()">Change Background Color</button>

    <!-- Task 2: Count Button Clicks -->
    <h2>Button Clicked: <span id="clickCount">0</span> times</h2>
    <button onclick="incrementCounter()">Click Me</button>

    <script>
        // Task 1: Change Background Color
        function changeBackgroundColor() {
            const randomColor = '#' + Math.floor(Math.random() * 16777215).toString(16);
            document.body.style.backgroundColor = randomColor;
        }


2.<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Show/Hide Password</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f4f4f4;
        }
        .container {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        input {
            padding: 8px;
            width: 200px;
            margin-right: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            padding: 8px 12px;
            border: none;
            background-color: #007bff;
            color: white;
            cursor: pointer;
            border-radius: 5px;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>

<div class="container">
    <input type="password" id="password" placeholder="Enter password">
    <button id="toggleBtn">Show</button>
</div>

<script>
    const passwordInput = document.getElementById("password");
    const toggleBtn = document.getElementById("toggleBtn");



3.<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Show/Hide Password</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f4f4f4;
        }
        .container {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        input {
            padding: 8px;
            width: 200px;
            margin-right: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            padding: 8px 12px;
            border: none;
            background-color: #007bff;
            color: white;
            cursor: pointer;
            border-radius: 5px;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>

<div class="container">
    <input type="password" id="password" placeholder="Enter password">
    <button id="toggleBtn">Show</button>
</div>

<script>
    const passwordInput = document.getElementById("password");
    const toggleBtn = document.getElementById("toggleBtn");

    toggleBtn.addEventListener("click", function () {
        if (passwordInput.type === "password") {
            passwordInput.type = "text";
            toggleBtn.textContent = "Hide";
        } else {
            passwordInput.type = "password";
            toggleBtn.textContent = "Show";
        }
    });
</script>

</body>
</html>


4.<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Real-Time Character Counter</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f4f4f4;
            flex-direction: column;
        }
        .container {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            text-align: center;
            width: 300px;
        }
        textarea {
            width: 100%;
            height: 100px;
            padding: 8px;
            border: 1px solid #ccc;
            border-radius: 5px;
            resize: none;
        }
        p {
            margin-top: 10px;
            font-size: 16px;
        }
    </style>
</head>
<body>

<div class="container">
    <textarea id="textArea" placeholder="Type something..."></textarea>
    <p>Characters: <span id="charCount">0</span></p>
</div>

<script>
    const textArea = document.getElementById("textArea");
    const charCount = document.getElementById("charCount");

    textArea.addEventListener("input", function () {
        charCount.textContent = textArea.value.length;
    });
</script>

</body>
</html>
