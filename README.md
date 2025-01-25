
#  Blog Site Management API

This project involves building a backend for a blogging platform with role-based access control for Admin and User roles. The Admin can manage users and delete any blog, while Users can create, update, and delete their own blogs. The backend features secure authentication and authorization using JWTs, with public APIs for viewing blogs, including search, sort, and filter functionalities.


## ✨ Features
#### User Roles :

* Admin: Can delete blogs, block users, and manage the platform.
* User: Can register, log in, and perform CRUD operations on their blogs.
#### Authentication & Authorization :

* Users must log in to perform protected operations.
#### Admin and User permissions are strictly enforced Blog Management:

* Public API supports fetching blogs with search, sort, and filter options.
Users can create, update, or delete their blogs.
Models:

* User: Includes name, email, password, role, and block status.
* Blog: Stores title, content, author reference, and timestamps.
#### Error Handling:

* Centralized responses for validation, authentication, authorization, and server errors ensure consistency.


# 🛠️ Technology Stack
* Language: TypeScript
* Framework: Express.js
* Database: MongoDB
* (ODM)library: Mongoose

* Other Tools: 
     * ts-node-dev for development with TypeScript
     * dotenv for environment variable management

     * eslint and prettier for code linting and formatting
## API Endpoints

## Users

| Method | Endpoint     | **Description** |
| :-------- | :------- | :------------------------- |
| `POST` | ```https://blog-fawn-sigma.vercel.app/api/auth/register``` | Register User |
| `POST` | `https://blog-fawn-sigma.vercel.app/api/auth/login` | Login User |
| `POST` | `https://blog-fawn-sigma.vercel.app/api/blogs` | Create Blog |
| `UPDATE` | `https://blog-fawn-sigma.vercel.app/api/blogs/:id` | Update Blog |
| `DELETE` | `https://blog-fawn-sigma.vercel.app/api/blogs/:id` | Delete Blog |

## Public

| Method | Endpoint     | **Description** |
| :-------- | :------- | :------------------------- |
| `GET` | `https://blog-fawn-sigma.vercel.app/api/blogs` | Get All Blogs |
| `GET` | `https://blog-fawn-sigma.vercel.app/api/blogs?search=technology&sortBy=createdAt&sortOrder=desc&filter=67950d81f31d9350c1837e2e` | Search SortBy SortOrder Filter |


## Admin 

| Method | Endpoint     | **Description** |
| :-------- | :------- | :------------------------- |
| `PATCH` | `https://blog-fawn-sigma.vercel.app/api/admin/users/:userId/block` | Block User |
| `DELETE` | `https://blog-fawn-sigma.vercel.app/api/admin/blogs/:id` | Delete Blog |


## Projects Related All Links & Documents :


* Live Deployment Link (Server) :
```
https://blog-fawn-sigma.vercel.app/

```
* GitHub Repository Links (Server)  :
```
https://github.com/SUJAIT/assignment-iii.git

```
* Admin login crediential (email and password) :

```http
Gmail : admin@gmail.com
Password : admin

```
* Project Overview Video. (A brief video providing an overview of the project.) :
```http
https://youtu.be/EF6fqnnl3Uk?si=p_0JCeXvXx2tOSgr
```

