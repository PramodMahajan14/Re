
1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/your-username/node-api.git

2. step:
    ```bash
    cd node-api
3. step
    ```
      npm intall

4. step : Make sure create .env file and include following credentials
   ```bash
     DB=YOUR MONGODB URI
     CLIENT_URL= YOUR_CLIENT_SIDE_URL
     ACCESS_TOKEN_SECRET= PUT_ANY_STRING
     REFRESH_TOKEN_SECRET = PUT_ANY_STRING
     SMTP_USER = EMAIL_ADDRESS
     SMTP_PASSWOR = EMAIL_PASSWORD  
 
5. step : start your main file 
   ```
   node index


### API Endpoints

In this project has 9 Endpoints

1 SIGNUP: After the signup we will get mail,once click 'verify' then w'll redirect  http://localhost:4000/api/auth/verify/${userId}
then user will be verified.And redirect to client side for showing the verification done
  ```
    POST http://localhost:4000/v1/api/signup

2 SIGNIN : w'll get  token 
  ```
    POST http://localhost:4000/v1/api/signin

3.ACCESS-TOKEN: make sure, token passed in header section, then  w'll get  accesstoken
   ```
    GET http://localhost:4000/v1/api/access


4 Profile : must add accesstoken in header section, then call 
  ```
    GET http://localhost:4000/v1/api/profile
    
5 NEWTask : In this endpoint, date and time is optionally if we passed dateTime, after that time w'll get Notification through mail 
  ```
    POST http://localhost:4000/v1/api/newtask/:userId

6 ALLTASK :w'll get signin user all tasks 
  ```
    GET http://localhost:4000/v1/api/profile

7 TASK :w'll get Specific tasks by passing task id
  ```
    GET http://localhost:4000/v1/api/tasks/:id

8 UPDATETASK 
  ```
    GET http://localhost:4000/v1/api/updatetask/:id/:userId
    
9 DELETETASK 
  ```
    GET http://localhost:4000/v1/api/removetask/:id
    
