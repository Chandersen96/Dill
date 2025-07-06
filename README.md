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
            color: red;
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
        <!-- Replace [what i love to call you?] with your first question -->
        <label for="q1">Question 1: [Your question 1]</label>
        <input type="text" id="q1" name="q1" placeholder="Enter answer"><br><br>
        <!-- Replace [What is my medicine from you?] with your second question -->
        <label for="q2">Question 2: [Your question 2]</label>
        <input type="text" id="q2" name="q2" placeholder="Enter answer"><br><br>
        <!-- Replace [On which date you came into my life?] with your third question -->
        <label for="q3">Question 3: [Your question 3]</label>
        <input type="text" id="q3" name="q3" placeholder="Enter answer"><br><br>
        <button type="button" onclick="checkAnswers()">Submit</button>
    </form>
    <div id="message">
        <!-- Replace [Yoy said i made you addicted to my food but what about you? You made me addicted to your kind heart, your pure soul, your nature, your smile jisko dekhe bina mai adhura sa rehta hun. ab to subah sham rehta hai tumhara hi khyal. sunke naam tera ho jata hun mai laal. Dekh kar mere chare par blush kar dete hai nisha or aman ched ched kar mera bura haal. Tere liye sab kuch karne ka karta hai maan. Dillon dimaag par chai ho tum. tmhari ek hasin k liye kar sakta hun kuch bhi. zamana chae kitni bhi karle koshish tumhe rulane ya satane ki par mai khada hun unke aur tumhare beech. Tere chere par vo shocking khusi or smile ki vehj ban bankar dill ko bahut sukoon mila. Hamesha chata hun tujhe sab dena aur karunga puri koshish ki hamesha kar paaun isse puraa. Kabhi bhi tu hichkichana maat chahe ho milna, ya kuch khana ya kuch bhi ho khul k bol dena kisi bhi time kisi bhi jagh mai puri koshish karunga usee puraa karne ki meri Queeny. ] with your birthday wish -->
        <h2>Happy Birthday MY QUEENY!</h2>
        <p>[Your personalized message]</p>
    </div>
    <script>
        function checkAnswers() {
            // Replace [Answer 1], [Answer 2], [Answer 3] with the correct answers
            var correctQ1 = "[Queeny]";
            var correctQ2 = "[Your Smile]";
            var correctQ3 = "[15/06/2025]";
            
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
