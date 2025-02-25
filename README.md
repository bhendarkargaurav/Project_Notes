# important notes

    1. NPM
    npm (Node Package Manager) is a package manager for JavaScript, and it is the default package manager for the Node.js JavaScript runtime environment. It helps developers manage dependencies for their projects, allowing them to easily install, update, and manage libraries and packages that their applications rely on.
    Key Features of npm
    Package Installation
    Dependancy management
    Package Publishing
    Script: npm allows you to define custom scripts in your package.json file, which can be run using the npm run command. 
     
    What Does body-parser Do?
    body-parser is a middleware for Node.js that allows you to parse incoming request bodies in a middleware before your handlers. It supports various types of request bodies, including JSON and URL-encoded data.
    Parse incoming request" means to read and interpret the data sent with an HTTP request so that it can be used by the server-side application. When a client (like a web browser or a mobile app) sends a request to a server, it often includes data in the request body. This data needs to be parsed so that the server can understand and process it.
     
    Nodemon is a utility that helps to develop Node.js applications by automatically restarting the application when file changes in the directory are detected. It is particularly useful during development because it eliminates the need to manually stop and restart the server each time you make changes to your code.
    Automatic Restart: Nodemon watches for changes in your files and automatically restarts your Node.js application when it detects any changes.
 
 
    • Controllers: Controllers handle the incoming HTTP requests and define the logic for processing them. They interact with services or models to fetch and manipulate data, and then send responses back to the client.
    • Middlewares: Middlewares are functions that process requests before they reach the controllers. They are used for tasks like authentication, logging, validation, and error handling, providing reusable functionality across the application.
    • Repository: The repository layer is responsible for interacting with the database. It abstracts the data access logic, making it easier to manage CRUD operations and other database queries in a centralized manner..

46. For Node.js, why does Google use the V8 engine?
The V8 engine, developed by Google, is open-source and written in C++. Google Chrome makes use of this engine. V8, unlike the other engines, is also utilized for the popular Node.js runtime. V8 was initially intended to improve the speed of JavaScript execution within web browsers. Instead of employing an interpreter, V8 converts JavaScript code into more efficient machine code to increase performance. It turns JavaScript code into machine code during execution by utilizing a JIT (Just-In-Time) compiler, as do many current JavaScript engines such as SpiderMonkey or Rhino (Mozilla).

    2. Setup Express:

    const express = require('express');
    const bodyParser = require('body-parser');
    
    const app = express();
    const port = 3000;
    
    // Middleware to parse JSON bodies
    app.use(bodyParser.json());
    
    // Basic route
    app.get('/', (req, res) => {
      res.send('Hello, World!');
    });
    
    // Start the server
    app.listen(port, () => {
      console.log(`Server running at http://localhost:${port}`);
    });
    
Which database is more popularly used with Node.js?
MongoDB is the most common database used with Node.js. It is a NoSQL, cross-platform, document-oriented database that provides high performance, high availability, and easy scalability.

Why use Express.Js?
Express.js is a lightweight Node.js framework that gives us ability to create server-side web applications faster and smarter. The main reason for choosing Express is its simplicity, minimalism, flexibility, and scalability characteristics. It provides easy setup for middlewares and routing.

DSA ?
Algorithm is a step-by-step procedure for solving a problem or accomplishing a task. In the context of data structures and algorithms, it is a set of well-defined instructions for performing a specific computational task.
Elements in an array can be modified by assigning a new value to their corresponding index.

*Git?
Git is a distributed version control system (VCS) that allows developers to track changes in their codebase over time. It manages source code history, facilitates collaboration among team members, and enables branching and merging for parallel development.
    Usage: Git is primarily used for managing source code and tracking its evolution, facilitating collaboration among developers on a project.
GitHub
    • Definition: GitHub is a web-based platform that provides Git repository hosting along with additional collaboration features. It extends Git’s functionality by offering a centralized cloud-based platform for project management, code review, issue tracking, and team collaboration.
          
Nature:
    • Git is a version control system designed for tracking changes in code locally and facilitating distributed development.
    • GitHub is a web-based platform that provides Git repository hosting, collaboration tools, and project management features.

Sequelize: 
    Sequelize is a popular Node.js ORM (Object-Relational Mapping) library that provides an easy-to-use interface for interacting with SQL databases. It supports various SQL databases such as MySQL, PostgreSQL, SQLite, and MSSQL, allowing developers to work with databases using JavaScript 
    Sequelize provides a powerful querying API that supports CRUD operations (Create, Read, Update, Delete) and complex queries using methods like findAll, findOne, create, update, and destroy.
    
Sequelize-cli:
    The sequelize-cli is a command-line interface (CLI) tool for Sequelize
    • Create Migrations: Generate migration files to manage changes in database schema over time (sequelize-cli migration:generate).
    • Run Migrations: Apply pending migrations to update the database schema (sequelize-cli db:migrate).
    • Undo Migrations: Roll back the last migration (sequelize-cli db:migrate:undo).
    • Same for Seeders:

Mysql2:
    mysql2 is a Node.js client library for MySQL databases that provides fast and efficient connectivity. It is an enhanced version of the original mysql package with several improvements, including support for promises, async/await, and better performance.

# Interesting fact about js
JavaScript was created in just 10 days! In May 1995, Netscape Communications Corporation tasked Brendan Eich with developing a scripting language that would complement Java and appeal to non-professional programmers. Eich created JavaScript (originally called Mocha, then LiveScript) in just 10 days. Despite its quick inception, JavaScript has grown to become one of the most popular and essential programming languages in the world, particularly for web development.

# Nodejs Interview Preparation start
1. Why use Node.js?
Node.js makes building scalable network programs easy. Some of its advantages include:

It is generally fast
It rarely blocks
It offers a unified programming language and data type
Everything is asynchronous 
It yields great concurrency

1. What is Node.js? Where can you use it?
Node.js is an open-source, cross-platform JavaScript runtime environment and library to run web applications outside the client’s browser. It is used to create server-side web applications.

Node.js is perfect for data-intensive applications as it uses an asynchronous, event-driven model. You can use  I/O intensive web applications like video streaming sites. You can also use it for developing: Real-time web applications, Network applications, General-purpose applications, and Distributed systems.

2. Which database is more popularly used with Node.js?
MongoDB is the most common database used with Node.js. It is a NoSQL, cross-platform, document-oriented database that provides high performance, high availability, and easy scalability.

3. What is NPM?
NPM stands for Node Package Manager, responsible for managing all the packages and modules for Node.js.

Node Package Manager provides two main functionalities:
Provides online repositories for node.js packages/modules, which are searchable on search.nodejs.org
Provides command-line utility to install Node.js packages and also manages Node.js versions and dependencies  

Node.js is a super popular server-side platform that more and more organizations are using. If you are preparing for a career change and have an upcoming job interview, it’s always a good idea to prepare and brush up on your interview skills beforehand. Although there are a few commonly asked Node.js interview questions that pop up during all types of interviews, we also recommend that you prepare by focusing on exclusive questions to your specific industry.

Want a Top Software Development Job? 
jwt

.js is a lightweight Node.js framework that gives us ability to create server-side web applications faster and smarter. The main reason for choosing Express is its simplicity, minimalism, flexibility, and scalability characteristics. It provides easy setup for middlewares and routing.

1. What is Express.Js?
Express is a small framework that sits on top of Node.js’s web server functionality to simplify its APIs and add helpful new features. It makes it easier to organize your application’s functionality with middleware and routing; it adds helpful utilities to Node.js’s HTTP objects; it facilitates the rendering of dynamic HTTP objects.

Express is a part of MEAN stack, a full stack JavaScript solution used in building fast, robust, and maintainable production web applications.
Express.js is a lightweight Node.js framework that gives us ability to create server-side web applications faster and smarter. The main reason for choosing Express is its simplicity, minimalism, flexibility, and scalability characteristics. It provides easy setup for middlewares and routing.
1. What is Node.js? Where can you use it?
Node.js is an open-source, cross-platform JavaScript runtime environment and library to run web applications outside the client’s browser. It is used to create server-side web applications.

Node.js is perfect for data-intensive applications as it uses an asynchronous, event-driven model. You can use  I/O intensive web applications like video streaming sites. You can also use it for developing: Real-time web applications, Network applications, General-purpose applications, and Distributed systems.

2. Why use Node.js?
Node.js makes building scalable network programs easy. Some of its advantages include:

It is generally fast
It rarely blocks
It offers a unified programming language and data type
Everything is asynchronous 
It yields great concurrency
3. How does Node.js work?
A web server using Node.js typically has a workflow that is quite similar to the diagram illustrated below. Let’s explore this flow of operations in detail.

Node.js Architecture Workflow

3. What is the difference between asynchronous and synchronous functions?
Synchronous functions block the execution of other code until they are complete, while asynchronous functions allow other code to continue executing while they are running, making them essential for writing scalable Node.js applications.

Clients send requests to the webserver to interact with the web application. Requests can be non-blocking or blocking:
Querying for data
Deleting data 
Updating the data
Node.js retrieves the incoming requests and adds those to the Event Queue
The requests are then passed one-by-one through the Event Loop. It checks if the requests are simple enough not to require any external resources
The Event Loop processes simple requests (non-blocking operations), such as I/O Polling, and returns the responses to the corresponding clients
A single thread from the Thread Pool is assigned to a single complex request. This thread is responsible for completing a particular blocking request by accessing external resources, such as computation, database, file system, etc.

Once the task is carried out completely, the response is sent to the Event Loop that sends that response back to the client.
MongoDB is the most common database used with Node.js. It is a NoSQL, cross-platform, document-oriented database that provides high performance, high availability, and easy scalability.
Want a Top Software Development Job? Start Here!
Full Stack Developer - MERN StackExplore ProgramWant a Top Software Development Job? Start Here!
4. Why is Node.js Single-threaded?
Node.js is single-threaded for async processing. By doing async processing on a single-thread under typical web loads, more performance and scalability can be achieved instead of the typical thread-based implementation.
it all are imp
Why is Node.js Single-threaded?
Node.js is single-threaded for async processing. By doing async processing on a single-thread under typical web loads, more performance and scalability can be achieved instead of the typical thread-based implementation.
# Express
What Is Express JS?     
Express is a node js web application framework that provides broad features for building web and mobile applications. It is used to build a single page, multipage, and hybrid web application.
Node.js is perfect for data-intensive applications as it uses an asynchronous, event-driven model. You can use  I/O intensive web applications like video streaming sites. You can also use it for developing: Real-time web applications, Network applications, General-purpose applications, and Distributed systems.
   # Powerful Expressjs Features That You Need to Know
Routing Capabilities. ...
Express Middleware functionality. ...
Templating Engine Support. ...
MVC Architecture Support. ...
Easy and Flexible API Development. ...
Error Handling Abilities. ...
JSON Web Token (JWT) Integration. ...

Mentions few features of Express.js.
Few features of the Express.js includes

What is Authentication?
Authentication is the process of verifying the identity of a user or system. In the context of web development, authentication is commonly used to grant access to users based on their credentials, such as username and password.

Routing: Express provides a simple way to define routes for handling HTTP requests. Routes are used to map different URLs to specific pieces of code, making it easy to organize your application's logic.
Middleware: Express uses middleware functions to perform tasks during the request-response cycle. Middleware functions have access to the request, response, and the next middleware function.
HTTP Utility Methods: Express mainly used for handling HTTP methods like GET, POST, PUT, and DELETE. This makes it easy to define how the application should respond to different types of HTTP requests.
Static File Serving: It can also serve static files, such as images, CSS, and JavaScript, with the help of built-in express.static middleware.
Security: It includes features and middleware to strengthen the security of your web applications, such as the helmet middleware to secure your app.

MongoDB: MongoDB is a NoSQL database that shops records in a bendy, JSON-like format. It is used because the database for storing OTP and associated data on this software. MongoDB's flexibility makes it suitable for storing unstructured or semi-structured information like OTPs.
done.

 What is .env file used for?
The .env file is used for storing sensitive information in a web application which we don't want to expose to others like password, database connection string etc. It is a simple text file where each line represents a key-value pair, and these pairs are used to configure various aspects of the application.
