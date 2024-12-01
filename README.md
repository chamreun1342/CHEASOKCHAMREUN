<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Matin Topup</title>
    <style>
        /* General Styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #ffeef1;
        }

        .container {
            max-width: 600px;
            margin: 20px auto;
            padding: 20px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        /* Header */
        header {
            text-align: center;
            background-color: #ff66a3;
            padding: 15px;
            border-radius: 10px 10px 0 0;
        }

        header h1 {
            color: white;
            font-size: 24px;
            margin: 0;
        }

        /* Notice Section */
        .notice {
            margin: 10px 0;
            padding: 10px;
            background-color: #ffe4e9;
            border-left: 5px solid #ff66a3;
        }

        .notice p {
            font-size: 14px;
            margin: 0;
            color: #333;
        }

        /* Pricing Section */
        .pricing {
            padding: 15px 0;
        }

        .pricing h2 {
            font-size: 18px;
            margin-bottom: 10px;
        }

        .option {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 10px;
            background-color: #f9f9f9;
            border: 1px solid #ccc;
            border-radius: 5px;
            margin-bottom: 10px;
            cursor: pointer;
            transition: background-color 0.2s;
        }

        .option:hover {
            background-color: #ffe4e9;
        }

        .option p {
            margin: 0;
            font-size: 14px;
        }

        .option span {
            color: #ff66a3;
            font-weight: bold;
        }

        .option img {
            width: 40px;
            height: 40px;
        }

        /* Payment Section */
        .payment-field {
            display: none;
            margin-top: 20px;
            padding: 15px;
            background-color: #f9f9f9;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        .payment-field input {
            width: 100%;
            padding: 10px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 14px;
        }

        .pay-button {
            width: 100%;
            padding: 10px;
            background-color: #ff66a3;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }

        .pay-button:hover {
            background-color: #e05590;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header -->
        <header>
            <h1>Matin Topup</h1>
            <h2>Mobile legends</h2>
        </header>

        <!-- Notice -->
        <div class="notice">
            <p>10 នាទី បន្ទាប់ពីបញ្ចូលមិនបានសូមទំនាក់ទំនងសេវាកម្មដើម្បីជួយផងដែរ។</p>
        </div>
        <!-- Notice -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Game ID and Server ID Check</title>
    <style>
        /* General styles for the page */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        .container {
            width: 90%;
            max-width: 400px;
            margin: 100px auto;
            padding: 20px;
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        /* Title styles */
        h2 {
            text-align: center;
            color: #333;
            font-size: 24px;
        }

        /* Input field and button styles */
        input {
            width: 100%;
            padding: 12px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 16px;
        }

        .submit-btn {
            background-color: #007bff;
            color: white;
            font-size: 16px;
            cursor: pointer;
            border: none;
            padding: 12px;
            width: 100%;
            border-radius: 5px;
        }

        .submit-btn:hover {
            background-color: #0056b3;
        }

        .result {
            margin-top: 20px;
            padding: 10px;
            background-color: #f1f1f1;
            border-radius: 5px;
            display: none;
        }

        .result p {
            margin: 0;
            font-size: 16px;
            color: #333;
        }

        .pink-name {
            color: pink;
            font-weight: bold;
        }
    </style>
</head>
<body>

    <div class="container">
        <h2>បញ្ចូលព័ត៌មាន</h2>

        <!-- Form for Game ID and Server ID -->
        <form id="gameForm">
            <input type="text" id="gameId" placeholder="Enter Game ID" required>
            <input type="text" id="serverId" placeholder="Enter Server ID" required>

            <!-- Button to check the IDs -->
            <button type="button" class="submit-btn" onclick="checkIds()">Check</button>
        </form>

        <!-- Display result after clicking the button -->
        <div class="result" id="result">
            <p><strong>Player Name:</strong> <span id="resultPlayerName" class="pink-name"></span></p>
        </div>
    </div>

    <script>
        // Function to simulate checking the entered Game ID and Server ID
        function checkIds() {
            // Get the values from the input fields
            const gameId = document.getElementById("gameId").value;
            const serverId = document.getElementById("serverId").value;

            // Simulate fetching a player name based on the Game ID and Server ID
            let playerName = "Unknown Player";

            // Simulate different player names based on the Game ID and Server ID
            if (gameId === "12345" && serverId === "1") {
                playerName = "John Doe"; // Example player for Game ID 12345 and Server ID 1
            } else if (gameId === "67890" && serverId === "2") {
                playerName = "Jane Smith"; // Another example for Game ID 67890 and Server ID 2
            } else if (gameId === "11111" && serverId === "3") {
                playerName = "Player One"; // Another example for Game ID 11111 and Server ID 3
            }

            // Display the player name in the result div with pink color
            document.getElementById("resultPlayerName").textContent = playerName;

            // Show the result section
            document.getElementById("result").style.display = "block";
        }
    </script>

</body>
</html>
        <!-- Notice -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Telegram Link</title>
    <style>
        /* Style for the clickable button */
        .telegram-button {
            display: inline-block;
            padding: 10px 20px;
            background-color: #0088cc;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            font-size: 16px;
            text-align: center;
            transition: background-color 0.3s;
        }

        .telegram-button:hover {
            background-color: #0077b5;
        }
    </style>
</head>
<body>
    <a href="https://t.me/MATIN0168" class="telegram-button" target="_blank">Go to Telegram</a>
</body>
</html>

        <!-- Pricing Section -->
        <div class="pricing">
            <h2>សេវាកម្មជ្រើសរើស</h2>
            <!-- Option 1 -->
            <div class="option" onclick="selectService('Weekly Pass', 1.49)">
                <img src="https://via.placeholder.com/40" alt="Weekly Pass">
                <p>Weekly Pass</p>
                <span>$1.49</span>
            </div>
            <!-- Option 2 -->
            <div class="option" onclick="selectService('Weekly Pass x3', 4.77)">
                <img src="https://via.placeholder.com/40" alt="Weekly Pass x3">
                <p>Weekly Pass x3</p>
                <span>$4.77</span>
            </div>
            <!-- Option 3 -->
            <div class="option" onclick="selectService('Weekly Pass x5', 7.45)">
                <img src="https://via.placeholder.com/40" alt="Weekly Pass x5">
                <p>Weekly Pass x5</p>
                <span>$7.45</span>
            </div>
            <!-- Option 4 -->
            <div class="option" onclick="selectService('172 DM + Weekly Pass', 4.29)">
                <img src="https://via.placeholder.com/40" alt="172 DM + Weekly Pass">
                <p>172 DM + Weekly Pass</p>
                <span>$4.29</span>
            </div>
        </div>

        <!-- Payment Section (Initially Hidden) -->
        <div class="payment-field" id="payment-field">
            <h3>សូមបញ្ចូលព័ត៌មានការទូទាត់</h3>
            <input type="text" id="user-id" placeholder="Enter User ID" readonly>
            <input type="text" id="zone-id" placeholder="Enter Zone ID" readonly>
            <button class="pay-button" onclick="goToPayline()">Pay Now</button>
        </div>
    </div>

    <script>
        let selectedService = "";
        let selectedPrice = 0;

        // Handle Service Selection
        function selectService(serviceName, price) {
            selectedService = serviceName;
            selectedPrice = price;

            // Show the payment field with the selected service details
            document.getElementById('payment-field').style.display = 'block';
            document.getElementById('user-id').value = serviceName;  // Set User ID as Service Name (for demo)
            document.getElementById('zone-id').value = `$${price.toFixed(2)}`;  // Set Zone ID as Price
        }

        // Redirect to Payment Gateway (Aba Payline for this example)
        function goToPayline() {
            // In this example, we'll just simulate a redirect
            // For a real implementation, you'd redirect to the payment gateway like Aba Payline

            const paymentUrl = "https://pay.ababank.com/pfSZ5LnXfYBKRFHd8";  // Replace with actual Aba Payline URL
            window.location.href = paymentUrl;
        }
    </script>
</body>
</html>
