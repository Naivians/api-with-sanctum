If you want to use this as a reference
first things first do the following

1. You should have PHP installed on your computer
2. You should have composer installed on your computer
3. open your xampp and create a database 'api_sanctum' or you can change this whatever you want
4. before running rename the '.env.example' to '.env' otherwise it will not work because it won't be abale to locate the .env file
5. go to config/sanctum.php and do your preferred setting or you can leave it as it is

**API ENDPOINTS**
this is for local development only. you may configure your proper domain when during deployment.

1. **/Register** => http://127.0.0.1:8000/api/register
   **Parameters**
    1. name
    2. email
    3. password
    4. password_confirmation => you name you parameters according to this
       
2. **/Login**
   **Parameters**
   1. name
   2. email
**return** => token and user object

3. **/User**
the /user and the logout is protected by sanctum so in order to access these pages each request should have this header
**Header**
**Authorization: Brearer <YOUR_TOKEN>** => during login a token will be generated and this token will serve as the security acces for all pages

4. **/logout**
**Header**
**Authorization: Brearer <YOUR_TOKEN>**
