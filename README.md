# Simple-Cpp-Setup

🎉 Welcome to this simple C++ template project!<br/>
👩‍💻 It contains everything you need to get started with programming in C++.

If your machine is already setup and can compile C++ code, you can jump to [Creating a repository](#creating-a-repository).

- [Installing the tools](#installing-the-tools)
    * [IDE](#ide)
    * [Compiler](#compiler)
    * [CMake](#cmake)
    * [LLVM (Optional, but strongly recommended)](#llvm--optional--but-strongly-recommended-)
- [Creating a repository](#creating-a-repository)
- [Downloading the code on your computer](#downloading-the-code-on-your-computer)
- [Running the code](#running-the-code)

## Installing the tools

### IDE

We recommend using Visual Studio Code as your IDE (Integrated Development Environment). [You can download it from here.](https://code.visualstudio.com/)

Then you will need the C++ extensions: [ms-vscode.cpptools-extension-pack](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools-extension-pack).

Optionally you can also install [ms-vsliveshare.vsliveshare](https://marketplace.visualstudio.com/items?itemName=ms-vsliveshare.vsliveshare): It will allow you to work remotely with your teammates in one single editor, just like a GoogleDoc. It is amazing to work together on projects!

### Compiler

Follow the instructions from https://julesfouchy.github.io/Learn--Clean-Code-With-Cpp/lessons/install-a-compiler/.

### CMake

Install CMake from https://cmake.org/download/ (or from your favorite package manager).

### LLVM (Optional, but strongly recommended)

This will install tools that will format and lint your code (a.k.a. give you advice and show you where potential bugs are).

Install it from https://github.com/llvm/llvm-project/releases/latest. Choose the right one for your platform (e.g. the one finishing with *-win64.exe* if you are on Windows). On Linux, you can also install it from the command line.

Then, setup the extensions in VS Code by following the lessons on [formatters](https://julesfouchy.github.io/Learn--Clean-Code-With-Cpp/lessons/formatting-tool/) and [static analysers](https://julesfouchy.github.io/Learn--Clean-Code-With-Cpp/lessons/static-analysers/).


## Creating a repository

Make a copy of this repository on your own Github account by using `Use this template`.
![](./docs/use-this-template.png)

> **NB:** If you are not using GitHub but GitLab or anything else, just download the code (using the `Code` dropdown next to `Use this template`), then create a repo on your own, and commit the downloaded code to that repo. `Use this template` is just a convenient shortcut, it is not mandatory.

## Downloading the code on your computer

Open a terminal in the folder where you want to download this repository, and run
```bash
git clone [url to your repository]
```

For example in my case this would be:
```bash
git clone https://github.com/JulesFouchy/Simple-Cpp-Setup
```

## Running the code

Open the folder in Visual Studio Code. You should then see something like

![](./docs/open-project.png)

In the bottom section, click the `Run` button:

![](./docs/run.png)

The first time, it will ask you which compiler you want to use. If you installed everything correctly, you should have at least one in the list. Select any of them.

Your program should then compile, run, and output "Hello World!":

![](./docs/hello-world.png)

