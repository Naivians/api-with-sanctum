<h1 style="color: red;">LARAVEL API WITH SANCTUM</h1>

If you want to use this as a reference
first things first do the following

1. You should have PHP installed on your computer.
2. You should have composer installed on your computer.
3. open your xampp and create a database 'api_sanctum' or you can change this whatever you want.
4. before running rename the '.env.example' to '.env' otherwise it will not work because laravel cannot find the .env file.
5. go to config/sanctum.php and do your preferred setting or you can leave it as it is.

<h2>API ENDPOINTS</h2>
<p>this is for local development only. you may configure your proper domain during deployment.</p>

1. <p><b>Register</b></p> => http://127.0.0.1:8000/api/register
   **Parameters**
    1. name
    2. email
    3. password
    4. password_confirmation => you name you parameters according to this
<p><b>Return</b> **token** and **user object**</p>
       
2. <p><b>Login</b></p> http://127.0.0.1:8000/api/login
   **Parameters**
   1. name
   2. email
**return** => **token** and **user object**

3. <p>User</p> http://127.0.0.1:8000/api/user
the /user and the logout is protected by sanctum so in order to access these pages each request should have this header
<h2>Header</h2>
**Authorization: Bearer <YOUR_TOKEN>** => during login a token will be generated and this token will serve as the security acces for all pages
**return** => **user object**

5. <p>Logout</p> http://127.0.0.1:8000/api/logout
**Header**
**Authorization: Bearer <YOUR_TOKEN>**
