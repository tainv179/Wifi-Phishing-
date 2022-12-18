# Wifi-Phishing


SET PASSWORD FOR 'root'@localhost = PASSWORD("myReallyStrongPwd");


<?php
$servername = "localhost";
$database = "rogue_AP";
$username = "root";
$password = "myPass170901";
// Create connection
$conn = mysqli_connect($servername, $username, $password, $database);
// Check connection
if (!$conn) {
      die("Connection failed: " . mysqli_connect_error());
}
 
echo "Connected successfully";
$sql = "insert into wpa_keys(password1, password2) values ('tes2tpass', 'tes2tpass')";
if (mysqli_query($conn, $sql)) {
      echo "New record created successfully";
} else {
      echo "Error: " . $sql . "<br>" . mysqli_error($conn);
}
mysqli_close($conn);
?>
    



https://github.com/wifiphisher/wifiphisher
