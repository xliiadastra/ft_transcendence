# ft_transcendence
1. Project Setup
NestJS
NestJS is a progressive Node.js framework for building efficient and scalable server-side applications. It uses modern JavaScript or TypeScript and combines elements of OOP (Object Oriented Programming), FP (Functional Programming), and FRP (Functional Reactive Programming).

To get started with NestJS:
Install Node.js and npm on your system.
Install the Nest CLI globally using npm i -g @nestjs/cli.
Create a new project using nest new project-name.
NestJS Key Concepts:
Modules: A module is a class annotated with a @Module() decorator. The @Module() decorator provides metadata that Nest makes use of to organize the application structure. Every application has at least one module, a root module, which is the starting point of the application.

Controllers: A controller handles HTTP requests. Each controller should be a class with the @Controller() decorator. This decorator can take an optional string that defines the route path.

Providers/Services: Providers are a fundamental concept in Nest. Many of the basic Nest classes can be treated as a provider – services, repositories, factories, helpers, etc. The @Injectable() decorator marks a class as a provider.

Middleware: Middleware is a function that is called before the route handler. It has access to the client request and the server response objects.

Svelte
Svelte is a modern component-based JavaScript framework similar to React and Vue. It has a unique approach: it compiles your code to tiny, framework-less vanilla JS which leads to faster load times and improved performance.

To get started with Svelte:
Install Node.js and npm.
Use the degit tool to create a new project template: npx degit sveltejs/template svelte-app.
Move into the new project folder and install dependencies: cd svelte-app && npm install.
Svelte Key Concepts:
Components: Svelte is a component-based framework, which means you build your UI using components. A Svelte component is a reusable, self-contained block of code that encapsulates HTML, CSS, and JavaScript that belongs to the component.

Reactivity: Svelte has a different way to handle reactivity compared to other frameworks. You can declare reactive variables using a simple = syntax.

Stores: Stores are used to manage application state in Svelte. They provide a way to hold state, and notify components when that state has changed.

PostgreSQL
PostgreSQL is a powerful, open source object-relational database system.

You will need to install PostgreSQL, set up a database and integrate it with your NestJS backend.

For integration, you can use TypeORM which is an ORM that can run in NodeJS and can be used with TypeScript and JavaScript (ES5, ES6, ES7, ES8) and supports both Active Record and Data Mapper patterns. You can also use Sequelize which is a promise-based Node.js ORM for PostgreSQL.

Docker
Docker allows you to package your application and its dependencies in a "container" which can then be easily shared and deployed. Docker Compose, a tool for defining and running multi-container Docker applications, allows you to manage your app's services.

You'll use Docker to run your PostgreSQL database and NestJS app in different containers. Docker Compose will be used to define and run the multi-container application.

2. Security Concerns
Password Hashing: Passwords should never be stored as plain text. You'll need to use a strong hashing algorithm. Libraries like bcrypt, scrypt or Argon2 can be used for password hashing.

SQL Injections: You need to make sure your app is protected from SQL Injection attacks. Using an ORM like Sequelize or TypeORM can help prevent SQL Injections.

Form Validation: All form inputs should be validated on server-side to prevent bad data being injected into your database. You can use libraries like class-validator with NestJS for input validation.

3. User Account
OAuth with 42 intranet means that users can log in using their 42 intranet accounts. You'll need to register your app in the 42 intranet's developer portal to get your OAuth credentials (client ID and client secret). You can use libraries like Passport.js to manage OAuth authentication in NestJS.

Other tasks such as avatar upload, two-factor authentication, friends feature, and user stats will require further integration and development. Make sure to store sensitive data securely and encrypt it if necessary.

4. Chat
Creating a chat system can be complex. You'll need to create a system that supports direct messages, chat rooms, and various permissions. You might find WebSocket useful for real-time communication. NestJS has built-in support for WebSocket.

5. Game
The Pong game will be the most challenging part of this project. You can use HTML5 canvas or a JavaScript game library to create the game. Make sure it works well on all screens and handles network issues gracefully.

Remember, each of these points can be quite complex and would typically involve multiple steps to implement. Before starting with the actual coding, you may find it helpful to create a design or plan of how each component will work and how they will interact with each other. Start coding only after you have a clear understanding of how everything fits together.
