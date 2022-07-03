# Simple-Cpp-Setup

Welcome to this simple C++ template project!<br/>
It contains everything you need to get started with programming in C++.

If your machine is already setup and can compile C++ code, you can jump to [Creating a repository](#creating-a-repository).

TODO TOC

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

Open the folder in Visual Studio Code

![](./docs/run.png)

## If you use the Dev Container

If you install [ms-vscode-remote.remote-containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) and [Docker](https://www.docker.com/products/docker-desktop), you will be able to run your code inside a Linux container (kind of like a virtual machine, but faster). Also, you will get static analyzers, code formatters and useful extensions installed out of the box! It is a great option to get started with C++ quickly.

(Unfortunately, if you want to do GUI applications they don't work well from within a container and you might have to do a proper setup on your own desktop instead. But for simple command-line applications this works amazingly well!)

NB: the container might take a while to build the first time.

## If you don't use the Dev Container

### Compiling

You need to install [CMake](https://cmake.org/download/).

To use CMake I recommend this VS Code extension : [ms-vscode.cmake-tools](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cmake-tools). You will need to setup the extension with a compiler. Here is [the tutorial](https://code.visualstudio.com/docs/cpp/cmake-linux). It is based on Linux but at the bottom of the page you will find the explanations to adapt it for [Windows](https://code.visualstudio.com/docs/cpp/config-msvc) and [Mac](https://code.visualstudio.com/docs/cpp/config-clang-mac).

Alternatively you can just create a *build* folder at the root of this project, open a terminal and run `cmake ..`; chances are it will detect what compiler you have installed and generate the appropriate Makefile / Visual Studio solution / Xcode project.

### Auto-formatting

[Check this out](https://julesfouchy.github.io//Learn--Clean-Code-With-Cpp/lessons/formatting-tool) to learn why you would want to use a code formatter and how to do it.

### Static analysis

[Check this out](https://julesfouchy.github.io/Learn--Clean-Code-With-Cpp/lessons/static-analysis-and-sanitizers) to learn why you would want to use static analysis and how to do it.
