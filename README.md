# Forever Full Stack

Forever Full Stack is a full-stack web application that includes an admin panel, a frontend for users, and a backend server. The project is built using React, Vite, Express, and MongoDB. It also features role-based access control to manage different user permissions.

## Project Structure
forever-full-stack/ ├── admin/ │ ├── .env │ ├── .eslintrc.cjs │ ├── .gitignore │ ├── index.html │ ├── package.json │ ├── postcss.config.js │ ├── public/ │ ├── README.md │ ├── src/ │ ├── tailwind.config.js │ └── vite.config.js ├── backend/ │ ├── .env │ ├── .gitignore │ ├── config/ │ ├── controllers/ │ ├── middleware/ │ ├── models/ │ ├── package.json │ ├── routes/ │ ├── server.js │ └── vercel.json ├── frontend/ │ ├── .env │ ├── .eslintrc.cjs │ ├── .gitignore │ ├── index.html │ ├── package.json │ ├── postcss.config.js │ ├── public/ │ ├── README.md │ ├── src/ │ ├── tailwind.config.js │ └── vite.config.js └── How To Run Project.txt


## Features

- **Admin Panel**: Manage products, orders, and users.
- **User Frontend**: Browse products, place orders, and manage cart.
- **Backend Server**: Handle API requests, authentication, and database operations.
- **Role-Based Access Control**: Different permissions for admin and users.

## Role-Based Access Control

The project implements role-based access control to ensure that only authorized users can access certain features. The roles include:

- **Admin**: Can manage products, orders, and users.
- **User**: Can browse products, place orders, and manage their cart.

## Technologies Used

- **Frontend**: React, Vite, Tailwind CSS
- **Backend**: Express, MongoDB, Mongoose
- **Authentication**: JSON Web Tokens (JWT)
- **Payment Integration**: Stripe, Razorpay
- **File Uploads**: Cloudinary

## Setup Instructions

1. Clone the repository:
   ```git clone https://github.com/yourusername/forever-full-stack.git```

2. Install dependencies for backend:
    ```
    cd forever-full-stack/backend
    npm install
    ```

3. Install dependencies for frontend:
    ```cd ../frontend
        npm install
    ```

4. Install dependencies for the admin panel:
    ```cd ../admin
        npm install
    ```

5. Create a .env file in the backend directory and add your environment variables:
    ```
    PORT=4000
    MONGODB_URI=your_mongodb_uri
    CLOUDINARY_URL=your_cloudinary_url
    JWT_SECRET=your_jwt_secret
    ```

6. Run the backend server:
    ```cd ../backend
        npm run server
    ```

7. Start the frontend development server:
    ```cd ../frontend
        npm run dev
    ```

8. Start the admin panel development server:
    ```cd ../admin
        npm run dev
    ```