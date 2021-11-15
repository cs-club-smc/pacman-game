# Contributing

Haiii ^w^, welcome to `pacman-game`!

You can jump to 'Getting Started' if you are ready for running this project on your computer; if not see 'Learning' if you're not really sure where to start

## Learning

If you're not sure where to start, I would recommend watching either the first three videos of the [Git and GitHub for Poets](https://www.youtube.com/watch?v=BCQHnlnPusY&list=PLozRqGzj97d02YjR5JVqDwN2K0cAiT7VK) series by The Coding Train, or this [How to Contribute to an Open Source Project on GitHub](https://egghead.io/lessons/javascript-introduction-to-github) mini-course by Kent C. Dodds. The former is longer and more conceptual while the latter is shorter and focuses more on real-world usage. There is also this [100 Second video](https://www.youtube.com/watch?v=8lGpZkjnkt4) by Fireship

Once you are more familiar with Git, you are now ready to make a PR. I found  short video to be helpful in showing the whole pull request workflow, but you may need to use Google if you are not using Git through the command line, or run into errors

## Getting Started

Before you perform the following steps, you'll want to _Fork_ this repository, then _Clone_ it.

### 1. Installing NodeJS and Yarn

We are using [NodeJS](https://nodejs.org/en) as a backend server. This lets us write JavaScript that serves files, and responds to requests from browsers.

The most popular way to install NodeJS is through the [installer on the official website](https://nodejs.org). Follow the installation instructions for your operating system. As for versions, you can choose either the latest LTS (`16.13.0` at the time of writing), or the latest stable release (`17.1.0` at the time of writing)

To optionally check if NodeJS has been properly installed, you can open a terminal and see if you get the following output:

```sh
$ node --version
v17.1.0
```

Note that your version of NodeJS may be different than mine

Once you have done this, you'll want to install a package manager for NodeJS. Package managers allow us to easily use someone elses code in our project. The package manager that comes with NodeJS is called `npm`, but we'll be using `yarn` for this project. These days, there isn't a huge difference between the two, but Yarn

- Is slightly faster
- Has a much nicer / more readable output
- Does not print irrelevant errors / warnings

To install Yarn, run the following

```sh
npm install -g yarn
```

You have just installed a package manager... with another package manager 😎

### 2. Cloning this repository

Once you have NodeJS and Yarn installed, you are ready to clone this repository. Use your favorite Git client! For those that wish to use the terminal, enter the following

```sh
git clone https://github.com/cs-club-smc/pacman-game
cd pacman-game
```

### 3. VSCode amenities

I would _highly_ recommend installing the [EditorConfig](https://editorconfig.org) and [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) VSCode [extensions](https://code.visualstudio.com/docs/editor/extension-marketplace). Both EditorConfig and Prettier are used so all contributors add code with the same coding style. For example, the [./.editorconfig](./.editorconfig) and [./.prettierrc.json](./.prettierrc.json) files tell the VSCode extensions not to add `;` to the end of lines, and to write strings like `'my-string'` instead of `"my-string"`, among other things

VSCode is configured to automatically format the code with Prettier when you save a file. Under the hood, VSCode reads [`./vscode/settings.json`](./.vscode/settings.json), and tells the Prettier extension to format the file

### 4. Running the code

There are two main ways to run the code

#### 4.1 VSCode Tasks

The first method is within VSCode. Open the [Command Palette](https://code.visualstudio.com/docs/getstarted/userinterface#_command-palette) (`Ctrl+Shift+P` or `F1`), and choose `Tasks: Run Task`. Then choose `Start NodeJS Server`. A terminal within VSCode should pop up, with the result of running the app

Under the hood, VSCode reads [./.vscode/tasks.json](./.vscode/tasks.json), and executes the command `yarn run start`

#### 4.2 Terminal

The second method is using the Terminal. Navigate to this project directory, and run

```sh
yarn run start
```

Undner the hood, `yarn` will read [./package.json](./package.json), and run the `"start"` script, or `node src/index.js`

### 5. Finished!

And now you are done!

<img alt='Red Panda celebrating' src='./assets/red-panda-celebrate.png' width='200'>

Art by [Pulex](https://www.pulexart.com)

From here, you are ready to make a PR! Feel free to make a PR to this repostory, such as adding printed lines in [./src/index.js](./src/index.js) or fixing typos, especially if you've never made a PR before

