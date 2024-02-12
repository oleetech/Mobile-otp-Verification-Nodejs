# Mobile-otp-Verification-Nodejs


## OTP Registration API Documentation

This API provides endpoints for OTP registration, login, and verification.

## Endpoints

1. **Register User:**
   - URL: `http://127.0.0.1:3000/api/users/register`
   - Method: POST
   - Request Body:
     ```json
     {
         "phoneNumber": "YOUR_PHONE_NUMBER",
         "name": "YOUR_NAME",
         "password": "YOUR_PASSWORD"
     }
     ```
   - Response:
     ```json
     {
         "message": "User registered successfully",
         "id": "USER_ID"
     }
     ```

2. **Verify OTP:**
   - URL: `http://127.0.0.1:3000/api/users/verify`
   - Method: POST
   - Request Body:
     ```json
     {
         "phoneNumber": "YOUR_PHONE_NUMBER",
         "otp": "YOUR_OTP"
     }
     ```
   - Response:
     ```json
     {
         "message": "OTP verified successfully"
     }
     ```

3. **Login:**
   - URL: `http://127.0.0.1:3000/api/users/login`
   - Method: POST
   - Request Body:
     ```json
     {
         "phoneNumber": "YOUR_PHONE_NUMBER",
         "password": "YOUR_PASSWORD"
     }
     ```
   - Response:
     ```json
     {
         "token": "YOUR_JWT_TOKEN"
     }
     ```
