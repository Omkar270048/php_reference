# php_reference

```php
// Create connection
$conn = new mysqli(servername, username, password, database_name);

// Check connection
if ($conn->connect_error) {
  die("Connection failed: " . $conn->connect_error);
}
echo "Connected successfully";
?>
```

Creating Table
```php
CREATE TABLE TableName (
id INT(6) UNSIGNED AUTO_INCREMENT PRIMARY KEY,
firstname VARCHAR(30) NOT NULL,
lastname VARCHAR(30) NOT NULL,
email VARCHAR(50),
reg_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP
)
```

Insert value in table
```php
$sql = "INSERT INTO TableName (firstname, lastname, email)
VALUES ('John', 'Doe', 'john@example.com')";
```
