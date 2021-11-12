# Contributing

🚧 Warning! This page isn't finished 🚧

## Getting Started

Haiii ^w^, welcome to `smc-pacman`! To get the project running on your local development machine, follow these steps

### 1. Installing NodeJS

We are using [NodeJS](https://nodejs.org/en) as a backend server. This lets us write JavaScript to serve files, and respond to requests from browsers.

The most popular way to install NodeJS is through the [installer on the official website](https://nodejs.org). Follow the installation instructions for your operating system. As for versions, you can choose either the latest LTS (`16.13.0` at the time of writing), or the latest stable release (`17.1.0`)

To optionally check if NodeJS has been properly installed, you can open a terminal (Term.app on MacOS or Powershell on Windows) and see if you get the following output:

```sh
node --version
v17.1.0
```

Note that your version of NodeJS may be different than mine

Once you have done this, you'll want to install a package manager for NodeJS. Package managers allow us to easily use someone elses code in our project. The package manager that comes with NodeJS is called `npm`, but we'll be using `yarn` for this project. These days, there isn't a huge difference between the two, but Yarn

- Is slightly faster
- Has a much nicer / more readable output
- Does not print irrelevant errors / warnings

To install Yarn, run the following in a terminal

```sh
npm --global install yarn
```

### 2. Cloning this repository

Once you have NodeJS and Yarn installed, you are ready to clone this repository. Use your favorite Git client, or run the following in the terminal

```sh
https://github.com/cs-club-smc/pacman-game
cd pacman-game
```

### 3. VSCode amenities

I would _highly_ recommend downloading [EditorConfig](https://editorconfig.org), [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode), and [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint). Both EditorConfig and Prettier are used so all contributors add code with the same coding style. The [.editorconfig](./.editorconfig) and [.prettierrc.json](./.prettierrc.json) tell the plugin that we do not want to add semicolons to the end of lines, and to write strings like `'my-string'` instead of `"my-string"`.

### 4. Running the code

There are two main ways to run the code

The first method is within VSCode. Open the [Command Palette](https://code.visualstudio.com/docs/getstarted/userinterface#_command-palette) (`Ctrl+Shift+P`), and choose `Tasks: Run Task`. Then choose `Start NodeJS Server`. A terminal within VSCode should pop up, with the contents of

The second method is using the Terminal. Navigate to this project directory, and run

```sh
yarn run start
```

Undner the hood, `yarn` will run the `"start"` script in `package.json`
