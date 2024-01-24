
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            color: #333;
            padding: 10px;
            text-align: right;
            font-size: 14px;
        }

        a {
            text-decoration: none;
            color: #333;
            padding: 5px;
            border-radius: 4px;
        }

        section {
            max-width: calc(100% - 20px); /* Adjusted max-width */
            margin: 20px auto;
            border: none; /* Remove border */
            padding: 10px; /* Added padding for the small box effect */
        }

        h2 {
            text-align: center;
            font-size: 18px;
            margin-bottom: 10px;
        }

        h2 span {
            display: block;
            font-weight: bold;
            font-size: 16px;
        }

        h3 {
            text-align: center;
            font-size: 16px;
            margin-bottom: 10px;
        }
       
        h4 {
            text-align: left;
            font-size: 6px;
            margin-bottom: 4px;
        }

        form {
            font-size: 10px; /* Adjusted font size */
            text-align: center;
        }

        .grey-box {
            background-color: #ddd;
            display: inline-block;
            padding: 5px;
            border-radius: 4px;
            margin: 5px; /* Added margin for separation */
        }

        form input {
            box-sizing: border-box;
            padding: 5px;
            border: 1px solid #ddd;
            border-radius: 4px;
            margin-bottom: 5px;
            width: auto; /* Adjusted width to fit content */
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }

        table,
        th,
        td {
            border: 1px solid #ddd;
        }

        th,
        td {
            padding: 12px;
            text-align: left;
        }

        th {
            background-color: #333;
            color: white;
        }

        .small-text {
            font-size: 8px; /* Adjusted font size to make it very small */
            text-align: left;
        }

        .tiny-text {
            font-size: 6px; /* Further reduced font size */
            text-align: left;
        }
    </style>
    <title>Your Website</title>
</head>

<body>

    <header>
        <a href="#">Logout</a>
    </header>

    <section>
        <h2>
            <span>Computer</span>
            <span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Networking</span>
            <span>Technology</span>
        </h2>
        <h3>Enter Course Grades</h3>

        <div class="grey-box">
            <form>
                <label for="firstName">First Name:</label>
                <input type="text" id="firstName" name="firstName" placeholder="First Name" required>

                <label for="lastName">Last Name:</label>
                <input type="text" id="lastName" name="lastName" placeholder="Last Name" required>

                <label for="courseNumber">Course Number:</label>
                <input type="text" id="courseNumber" name="courseNumber" placeholder="Course Number" required>

                <label for="finalGrade">Final Grade:</label>
                <input type="number" id="finalGrade" name="finalGrade" placeholder="Final Grade" required>

                <input type="submit" value="Submit">
                <input type="reset" value="Reset">
            </form>
        </div>

        <h4 class="tiny-text">The table below displays the contents of the FinalGrades.txt file located on the Webserver</h4>

        <table>
            <thead>
                <tr>
                    <th>First Name</th>
                    <th>Last Name</th>
                    <th>Course#</th>
                    <th>Grade</th>
                    <th>Letter Grade</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td id="outputFirstName"></td>
                    <td id="outputLastName"></td>
                    <td id="outputCourseNumber"></td>
                    <td id="outputFinalGrade"></td>
                    <td id="outputLetterGrade"></td>
                </tr>
                <!-- Add more rows as needed -->
            </tbody>
        </table>

        <p class="tiny-text">Clear Text file</p>
    </section>

    <script>
        // JavaScript code to update table based on form input
        document.querySelector('form').addEventListener('submit', function (event) {
            event.preventDefault();

            // Get form input values
            var firstName = document.getElementById('firstName').value;
            var lastName = document.getElementById('lastName').value;
            var courseNumber = document.getElementById('courseNumber').value;
            var finalGrade = document.getElementById('finalGrade').value;

            // Display values in the table
            document.getElementById('outputFirstName').innerText = firstName;
            document.getElementById('outputLastName').innerText = lastName;
            document.getElementById('outputCourseNumber').innerText = courseNumber;
            document.getElementById('outputFinalGrade').innerText = finalGrade;
            document.getElementById('outputLetterGrade').innerText = getLetterGrade(finalGrade);
        });

        // Function to get letter grade based on numeric grade
        function getLetterGrade(grade) {
            if (grade >= 90) {
                return 'A';
            } else if (grade >= 80) {
                return 'B';
            } else if (grade >= 70) {
                return 'C';
            } else if (grade >= 60) {
                return 'D';
            } else {
                return 'F';
            }
        }
    </script>

</body>

</html>
