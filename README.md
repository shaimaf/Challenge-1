<!DOCTYPE html>
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
            background-color: white;
            color: #333;
            padding: 10px;
            text-align: left;
            font-size: 14px;
        }

        section {
            max-width: 600px;
            margin: 20px auto;
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        form {
            font-size: 12px;
        }

        form label {
            display: inline-block;
            width: 150px; /* Adjusted width to provide some spacing */
        }

        form input {
            width: calc(100% - 160px); /* Adjusted width to make the input take the remaining space */
            box-sizing: border-box; /* Included to ensure the total width includes padding and border */
            margin-bottom: 10px; /* Added margin for spacing between inputs */
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
    </style>
    <title>Your Website</title>
</head>

<body>

    <header>
        <a href="#" style="text-decoration: none; color: #333;">Logout</a>
    </header>

    <section>
        <h2>COMPUTER NETWORKING TECHNOLOGY</h2>
        <h3>Enter Course Grades</h3>

        <form>
            <label for="firstName">Full Name: First Name Only</label>
            <input type="text" id="firstName" name="firstName" required>

            <label for="lastName">Last Name: Last Name Only</label>
            <input type="text" id="lastName" name="lastName" required>

            <label for="courseNumber">Course Number</label>
            <input type="text" id="courseNumber" name="courseNumber" required>

            <label for="finalGrade">Final Grade</label>
            <input type="number" id="finalGrade" name="finalGrade" required>

            <input type="submit" value="Submit">
            <input type="reset" value="Reset">
        </form>

        <h3>The table below displays the contents of the FinalGrades.txt file located on the Webserver</h3>

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
                    <td>Chris</td>
                    <td>Arsenault</td>
                    <td>CNET2020</td>
                    <td>95</td>
                    <td>A</td>
                </tr>
                <!-- Add more rows as needed -->
            </tbody>
        </table>

        <p>Clear Text file</p>
    </section>

</body>

</html>



        <p>Clear Text file</p>
    </section>

</body>
</html>