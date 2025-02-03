<!DOCTYPE html>
<html lang="el">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Θα γίνεις η Βαλεντίνα μου;</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: pink;
        }
        .container {
            margin-top: 100px;
        }
        .button {
            font-size: 20px;
            padding: 10px 20px;
            margin: 10px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
        }
        #yes {
            background-color: red;
            color: white;
        }
        #no {
            background-color: white;
            color: red;
            position: absolute;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Θα γίνεις η Βαλεντίνα μου;</h1>
        <button id="yes" class="button">Ναι</button>
        <button id="no" class="button">Όχι</button>
    </div>

    <script>
        document.getElementById("no").addEventListener("mouseover", function() {
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            this.style.left = x + "px";
            this.style.top = y + "px";
        });
        document.getElementById("yes").addEventListener("click", function() {
            alert("Τέλεια! 💖 Ανυπομονώ για την ημέρα του Αγίου Βαλεντίνου μαζί σου!");
        });
    </script>
</body>
</html>
