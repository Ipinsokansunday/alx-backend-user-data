#



User model: Create a SQLAlchemy model User with attributes like id, email, hashed_password, etc.
Create user: Implement the add_user method in the DB class to save new users to the database.
Find user: Implement the find_user_by method to locate users by arbitrary keyword arguments.
Update user: Implement the update_user method to update attributes of a user.
Hash password: Implement _hash_password using bcrypt.hashpw.
Register user: Implement Auth.register_user to handle user registration.
Basic Flask app: Set up a simple Flask app to handle user-related API routes.
Credentials validation: Implement Auth.valid_login to validate user credentials.
Routes
GET /: returns logout message when user is logged out
GET /profile returns email of logged in user
POST /users: creates new user (Form data: email, password)
POST /sessions: logs in existing user(Form data: email, password)
POST /reset_password: returns password reset token (Form data: email)
PUT /reset_password: updates existing user's password (Form data: email, new_password, reset_token)
DELETE /sessions: logs out user
