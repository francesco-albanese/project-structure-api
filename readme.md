<div id="top"></div>

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

<br />
<div align="center">
  <h3 align="center">Project Structure API</h3>

  <p align="center">
    Complete project template for building RESTful API with Typescript
    <br />
    <br />
    <a href="https://github.com/arifintahu/project-structure-api/issues">Report Bug</a>
    ·
    <a href="https://github.com/arifintahu/project-structure-api/issues">Request Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contributing">Contributing</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->

## About The Project

Building project with standardized structure could save much our time. We could focus on business process without considering too much on project structure. On the other hand, a good project structure should be clean, nice refactored, and easy to maintain.

Here's why:

- Your time should be focused on creating something amazing. A project that solves a problem and helps others.
- You shouldn't be doing the same tasks over and over like structuring project
- You should implement dry principles to the rest of your life

Of course, no one template will serve all projects since your needs may be different. So I'll be adding more in the near future. You may also suggest changes by forking this repo and creating a pull request or opening an issue. Thanks to all the people have contributed to expanding this project template!

<p align="right">(<a href="#top">back to top</a>)</p>

### Built With

This project structure is built using

- [Express.js](https://expressjs.com/)
- [Sequelize](https://sequelize.org/)
- [Swagger](https://swagger.io/)
- [Typescript](https://www.typescriptlang.org/)
- [JsonWebToken](https://www.npmjs.com/package/jsonwebtoken)
- [Postgresql](https://www.postgresql.org/)
- [Mocha](https://mochajs.org/)
- [Supertest](https://www.npmjs.com/package/supertest)

<p align="right">(<a href="#top">back to top</a>)</p>

### Features

- Everything is modular and unit testable
- Typescript everything
- Express API with dependency injected routes, controllers, repositories, middleware, and services
- Centralized configuration loading and validation

### Folder Structure

```
├── .husky/                     # Pre-commit config for lint staged
├── src/                        # All application source
├──── @types/                   # Type definition
|
├──── api/
├────── controllers/            # Define all controllers
├────── helpers/                # Define all helpers
├────── lib/
├──────── logger.ts             # Define logger
├────── middlewares/
├──────── authorization.ts      # Define authorization using JWT
├──────── morgan.ts             # Define morgan
├────── models/                 # Define all schema models
├────── repositories/           # Define all repositories
├────── routes/
├──────── v1/                   # Define all v1 routes
├────── services/               # Define all services
├────── validations/            # Define all controller validations
|
├──── config/
├────── swagger/                # Define swagger configuration
├────── database.ts             # Define postgres database connection
├────── express.ts              # Define express configuration
|
├──── constants/                # Define all constants
├──── server.ts                 # Create express config
├──── index.ts                  # ENTRYPOINT - Start server
|
├── test/                       # End-to-end test
|
└── Lots of random build-related files
```

<!-- GETTING STARTED -->

## Getting Started

To start project, just clone this repo or [Use this template](https://github.com/arifintahu/project-structure-api/generate)

### Prerequisites

Before installation, make sure you have the following prerequisites

- NPM
  ```sh
  npm install npm@latest -g
  ```
- Postgresql server

### Installation

1. Clone the repo or simply select [use this template](https://github.com/arifintahu/project-structure-api/generate)
   ```sh
   git clone https://github.com/arifintahu/project-structure-api.git
   ```
2. Install NPM packages
   ```sh
   npm install
   ```
3. Create .env file in main directory
   ```sh
   touch .env
   ```
4. Write the following example environment
   ```sh
   NODE_ENV=development
   PORT=3001
   DB_HOST=localhost
   DB_NAME=test
   DB_USER=postgres
   DB_PASS=postgres
   DB_PORT=5432
   DB_LOG=true
   ```
5. Test and build the project
   ```sh
   npm run build
   ```
6. Run the server
   ```sh
   npm run start
   ```

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTRIBUTING -->

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/feature-name`)
3. Commit your Changes (`git commit -m 'Add some feature-name'`)
4. Push to the Branch (`git push origin feature/feature-name`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[contributors-shield]: https://img.shields.io/github/contributors/arifintahu/project-structure-api.svg?style=for-the-badge
[contributors-url]: https://github.com/arifintahu/project-structure-api/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/arifintahu/project-structure-api.svg?style=for-the-badge
[forks-url]: https://github.com/arifintahu/project-structure-api/network/members
[stars-shield]: https://img.shields.io/github/stars/arifintahu/project-structure-api.svg?style=for-the-badge
[stars-url]: https://github.com/arifintahu/project-structure-api/stargazers
[issues-shield]: https://img.shields.io/github/issues/arifintahu/project-structure-api.svg?style=for-the-badge
[issues-url]: https://github.com/arifintahu/project-structure-api/issues
