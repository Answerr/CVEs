SQL Injection in /Admin/login.php        Row 10 and 11 has vulnerability![image-20240408163713811](C:\Users\Jason\AppData\Roaming\Typora\typora-user-images\image-20240408163713811.png)

$result = mysqli_query($conn,$sql);

![image-20240408163830757](C:\Users\Jason\AppData\Roaming\Typora\typora-user-images\image-20240408163830757.png)

![image-20240408163842153](C:\Users\Jason\AppData\Roaming\Typora\typora-user-images\image-20240408163842153.png)

SELECT * FROM users WHERE username= or true=true -- //**''' and password = '".$password."'";**     which is Spliced sql statements

![image-20240408164543299](C:\Users\Jason\AppData\Roaming\Typora\typora-user-images\image-20240408164543299.png)

![image-20240408164554016](C:\Users\Jason\AppData\Roaming\Typora\typora-user-images\image-20240408164554016.png)