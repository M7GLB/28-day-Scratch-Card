<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>28 Day Sctratch card</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f4f4f4;
      margin: 0;
      padding: 0;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }

    .container {
      background-color: #fff;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      padding: 20px;
      text-align: center;
    }

    h1 {
      color: #333;
      font-size: 28px;
      margin-bottom: 10px;
    }

    p {
      color: #666;
      font-size: 24px;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>28 Day Sctratch card</h1>
    </p>Cards scratched on or before :</p>
    <p id="displayDate"></p>
    </p>are expired</p>
  </div>

  <script>
    // Get the current date
    var currentDate = new Date();

    // Calculate the date 29 days ago
    var pastDate = new Date(currentDate);
    pastDate.setDate(currentDate.getDate() - 29);

    // Format the date as dd/mm/yy
    var formattedDate = pastDate.toLocaleDateString('en-GB');

    // Display the formatted date
    document.getElementById('displayDate').innerText = formattedDate;
  </script>
</body>
</html>
