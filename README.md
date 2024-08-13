<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f4f4f4;
            margin: 0;
        }
        .container {
            width: 50%;
            background-color: white;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .container div {
            margin-bottom: 10px;
        }
        .container label {
            font-size: 12px;
        }
        .container input,
        .container textarea {
            width: 100%;
            padding: 8px;
            margin-top: 5px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        .container button {
            background-color: #800080;
            color: white;
            font-size: 12px;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        .container button:hover {
            background-color: #4B0082;
        }
    </style>
</head>
<body>
    <div class="container">
        <section>
            <div style="display: flex; flex-direction: column; align-items: center;">
                <div style="margin-bottom: 20px; text-align: center;">
                    <p style="font-size: 12px; margin: 5px;">Contact us</p>
                    <p style="font-size: 18px; margin: 5px;">Get in touch</p>
                    <p style="font-size: 12px; margin: 5px;">We love to hear from you. Please fill out this form</p>
                </div>
                <div style="width: 100%;">
                    <div style="display: flex; justify-content: space-between; margin-bottom: 10px;">
                        <div style="width: 48%;">
                            <label for="first-name" style="font-size: 12px;">First Name</label><br>
                            <input type="text" id="first-name" name="first-name"><br>
                        </div>
                        <div style="width: 48%;">
                            <label for="last-name" style="font-size: 12px;">Last Name</label><br>
                            <input type="text" id="last-name" name="last-name"><br>
                        </div>
                    </div>
                    <div>
                        <label for="email" style="font-size: 12px;">Email</label><br>
                        <input type="email" id="email" name="email"><br>
                    </div>
                    <div>
                        <label for="phone" style="font-size: 12px;">Phone Number</label><br>
                        <input type="tel" id="phone" name="phone"><br>
                    </div>
                    <div>
                        <label for="message" style="font-size: 12px;">Message</label><br>
                        <textarea id="message" name="message" rows="4"></textarea><br>
                    </div>
                    <div>
                        <label style="font-size: 12px;">
                            <input type="checkbox" name="privacy-policy" style="margin-right: 10px;"> You agree to our privacy policy
                        </label><br>
                    </div>
                    <div style="text-align: center;">
                        <button type="submit">Send Message</button>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <script>
        const container = {
            hidden: { opacity: 1, scale: 0 },
            visible: {
                opacity: 1,
                scale: 1,
                transition: {
                    delayChildren: 0.3,
                    staggerChildren: 0.2
                }
            }
        };

        const item = {
            hidden: { y: 20, opacity: 0 },
            visible: {
                y: 0,
                opacity: 1
            }
        };
    </script>
</body>
</html>
