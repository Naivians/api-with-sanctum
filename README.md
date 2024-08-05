<h1>LARAVEL API WITH SANCTUM</h1>
<p>If you want to use this as a reference first things first do the following</p>

1. You should have PHP installed on your computer.
2. You should have composer installed on your computer.
3. open your xampp and create a database 'api_sanctum' or you can change this whatever you want.
4. before running rename the '.env.example' to '.env' otherwise it will not work because laravel cannot find the .env file.
5. go to config/sanctum.php and do your preferred setting or you can leave it as it is.

<h2>API ENDPOINTS</h2>
<p>This is for local development only. you may configure your proper domain during deployment.</p>

<p><strong>Register</strong>: http://127.0.0.1:8000/api/register</p>
<p><strong>Parameters</strong></p>
<ol>
    <li>name</li>
    <li>email</li>
    <li>password</li>
    <li>password_confirmation</li>
</ol>
<p><strong>Return</strong> => TOKEN and USER OBJECTS</p>

<p><strong>Login</strong>: http://127.0.0.1:8000/api/login</p>
<p><strong>Parameters</strong></p>
<ol>
    <li>name</li>
    <li>email</li>
</ol>
<p><strong>Return</strong> => TOKEN and USER OBJECTS</p>


<p><strong>User</strong>: http://127.0.0.1:8000/api/user</p>
<p><strong>Note: </strong> => user and the logout is protected by sanctum so in order to access these pages each request should have this header</p>
<p><strong>(Header)</strong> => Authorization: Bearer (YOUR_TOKEN)</p>
<p><strong>Return</strong> => TOKEN and USER OBJECTS</p>


<p><strong>Logout</strong>: http://127.0.0.1:8000/api/logout</p>
<p><strong>(Header)</strong> => Authorization: Bearer (YOUR_TOKEN)</p>
<p><strong>Return</strong> => Logout Successfully</p>


