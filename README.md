<div align="center" >
  <p style="font-size:30px;">Bus Management System</p>
  <p>Effortlessly Plan, Book, and Manage Your Bus Trips</p>
  <br />
  <a href="https://github.com/JulianaSau/bms_web/issues/new?assignees=&labels=bug&template=01_BUG_REPORT.md&title=bug%3A+">Report a Bug</a>
  ·
  <a href="https://github.com/JulianaSau/bms_web/issues/new?assignees=&labels=enhancement&template=02_FEATURE_REQUEST.md&title=feat%3A+">Request a Feature</a>
</div>
<br/>

![image](https://github.com/JulianaSau/bms_web/assets/49183775/fe6e5191-6138-4a30-9914-05e22c53855f)

<br/>
<div align="center">

[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
[![license](https://img.shields.io/static/v1?label=licence&message=MIT&color=yellowgreen&style=flat-square)](LICENSE)
[![made with heart by bms_web](https://img.shields.io/badge/made%20with%20%E2%99%A5%20by-bms_web-ff1414.svg?style=flat-square)](https://github.com/JulianaSau/bms_web/)
[![Test and Build App](https://github.com/Kiotapay-org/financial_module/actions/workflows/test.yml/badge.svg?branch=develop)](https://github.com/JulianaSau/bms_web/actions/workflows/test.yml)
</div>

<details open="open">
<summary>Table of Contents</summary>

- [Introduction](#about)
  - [Built With](#built-with)
- [Installation](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Usage](#usage)
    - [Variables reference](#variables-reference)
- [License](#license)

</details>

---

## About

This is an application meant to ease bus booking created by [Juliana Sau]([https://](https://www.linkedin.com/in/juliana-sau/)). It is built using ReactJs

- [Deployed Site](https://bookings.rentallscale.com)
- [Find out what inspired this app]()

## Features

- Next.js 13 App Directory
- Radix UI Primitives
- Tailwind CSS
- Icons from [Lucide](https://lucide.dev)
- Dark mode with `next-themes`
- Tailwind CSS class sorting, merging and linting.

## What's inside?

This repo includes the following:

### Folder structure

<details closed>

```
.
├── app
│   ├── layout.tsx
│   └── page.tsx
├── components
│   ├── ui
│   │   ├── modal.tsx
│   │   ├── button.tsx
│   │   ├── dropdown-menu.tsx
│   │   └── ...
│   ├── main-nav.tsx
│   ├── page-header.tsx
│   └── ...
├── config
│   └── site.ts
├── public
│   ├──  manifest.json
│   └── ...
├── lib
│   ├── utils.ts
│   └── ...
├── styles
│   └── globals.css
├── types
│   ├── user.ts
│   └── ...
├── next.config.js
├── package.json
├── postcss.config.js
├── tailwind.config.js
└── tsconfig.json
└── ...
```

</details>

- UI components in the `components/ui` folder.
- The rest of the components such as <PageHeader /> and <MainNav /> are placed in the `components` folder.
- The` lib` folder contains all the utility functions. There is a `utils.ts` where the `cn` helper is defined.
- The `styles` folder contains the global CSS.

Each package and app is 100% [TypeScript](https://www.typescriptlang.org/).

### Utilities

This repo has some additional tools already setup for you:

- [TypeScript](https://www.typescriptlang.org/) for static type checking
- [ESLint](https://eslint.org/) for code linting
- [Jest](https://jestjs.io) test runner for all things JavaScript
- [Prettier](https://prettier.io) for code formatting

### Built With

#### Frontend Technologies

| Technology    | Version | Use                                    |
| ------------- | ------- | -------------------------------------- |
| `TypeScript`  | ...     | Programming Language(typed Javascript) |
| `NextJs`      | v13.4.8 | Frontend Framework                     |
| `Shadcn UI`   | v1.8.6  | UI library                             |
| `RTK Toolkit` | v1.8.0  | State management                       |
| `Eslint`      | v1.8.0  | Code Linter                            |
| `Prettier`    | v1.8.0  | Code Formatter                         |

## Getting Started

### Environment Setup

- Linting has been set up for staged commits in the repository.
- We're using `eslint` for js linting, and `prettier` for code formating.
- Please make it a point to install `eslint` and `prettier` plugins on vscode to aid in your coding process.
- Your code has to be properly formatted and have the correct syntax for you to be able to commit your changes.
- Make sure you attend to all warnings and errors before you commit your code

#### Clone the repo

```bash
git clone https://github.com/Kiotapay-org/financial_module.git
```

#### Variables reference

- Ensure you create a `.env` file using the `.env.example` as a guide and request for the required values for the variables

Please note that entered values are case-sensitive.
Default values are provided as an example to help you figure out what should be entered.

> On manual setup, you need to replace only values written in **uppercase**.

| Name                            | Default value | Description                              |
| ------------------------------- | ------------- | ---------------------------------------- |
| NEXT_PUBLIC_API_BASE_URL        | "tbd"         | Backend API base url                     |
| NEXT_PUBLIC_PMS_URL             | "tbd"         | Backend API key                          |
| NEXT_PUBLIC_GOOGLE_MAPS_API_KEY | "tbd"         | Google Maps api key to access places api |
| NEXTAUTH_SECRET                 | "tbd"         | Related to next auth                     |
| NEXTAUTH_URL                    | "tbd"         | Related to next auth                     |
| NODE_ENV                        | "tbd"         | Current node environment                 |

#### Install all dependencies

```bash
yarn install
```

#### Run the development server:

```bash
yarn dev
```

- Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.
- You're all set. Happy coding😁

### Running with Docker

This repo is configured to be built with Docker, and Docker compose. To build all apps in this repo:

```
# Build
docker-compose -f docker-compose.yml build

# Start prod in detached mode
docker-compose -f docker-compose.yml up -d
```

Open http://localhost:3000.

To shutdown all running containers:

```
# Stop all running containers
docker kill $(docker ps -q) && docker rm $(docker ps -a -q)
```

### Building the application

- To build the whole application

```bash
yarn build
```

## Contributing

Please check on the gitub project to see assigned tasks to make conrtibutions to the repo

### Contribution Guidelines

1. Clone the repo `git clone https://github.com/JulianaSau/bms_web`.
2. Open your terminal & set the origin branch: `git remote add origin https://github.com/JulianaSau/bms_web.git`
3. Pull origin `git pull origin dev`
4. Create a new branch for the task you were assigned to, eg `(feat/bug/fix/chore)/issue-title` : `git checkout -b feat/routes`
5. After making changes, do `git add .`
6. Commit your changes with a descriptive commit message : `git commit -m "your commit message"`.
7. To make sure there are no conflicts, run `git pull origin dev`.
8. Push changes to your new branch, run `git push -u origin feat/routes`.
9. Create a pull request to the `dev` branch not `main`.
10. Ensure to describe your pull request.
11. If you've added code that should be tested, add some test examples.

### Merging

- Pipeline is `feature branch` -> `dev` -> `staging` -> `main`

### _Commit CheatSheet_

| Type     |                          | Description                                                                                                 |
| -------- | ------------------------ | ----------------------------------------------------------------------------------------------------------- |
| feat     | Features                 | A new feature                                                                                               |
| fix      | Bug Fixes                | A bug fix                                                                                                   |
| docs     | Documentation            | Documentation only changes                                                                                  |
| style    | Styles                   | Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)      |
| refactor | Code Refactoring         | A code change that neither fixes a bug nor adds a feature                                                   |
| perf     | Performance Improvements | A code change that improves performance                                                                     |
| test     | Tests                    | Adding missing tests or correcting existing tests                                                           |
| build    | Builds                   | Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)         |
| ci       | Continuous Integrations  | Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs) |
| chore    | Chores                   | Other changes that don't modify , frontend or test files                                                    |
| revert   | Reverts                  | Reverts a previous commit                                                                                   |

> _Sample Commit Messages_

- `chore: Updated README file` := `chore` is used because the commit didn't make any changes to the , frontend or test folders in any way.
- `feat: Added plugin info endpoints` := `feat` is used here because the feature was non-existent before the commit.

## Support

Reach out to the maintainer at one of the following places:

- [Twitter](https://x.com/juliana_sau)
- The email which is located [in GitHub profile](https://github.com/JulianaSau)

## License
This project is licensed under the MIT License - see the [LICENSE](https://github.com/JulianaSau/bms_web/) file for details.
