# from.php
<html>
<body>

<form method="post">

Name: <input type="text" name="name"><br><br>

Fname: <input type="text" name="fname"><br><br>

Lname: <input type="text" name="lname"><br><br>

Phone: <input type="text" name="phone"><br><br>

City: <input type="text" name="city"><br><br>

<input type="submit" name="send" value="Send">

</form>

<?php

if(isset($_POST['send']))
{
    echo $_POST['name']."<br>";
    echo $_POST['fname']."<br>";
    echo $_POST['lname']."<br>";
    echo $_POST['phone']."<br>";
    echo $_POST['city'];
}

?>

</body>
</html>