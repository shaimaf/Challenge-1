
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
            max-width: 600px;
            margin: 20px auto;
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            border: none; /* Remove border */
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

        form {
            font-size: 12px;
            display: flex;
            flex-wrap: wrap;
            gap: 5px;
        }

        form label {
            flex: 0 0 25%;
            text-align: right;
            margin-right: 10px;
        }

        form input {
            flex: 1;
            box-sizing: border-box;
            padding: 5px;
            border: 1px solid #ddd;
            border-radius: 4px;
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
        <a href="#">Logout</a>
    </header>

    <section>
        <h2>
            <span>Computer</span>
            <span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Networking</span>
            <span>Technology</span>
        </h2>
        <h3>Enter Course Grades</h3>

        <form>
            <label for="firstName">First Name:</label>
            <input type="text" id="firstName" name="firstName" placeholder="First Name Only" required>

            <label for="lastName">Last Name:</label>
            <input type="text" id="lastName" name="lastName" placeholder="Last Name Only" required>

            <label for="courseNumber">Course Number:</label>
            <input type="text" id="courseNumber" name="courseNumber" placeholder="Course Number" required>

            <label for="finalGrade">Final Grade:</label>
            <input type="number" id="finalGrade" name="finalGrade" placeholder="Final Grade" required>

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


    </section>

</body>

</html>





