<?php
$welcome_message = "You are welcome to Danny S Clement coding class. You can learn to become an expert and get a job from us or connect you abroad.";

$messages = [
    "Before you can access this website, you need to make a little payment. Thank you!",
    "To proceed, kindly make your payment. Your access will be granted afterward.",
    "Ensure you make payment to avoid restrictions. Thank you!",
    "Your payment unlocks access to all features. Proceed now!",
    "Complete your payment and send the receipt via WhatsApp to verify access."
];

$payment_not_received = "Daniel Clement hasn’t received your payment. Kindly send your payment receipt to us on WhatsApp for verification. Thank you!";
?>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Payment Board</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f4f4f4;
            padding: 20px;
        }
        .board {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
            max-width: 400px;
            margin: auto;
        }
        .moving-message {
            background: #ffcc00;
            padding: 10px;
            font-size: 16px;
            font-weight: bold;
            white-space: nowrap;
            overflow: hidden;
            width: 100%;
            box-sizing: border-box;
        }
        .moving-message span {
            display: inline-block;
            padding-left: 100%;
            animation: moveText 10s linear infinite;
        }
        @keyframes moveText {
            from { transform: translateX(100%); }
            to { transform: translateX(-100%); }
        }
        .prices {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }
        .price {
            background: #007bff;
            color: white;
            padding: 10px;
            margin: 5px;
            border-radius: 5px;
            cursor: pointer;
        }
        .payment-info {
            text-align: left;
            margin-top: 20px;
        }
        .rules {
            margin-top: 10px;
        }
        #confirm-btn {
            background: green;
            color: white;
            padding: 10px;
            border: none;
            cursor: pointer;
            margin-top: 10px;
            width: 100%;
            border-radius: 5px;
            display: none;
        }
        .hidden {
            display: none;
        }
        .waiting {
            font-weight: bold;
            color: red;
        }
    </style>
</head>
<body>

    <!-- Moving Message -->
    <div class="moving-message">
        <span id="message-text"><?php echo $messages[0]; ?></span>
    </div>

    <div class="board">
        <h2>Payment Board</h2>

        <!-- Price Selection -->
        <h3>Select a Payment Amount</h3>
        <div class="prices" id="price-options">
            <?php
            $amounts = ["₦3,000", "₦6,000", "₦10,000", "₦16,000", "₦25,000", "₦35,000", "₦50,000", "₦100,000", "₦500,000", "₦1,000,000"];
            foreach ($amounts as $amount) {
                echo "<div class='price' data-amount='$amount'>$amount</div>";
            }
            ?>
        </div>

        <!-- Bank Details -->
        <div class="payment-info">
            <h3>Bank Payment Details</h3>
            <p><strong>Bank Name:</strong> First Bank of Nigeria</p>
            <p><strong>Account Name:</strong> Daniel Clement</p>
            <p><strong>Account Number:</strong> 3216009085</p>
        </div>

        <!-- Accept Rules -->
        <div class="rules">
            <input type="checkbox" id="accept-rules"> I accept all rules
        </div>

        <!-- Confirmation Button -->
        <button id="confirm-btn">I've Made Payment</button>

        <!-- Waiting Message -->
        <p id="waiting-message" class="hidden waiting">Please wait, confirming your transaction...</p>

        <!-- WhatsApp Message -->
        <p id="success-message" class="hidden">
            We can't see your payment. Kindly 
            <a id="whatsapp-link" href="#" target="_blank">Click here to upload your payment receipt to us on WhatsApp</a> to verify. Thank you!
        </p>
    </div>

    <script>
        let welcomeMessage = "<?php echo $welcome_message; ?>";
        let messages = <?php echo json_encode($messages); ?>;
        let paymentNotReceived = "<?php echo $payment_not_received; ?>";
        let messageIndex = 0;
        let selectedAmount = "";

        function speakMessage(message) {
            let speech = new SpeechSynthesisUtterance(message);
            speech.rate = 1;
            speech.pitch = 1;
            speech.volume = 1;
            speech.lang = "en-US";
            window.speechSynthesis.speak(speech);
        }

        function updateMessage() {
            let messageText = document.getElementById("message-text");
            messageText.textContent = messages[messageIndex];

            speakMessage(messages[messageIndex]);

            messageIndex = (messageIndex + 1) % messages.length;
        }

        // Auto-Play Welcome Message on Page Load
        document.addEventListener("DOMContentLoaded", function() {
            speakMessage(welcomeMessage);
            setTimeout(() => {
                updateMessage();
            }, 5000);
        });

        setInterval(updateMessage, 10000);

        // Prevent AI voice from stopping
        setInterval(() => {
            if (!window.speechSynthesis.speaking) {
                speakMessage(messages[messageIndex]);
            }
        }, 3000);

        document.querySelectorAll(".price").forEach(price => {
            price.addEventListener("click", function () {
                selectedAmount = this.getAttribute("data-amount");
                speakMessage(`You have selected to make a payment of ${selectedAmount}`);
                document.getElementById("confirm-btn").style.display = "block";
            });
        });

        document.getElementById("confirm-btn").addEventListener("click", function() {
            let waitingMessage = document.getElementById("waiting-message");
            let successMessage = document.getElementById("success-message");
            let whatsappLink = document.getElementById("whatsapp-link");
            let acceptRules = document.getElementById("accept-rules");

            if (!selectedAmount || !acceptRules.checked) {
                speakMessage("Kindly click to complete your payment and get verified. Thank you!");
                return;
            }

            waitingMessage.classList.remove("hidden");
            successMessage.classList.add("hidden");

            setTimeout(() => {
                waitingMessage.classList.add("hidden");
                successMessage.classList.remove("hidden");

                speakMessage(paymentNotReceived);

                whatsappLink.href = `https://wa.me/2348139926868?text=Sir%2C%20I%20have%20already%20made%20the%20payment%20of%20${encodeURIComponent(selectedAmount)}.%20Kindly%20verify%20my%20transaction.%20Thank%20you%20sir.`;
            }, 5000);
        });
    </script>

</body>
</html>
