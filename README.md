# from.php
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Registration Form</title>
</head>
<body>

    <h2>Registration Form</h2>

    <form method="post">

        Name:
        <input type="text" name="name"><br><br>

        First Name:
        <input type="text" name="fname"><br><br>

        Last Name:
        <input type="text" name="lname"><br><br>

        Phone:
        <input type="tel" name="phone"><br><br>

        City:
        <input type="text" name="city"><br><br>

        <input type="submit" name="submit" value="Submit">

    </form>

    <?php
    if (isset($_POST['submit'])) {

        echo "Name: " . htmlspecialchars($_POST['name']) . "<br>";
        echo "First Name: " . htmlspecialchars($_POST['fname']) . "<br>";
        echo "Last Name: " . htmlspecialchars($_POST['lname']) . "<br>";
        echo "Phone: " . htmlspecialchars($_POST['phone']) . "<br>";
        echo "City: " . htmlspecialchars($_POST['city']) . "<br>";

    }
    ?>

</body>
</html>