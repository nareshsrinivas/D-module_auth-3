
1️⃣ User Signup (Registration)
URL: http://127.0.0.1:8000/api/signup/
Method: POST
Postman/Thunder Client Settings:

Method: POST
URL: http://127.0.0.1:8000/api/signup/
Headers:
Accept: application/json
Content-Type: application/json
Body:

{
      "username": "testuser",
      "email": "test@example.com",
      "mobile_number": "+919876543210",
      "password": "TestPass123!",
      "password2": "TestPass123!"
  }



2️⃣ User Login
URL: http://127.0.0.1:8000/api/login/
Method: POST
Postman/Thunder Client Settings:

Method: POST
URL: http://127.0.0.1:8000/api/login/
Headers:
Body:

{
      "email": "test@example.com",
      "password": "TestPass123!"
  }


3️⃣ Get User Profile
URL: http://127.0.0.1:8000/api/profile/
Method: GET
Postman/Thunder Client Settings:

Method: GET
URL: http://127.0.0.1:8000/api/profile/
Headers:

Authorization: Bearer YOUR_ACCESS_TOKEN_HERE
  Content-Type: application/json


4️⃣ Update User Profile
URL: http://127.0.0.1:8000/api/profile/
Method: PUT or PATCH
Postman/Thunder Client Settings:

Method: PUT (or PATCH)
URL: http://127.0.0.1:8000/api/profile/
Headers:

Authorization: Bearer YOUR_ACCESS_TOKEN_HERE
  Content-Type: application/json

Body:

{
      "username": "updateduser",
      "mobile_number": "+919876543211"
  }


5️⃣ Change Password
URL: http://127.0.0.1:8000/api/change-password/
Method: POST
Postman/Thunder Client Settings:

Method: POST
URL: http://127.0.0.1:8000/api/change-password/
Headers:
Authorization: Bearer YOUR_ACCESS_TOKEN_HERE
  Content-Type: application/json

Body:

{
      "old_password": "TestPass123!",
      "new_password": "NewSecurePass456!"
  }


6️⃣ List All Users
URL: http://127.0.0.1:8000/api/users/
Method: GET
Postman/Thunder Client Settings:

Method: GET
URL: http://127.0.0.1:8000/api/users/
Headers:

Authorization: Bearer YOUR_ACCESS_TOKEN_HERE
  Content-Type: application/json


7️⃣ Delete User Account
URL: http://127.0.0.1:8000/api/profile/
Method: DELETE
Postman/Thunder Client Settings:

Method: DELETE
URL: http://127.0.0.1:8000/api/profile/
Headers:

Authorization: Bearer YOUR_ACCESS_TOKEN_HERE
  Content-Type: application/json

8️⃣ Refresh Token
URL: http://127.0.0.1:8000/api/token/refresh/
Method: POST
Postman/Thunder Client Settings:

Method: POST
URL: http://127.0.0.1:8000/api/token/refresh/
Headers:

Body:
{
      "refresh": "YOUR_REFRESH_TOKEN_HERE"
  }


9️⃣ Logout
URL: http://127.0.0.1:8000/api/logout/
Method: POST
Postman/Thunder Client Settings:

Method: POST
URL: http://127.0.0.1:8000/api/logout/
Headers:

Authorization: Bearer YOUR_ACCESS_TOKEN_HERE
  Content-Type: application/json

Body:

{
      "refresh": "YOUR_REFRESH_TOKEN_HERE"
  }