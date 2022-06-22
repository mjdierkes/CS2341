# <img src="images/DS_Weiss_Book.jpg" align="right"> CS 2342 Code Examples

Textbook: Data Structures and Algorithm Analysis in C++ (Fourth Edition), by Mark Allen Weiss

Source Code by Mark Allen Weiss can be found here:
https://users.cs.fiu.edu/~weiss/dsaa_c++4/code/

## Tool Requirements

* Install Visual Studio Code: https://code.visualstudio.com/
* On Windows you will need to install WSL: https://code.visualstudio.com/docs/cpp/config-wsl
* Install Extensions for C++ and CMake: https://code.visualstudio.com/docs/languages/cpp
* Install git: https://git-scm.com/


## How to compile and run the examples in this repository

1. Clone the repository.
2. Go in your shell to an example and run `code .` Each folder can be seen as a project.
3. Click `Build` in the status bar. `CMake` creates a `build` directory with a `Makefile` which is used to 
   build the project.
4. Click the run button in the status bar.

*Note:* If you move a project directory, then you have to clean the project by removing the build folder.

## How to set up a new program

1. Make a directory.
2. Create at least a `main.cpp` file.
3. Configure CMake by going in the menu to `Help>Show All Commands` and type `CMake:Configure`. Choose a compiler 
   (C++11) and that you want to create an executable. This creates a file called `CMakeLists.txt`.
4. Additonal `.cpp` files can be added in the `add_executable()` instruction in `CMakeLists.txt`.

You are now ready to build and execute the program.

*Note:* Steps 2 and 3 can be done using `CMake:Quickstart` which will create a Hello World! program.

## How to debug

### In VS Code:

1. Set a breakpoint next to a line of code.
2. Click the debug symbol in the status bar which starts a frontend for `gdb`.
3. Use the navigation pannel and inspect and watch variables.

### Command line debuging with `gdb`.

1. Find the compiled executable (in VS Code it is in the build directory)
2. Start `gdb executable`.
3. set a break point with `b` and use `run`. See the [GDB QUICK REFERENCE](https://users.ece.utexas.edu/~adnan/gdb-refcard.pdf) for available commands.

### Valgrind to detect memory leaks

*Note:* `valgrind` is not available on Windows and the VS Code integration is not great. On Ubuntu it can be installed with
`sudo apt install valgrind`.

1. Find the compiled executable (in VS Code it is in the build directory)
2. Run `valgrind --leak-check=full ./executable` and look for lost bytes.

## How to run automatic tests

CMake comes with CTest. CTest is not a testing framework, but a tool to automate runing tests. We also need a testing framework. 
We will use a simple header-based framework called 
[Catch2](https://github.com/catchorg/Catch2) which can be
easily [integrated with CMake/CTest](https://github.com/catchorg/Catch2/blob/devel/docs/cmake-integration.md).

Steps:

1. Download the the [`catch.hpp`](https://github.com/catchorg/Catch2/releases/download/v2.13.9/catch.hpp) header file and place it into your project. 
2. You need a test file like `test.cpp` in the [testing example](Chapter1_Overview/testing/) to define test cases and required outputs. There are [more assertions](https://github.com/catchorg/Catch2/blob/v2.x/docs/assertions.md) available.
3. Add a testing section to `CMakeLists.txt`.
4. Building and testing is avaialble in the status bar.

Testing using GitHub Actions:

1. At the repository on the Github page, click on Actions and find `CMake based projects`.
2. Click configure and 


