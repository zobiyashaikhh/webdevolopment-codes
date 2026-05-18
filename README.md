1.	<!DOCTYPE html>
<html>
<head>
    <title>Student Bio Data</title>
</head>
<body>

    <h1 align="center">Student Bio Data</h1>
    <hr>

    <h2>Personal Information</h2>

    <p><b>Name:</b> Zobiya Shaikh</p>
    <p><b>Address:</b> Pune, Maharashtra</p>
    <p><b>Hobbies:</b> <i>Reading, Coding, Writing</i></p>

    <hr>

    <h2>Educational Background</h2>

    <p><u>College:</u> Sinhgad Academy of Engineering</p>
    <p><strong>Course:</strong> Computer Engineering</p>
    <p><em>Year:</em> Second Year (SE)</p>

</body>
</html>
Assignment 2 

<!DOCTYPE html>
<html>
<head>
    <title>Student Profile</title>
</head>
<body>

    <h1 align="center">Student Profile</h1>

    <table border="1" cellpadding="10">
        <tr>

            <!-- Left side -->
            <td align="center">
                <img src="student.jpg" alt="Student Photo"
                width="150" height="150"><br><br>

                <a href="https://www.unipune.ac.in" target="_blank">
                    Visit SPPU Website
                </a>
            </td>

            <!-- Right side (Nested Table) -->
            <td>
                <h3>Weekly Timetable</h3>

                <table border="1" cellpadding="5">
                    <tr>
                        <th>Day</th>
                        <th>Subject</th>
                    </tr>

                    <tr>
                        <td>Monday</td>
                        <td>Web Development</td>
                    </tr>

                    <tr>
                        <td>Tuesday</td>
                        <td>Python</td>
                    </tr>

                    <tr>
                        <td>Wednesday</td>
                        <td>Java</td>
                    </tr>

                </table>
            </td>

        </tr>
    </table>

</body>
</html>
Assignment 3 

<!DOCTYPE html>
<html>
<head>
    <title>Student Registration Form</title>
</head>
<body>

    <h2 align="center">Student Registration Form</h2>

    <form method="POST">

        <table border="1" cellpadding="10" align="center">

            <tr>
                <td>Name:</td>
                <td>
                    <input type="text" name="name">
                </td>
            </tr>

            <tr>
                <td>Email:</td>
                <td>
                    <input type="email" name="email">
                </td>
            </tr>

            <tr>
                <td>Gender:</td>
                <td>
                    <input type="radio" name="gender"> Male
                    <input type="radio" name="gender"> Female
                </td>
            </tr>

            <tr>
                <td>Date of Birth:</td>
                <td>
                    <input type="date" name="dob">
                </td>
            </tr>

            <tr>
                <td colspan="2" align="center">
                    <input type="submit" value="Submit">
                    <input type="reset" value="Reset">
                </td>
            </tr>

        </table>

    </form>

</body>
</html>
Assignment 4 :

Html : 


<!DOCTYPE html>
<html>
<head>
    <title>CSS Example</title>

    <!-- External CSS Link -->
    <link rel="stylesheet" href="style.css">

    <!-- Internal CSS -->
    <style>
        body {
            background-color: lightyellow;
        }

        table {
            font-family: Arial;
            border-collapse: collapse;
        }

        th, td {
            border: 1px solid black;
            padding: 10px;
        }
    </style>
</head>
<body>

    <!-- Inline CSS -->
    <h1 style="color: blue;" align="center">
        Student Information
    </h1>

    <table align="center">
        <tr>
            <th>Name</th>
            <th>Course</th>
        </tr>

        <tr>
            <td>Zobiya</td>
            <td>Computer Engineering</td>
        </tr>

        <tr>
            <td>Ali</td>
            <td>IT Engineering</td>
        </tr>
    </table>

</body>
</html>


Css :

h1 {
    text-decoration: underline;
}
Assignment 5

<!DOCTYPE html>
<html>
<head>
    <title>Bootstrap Example</title>

    <!-- Bootstrap CSS Link -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css"
    rel="stylesheet">
</head>
<body>

    <!-- Navbar -->
    <nav class="navbar navbar-dark bg-dark">
        <div class="container-fluid">
            <a class="navbar-brand" href="#">
                My Website
            </a>
        </div>
    </nav>

    <!-- Container -->
    <div class="container mt-4">

        <div class="row">

            <!-- Card 1 -->
            <div class="col-md-4">
                <div class="card p-3">
                    <h3>HTML</h3>
                    <p>Learn HTML basics.</p>
                </div>
            </div>

            <!-- Card 2 -->
            <div class="col-md-4">
                <div class="card p-3">
                    <h3>CSS</h3>
                    <p>Learn CSS styling.</p>
                </div>
            </div>

            <!-- Card 3 -->
            <div class="col-md-4">
                <div class="card p-3">
                    <h3>JavaScript</h3>
                    <p>Learn JavaScript basics.</p>
                </div>
            </div>

        </div>
    </div>

</body>
</html>
Assignment 6


<!DOCTYPE html>
<html>
<head>
    <title>Form Validation</title>

    <script>
        function validateForm() {

            var email = document.getElementById("email").value;
            var password = document.getElementById("password").value;

            // Check empty fields
            if (email == "" || password == "") {
                alert("Fields cannot be empty");
                return false;
            }

            // Check email format
            if (email.indexOf("@") == -1 || email.indexOf(".") == -1) {
                alert("Enter valid email");
                return false;
            }

            // Check password length
            if (password.length < 6) {
                alert("Password must be 6 characters");
                return false;
            }

            alert("Login Successful");
            return true;
        }
    </script>
</head>
<body>

    <h2 align="center">Login Form</h2>

    <form onsubmit="return validateForm()">

        <table align="center" border="1" cellpadding="10">

            <tr>
                <td>Email:</td>
                <td>
                    <input type="text" id="email">
                </td>
            </tr>

            <tr>
                <td>Password:</td>
                <td>
                    <input type="password" id="password">
                </td>
            </tr>

            <tr>
                <td colspan="2" align="center">
                    <input type="submit" value="Login">
                </td>
            </tr>

        </table>

    </form>

</body>
</html>
Assignment 7


<!DOCTYPE html>
<html>
<head>
    <title>DOM Example</title>

    <script>
        function changeText() {
            document.getElementById("box").innerHTML = "Hello Student";
        }

        function changeColor() {
            document.getElementById("box").style.backgroundColor = "yellow";
        }

        function hideBox() {
            document.getElementById("box").style.display = "none";
        }
    </script>
</head>
<body>

    <h2>DOM Example</h2>

    <div id="box" style="border:1px solid black; padding:20px;">
        Welcome
    </div>

    <br>

    <button onclick="changeText()">
        Change Text
    </button>

    <button onclick="changeColor()">
        Change Color
    </button>

    <button onclick="hideBox()">
        Hide
    </button>

</body>
</html>
Assignment 8 

<!DOCTYPE html>
<html>
<head>
    <title>Simple Calculator</title>

    <script>
        function calculate(op) {

            var num1 = parseFloat(document.getElementById("num1").value);
            var num2 = parseFloat(document.getElementById("num2").value);
            var result;

            switch(op) {

                case "+":
                    result = num1 + num2;
                    break;

                case "-":
                    result = num1 - num2;
                    break;

                case "*":
                    result = num1 * num2;
                    break;

                case "/":
                    result = num1 / num2;
                    break;
            }

            document.getElementById("answer").innerHTML =
            "Result = " + result;
        }
    </script>
</head>
<body>

    <h2>Simple Calculator</h2>

    Enter Number 1:
    <input type="number" id="num1"><br><br>

    Enter Number 2:
    <input type="number" id="num2"><br><br>

    <button onclick="calculate('+')">+</button>
    <button onclick="calculate('-')">-</button>
    <button onclick="calculate('*')">*</button>
    <button onclick="calculate('/')">/</button>

    <h3 id="answer"></h3>

</body>
</html>
Assignment 9

<!DOCTYPE html>
<html>
<head>
    <title>Welcome Page</title>
</head>
<body>

    <?php

    date_default_timezone_set("Asia/Kolkata");

    echo "<h2>Welcome Student</h2>";

    echo "Current Date: " . date("d-m-Y");
    echo "<br>";

    echo "Current Time: " . date("h:i:s A");

    ?>

</body>
</html>
Assignment 10

<!DOCTYPE html>
<html>
<head>
    <title>POST Method Example</title>
</head>
<body>

<h2>Student Form</h2>

<form method="POST">

    Name:
    <input type="text" name="name"><br><br>

    Age:
    <input type="number" name="age"><br><br>

    <input type="submit" value="Submit">

</form>

<?php

if ($_SERVER["REQUEST_METHOD"] == "POST") {

    $name = $_POST["name"];
    $age = $_POST["age"];

    echo "<h3>Name: $name</h3>";

    if ($age >= 18) {
        echo "Eligible for Voting";
    }
    else {
        echo "Not Eligible for Voting";
    }
}

?>

</body>
</html>
Assignment 11

<!DOCTYPE html>
<html>
<head>
    <title>String Functions</title>
</head>
<body>

<?php

$string = "Web Development using PHP";

echo "<h2>Original String: $string</h2>";

// Length
echo "Length: " . strlen($string);
echo "<br><br>";

// Reverse
echo "Reverse: " . strrev($string);
echo "<br><br>";

// Uppercase
echo "Uppercase: " . strtoupper($string);
echo "<br><br>";

// Replace
echo "Replace: " . str_replace("PHP", "Python", $string);
echo "<br><br>";

// Substring
echo "Substring: " . substr($string, 0, 15);

?>

</body>
</html>
Assignment 12 


<!DOCTYPE html>
<html>
<head>
    <title>PHP Array</title>
</head>
<body>

<h2>Indexed Array</h2>

<?php

// Indexed Array
$tech = array("HTML", "CSS", "PHP");

echo "<ul>";

foreach ($tech as $value) {
    echo "<li>$value</li>";
}

echo "</ul>";

?>

<h2>Associative Array</h2>

<?php

// Associative Array
$marks = array(
    "Web Dev" => 85,
    "DSA" => 78,
    "Python" => 90
);

echo "<table border='1' cellpadding='10'>";

echo "<tr>
        <th>Subject</th>
        <th>Marks</th>
      </tr>";

foreach ($marks as $subject => $score) {

    echo "<tr>
            <td>$subject</td>
            <td>$score</td>
          </tr>";
}

echo "</table>";

?>

</body>
</html>
