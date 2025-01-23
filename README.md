# API-S
 This is a simple REST API built with Node.js and Express.jsfor managing users.
The API supports CRUD operations that is Create Read Update and Delete.
##Set Up
 1. Clone the repository
 2. Run 'npm install'
 3. Start the Server: 'node index.js'
 4. API will be available at 'http://localhost:3000'
 ##  API Endpoints
 GET: Retrieves a list of all users
 Response: (200) OK
           Body:Array of users
               id , name, email
POST: Create a new user 
      /api/users
      Request: Body: (name,username required)
                     (email, useremail required)
      Response: (201) Created Successfully
               Body: Created user 
               (400) Bad request:If email or name is missing               
PUT: Updates a user/api/user/:id
    Request: Body (name: updated username)
                  (email: updated useremail)
    Response: (200) OK
              Body(updated user)
    (404) Not found if the user is given an ID that doesn't exist

DELETE: Removes a user /api/users/:id
  (204) No content :If the user was deleted successfully
  (404) Not found :If the user with the given ID does not exist
  
Error Handling 
This API returns :
400 Bad Request
404 Not Found
TRhis project is licensed under the MIT License
