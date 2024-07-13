
# Bellefull Integration Documentation

## Overview

The Belleful Food Ordering App API provides a seamless experience for customers to order their favorite meals. This API offers endpoints for managing user accounts, browsing available meals, placing orders, and tracking delivery status.


#### Key Features:
-   **User Registration**: Endpoints for creating new user accounts.
-   **Profile Setup**: Endpoints for setting up user profiles and preferences.
-   **Verification**: Endpoints for verifying user information and credentials.

#### Differentiating Users:

A header parameter called `x-request-source` is used to differentiate between vendors, admins, and customers. This parameter should be included in the request headers and set to the appropriate value for the user type (e.g., `vendor`, `admin`, `customer`).

## API Schema

The Belleful Food Ordering App API schema outlines the structure and types of data used in our API requests and responses. Detailed schema definitions for each endpoint can be found in the `API_REFERENCE.md` file. Additionally, our API is documented using Postman Documenter, which can be accessed [here](https://documenter.getpostman.com/view/15091597/2sA3e5eTsG#intro).

## Versioning
This project is versioned to ensure backward compatibility and easy maintenance. The current version is v1.


## Database and Relationships

The Belleful Food Ordering App database schema defines the structure and relationships between various entities. Here are some of the key tables:

- **Users**
  - Stores information about users, including customers, vendors, and admins.
- **Vendors**
  - Contains details about each vendor, including name, address, and description.
- **Meals**
  - Lists all available meals with their ingredients, prices, and images.
- **Orders**
  - Tracks customer orders, including meal details, quantities, and order status.
- **Cart**
  - Stores the current contents of a customer's cart.

Detailed relationships between these tables can be found [here](https://erd.dbdesigner.net/designer/schema/1720905377-bellefu).

# Dependencies for Belleful Food Ordering App

## Backend Dependencies
- **express**: Web framework for Node.js
- **pg**: PostgreSQL client for Node.js
- **typeorm**: ORM for TypeScript and JavaScript (ES7, ES6, ES5)
- **sequelize**: Promise-based Node.js ORM for Postgres, MySQL, MariaDB, SQLite, and Microsoft SQL Server
- **dotenv**: Loads environment variables from a `.env` file into `process.env`
- **bcrypt**: Library to hash passwords
- **jsonwebtoken**: For JSON Web Token authentication
- **cors**: Middleware to enable CORS (Cross-Origin Resource Sharing)
- **body-parser**: Middleware to parse incoming request bodies
- **morgan**: HTTP request logger middleware for Node.js
- **express-validator**: Express middleware for validation

## Testing Dependencies
- **jest**: JavaScript Testing Framework
- **supertest**: HTTP assertions made easy via superagent
- **chai**: BDD / TDD assertion library for node and the browser
- **mocha**: JavaScript test framework for Node.js

## Development Dependencies
- **nodemon**: Automatically restart the node application when file changes are detected
- **typescript**: TypeScript language support
- **ts-node**: TypeScript execution environment for Node.js
- **tslint**: Linter for TypeScript

## Documentation Dependencies
- **swagger-jsdoc**: JSDoc to Swagger API documentation generator
- **swagger-ui-express**: Swagger UI for Express.js
- **postman-doc**: Postman documentation tool for API standards, contracts and schema

## Folder Structure

```
|--- dist
|    |--- index.html
|--- src
|    |--- controllers
|    |--- database
|    |--- interfaces
|    |--- middlewares
|    |--- routes
|    |--- services
|    |--- utils
|    |--- server.ts
|--- .env
|--- app.ts
|--- .gitignore
|--- package.json
|--- README.md
|--- API_REFERENCE.md
|--- CONTRIBUTORS_GUIDE.md
|--- CODE_OF_CONDUCT.md
|--- tsconfig.json
```

```

## Getting Started

Before you begin, ensure you have the following installed on your machine:

- [Node.js](https://nodejs.org/) (v14 or later)
- [npm](https://www.npmjs.com/) (Node Package Manager, included with Node.js)
- [Git](https://git-scm.com/)

## Contribution Guide

## Getting Started

#### If you don't have git on your machine, [install it](https://docs.github.com/en/get-started/quickstart/set-up-git).

## Fork this repository

Fork this repository by clicking on the fork button on the top of this page.
This will create a copy of this repository in your account.

## Clone the repository

<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/clone.png" alt="clone this repository" />

Now clone the forked repository to your machine. Go to your GitHub account, open the forked repository, click on the code button and then click the _copy to clipboard_ icon.

Open a terminal and run the following git command:

```bash
git clone "url you just copied"
```

where "url you just copied" (without the quotation marks) is the url to this repository (your fork of this project). See the previous steps to obtain the url.

<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/copy-to-clipboard.png" alt="copy URL to clipboard" />

For example:

```bash
git clone git@github.com:this-is-you/first-contributions.git
```

where `this-is-you` is your GitHub username. Here you're copying the contents of the first-contributions repository on GitHub to your computer.

## Create a branch

Change to the repository directory on your computer (if you are not already there):

```bash
cd first-contributions
```

Now create a branch using the `git switch` command:

```bash
git switch -c your-new-branch-name
```

For example:

```bash
git switch -c add-alonzo-church
```

### Make Changes

Make your changes to the codebase. Ensure your code follows the project's coding standards and guidelines.

### Run Tests

Run the existing tests to ensure your changes do not break anything. If you added new functionality, write corresponding tests.

```sh
npm run test
```

## commit those changes

Now open `Contributors.md` file in a text editor, add your name to it. Don't add it at the beginning or end of the file. Put it anywhere in between. Now, save the file.

<img align="right" width="450" src="https://firstcontributions.github.io/assets/Readme/git-status.png" alt="git status" />

If you go to the project directory and execute the command `git status`, you'll see there are changes.

Add those changes to the branch you just created using the `git add` command:

## Push changes to GitHub

Push your changes using the command `git push`:

```bash
git push -u origin your-branch-name
```

replacing `your-branch-name` with the name of the branch you created earlier.

<details>
<summary> <strong>If you get any errors while pushing, click here:</strong> </summary>

- ### Authentication Error
     <pre>remote: Support for password authentication was removed on August 13, 2021. Please use a personal access token instead.
  remote: Please see https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/ for more information.
  fatal: Authentication failed for 'https://github.com/<your-username>/first-contributions.git/'</pre>
  Go to [GitHub's tutorial](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) on generating and configuring an SSH key to your account.

</details>

## Submit your changes for review into Staging

If you go to your repository on GitHub, you'll see a `Compare & pull request` button. Click on that button.

<img style="float: right;" src="https://firstcontributions.github.io/assets/Readme/compare-and-pull.png" alt="create a pull request" />

Now submit the pull request.

<img style="float: right;" src="https://firstcontributions.github.io/assets/Readme/submit-pull-request.png" alt="submit pull request" />

Soon your changes will be merged into the staging branch of this project. You will get a notification email once the changes have been merged.

## Setup Instructions

### 1. Clone the Repository

First, clone the repository to your local machine using Git.

```sh
git clone https://github.com/your-username/[app-name].git
cd [app-name]
```

### 2. Install Dependencies

Navigate to the project directory and install the required dependencies.

```sh
npm install
```

### 3. Configure Environment Variables

Create a `.env` file in the root directory of the project and add your environment-specific variables. You can use the provided `.env.example` file as a reference.

```sh
cp .env.example .env
```

Edit the `.env` file to match your environment configuration.

### 4. Compile TypeScript

Compile the TypeScript code to JavaScript.

```sh
npm run build
```

### 5. Run the Development Server

Start the development server with the following command. This will also watch for any changes in your code and automatically restart the server.

```sh
npm run start:dev
```

### 6. Run the Production Server

To run the application in a production environment, use the following command:

```sh
npm run start
```

### 7. Verify the Setup

Open your browser and navigate to `http://localhost:3000/api/v1/` to verify that the application is running correctly.

## Scripts

Here are some useful npm scripts that you can use during development and production:

- `npm run build`: Compiles the TypeScript code to JavaScript.
- `npm run start:dev`: Starts the development server with live reloading.
- `npm run start`: Starts the production server.
- `npm run test`: Runs the test suite (if available).
- `npm run lint`: Runs the linter to check for code style issues.

## Additional Resources

- [Node.js Documentation](https://nodejs.org/en/docs/)
- [TypeScript Documentation](https://www.typescriptlang.org/docs/)
- [Express Documentation](https://expressjs.com/)

By following these steps, you should have your Node.js and TypeScript application up and running. If you encounter any issues, please refer to the documentation of the respective tools or seek help from the community.

