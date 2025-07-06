# Dill
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Birthday Message</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            max-width: 600px;
            margin: 0 auto;
            padding: 20px;
            text-align: center;
        }
        #message {
            display: none;
            margin-top: 20px;
            padding: 20px;
            background-color: #f0f8ff;
            border-radius: 10px;
        }
        input[type="text"] {
            width: 100%;
            padding: 8px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <h1>Welcome to the Birthday Message</h1>
    <p>Answer the following questions to see the message:</p>
    <form id="quiz">
        <!-- Replace [Your question 1] with your first question -->
        <label for="q1">Question 1: [Your question 1]</label>
        <input type="text" id="q1" name="q1" placeholder="Enter answer"><br><br>
        <!-- Replace [Your question 2] with your second question -->
        <label for="q2">Question 2: [Your question 2]</label>
        <input type="text" id="q2" name="q2" placeholder="Enter answer"><br><br>
        <!-- Replace [Your question 3] with your third question -->
        <label for="q3">Question 3: [Your question 3]</label>
        <input type="text" id="q3" name="q3" placeholder="Enter answer"><br><br>
        <button type="button" onclick="checkAnswers()">Submit</button>
    </form>
    <div id="message">
        <!-- Replace [Your personalized message] with your birthday wish -->
        <h2>Happy Birthday!</h2>
        <p>[Your personalized message]</p>
    </div>
    <script>
        function checkAnswers() {
            // Replace [Answer 1], [Answer 2], [Answer 3] with the correct answers
            var correctQ1 = "[Answer 1]";
            var correctQ2 = "[Answer 2]";
            var correctQ3 = "[Answer 3]";
            
            var userQ1 = document.getElementById('q1').value.trim();
            var userQ2 = document.getElementById('q2').value.trim();
            var userQ3 = document.getElementById('q3').value.trim();
            
            if (userQ1 === correctQ1 && userQ2 === correctQ2 && userQ3 === correctQ3) {
                document.getElementById('message').style.display = 'block';
                document.getElementById('quiz').style.display = 'none';
            } else {
                alert("Incorrect answers. Please try again.");
            }
        }
    </script>
</body>
</html>
