# Project Food Delivery[Backend Work]
Backend Part
Simple backend application built using Node.js, Express, and MongoDB through Mongoose. It implements user registration and login APIs, facilitating user authentication and storage. The application begins by importing necessary modules like Express for handling routes, Mongoose for database interactions, dotenv for environment variable management, and bcryptjs for password hashing.

The server is set up to handle Cross-Origin Resource Sharing (CORS) and to parse incoming JSON requests. It connects to a MongoDB database using a URI sourced from an environment variable to ensure that sensitive information remains secure. The user details, including username, email, and hashed password, are stored in a MongoDB collection using a defined Mongoose schema.

In the registration API (/register), user data is received via a POST request, and the password is hashed before creating a new user record in the database. The API responds with a confirmation message indicating successful user registration. The login API (/login) checks for user credentials by finding the email in the database and validating the password against the stored hashed password. If successful, it returns a message indicating a successful login along with the user's username; otherwise, it returns an error response for invalid credentials.

Finally, the application listens on port 5000, ready to handle incoming requests, providing a foundation for further expansion, including more features like session management, email verification, or profile updates. Overall, this code serves as a solid starting point for developing a user authentication system with Node.js and MongoDB.
