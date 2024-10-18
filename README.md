# Data-Structure-Temporary

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Live Date and Time</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #333;
            color: white;
        }
        .time {
            font-size: 24px;
            padding: 10px;
            background-color: #222;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <div class="time">
        <p id="datetime"></p>
    </div>
    <script>
        function updateTime() {
            const now = new Date();
            const dateTimeStr = now.toLocaleString();
            document.getElementById("datetime").textContent = dateTimeStr;
        }
        setInterval(updateTime, 1000);
        updateTime();
    </script>
</body>
</html>
