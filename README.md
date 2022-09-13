# <img src="images/DS_Weiss_Book.jpg" align="right"> Code Examples for Data Structures

Textbook: Data Structures and Algorithm Analysis in C++ (Fourth Edition), by Mark Allen Weiss

Source Code by Mark Allen Weiss can be found [here.](https://users.cs.fiu.edu/~weiss/dsaa_c++4/code/)

Course material and assignments for CS 2341 can be found on [Canvas](https://www.smu.edu/OIT/Services/Canvas/).


## Required Tools

* Install [Visual Studio Code](https://code.visualstudio.com/) (VS Code)
* On **Windows** you will need to [install WSL](https://code.visualstudio.com/docs/cpp/config-wsl) and use the CS Code Remote WSL ([here is a video](https://www.youtube.com/watch?v=NY5izJWXi0U)). You also should install `cmake` and `valgrind` in the WSL shell using `sudo apt get install`. You will need to open folders by clicking on the green `><` at the bottom left corner of VS Code and select open folder in WSL.
* On **MacOS** you need to set up the [shell command](https://code.visualstudio.com/docs/setup/mac). This includes installing Xcode (for compilers) and [cMake](https://cmake.org/install/). 
* Install [git](https://git-scm.com/) and [VS Code integration](https://code.visualstudio.com/docs/editor/versioncontrol).
* Install [VS Code extensions for C++ and CMake](https://code.visualstudio.com/docs/languages/cpp). The extensions are: `C/C++`, `C/C++ Extension Pack`, `CMake Tools`. Make sure that you install the extensions **after** you have the software above installed or it might not find it. 

## Using VS Code With a Remote Linux Server

If you have access to a Linux host server with all development tools installed (see [genuse servers](https://www.smu.edu/OIT/Services/genuse) for SMU students) then you can install only VS Code and the VS Code extension `Remote - SSH`. You can then connect to the host by clicking on the green `><` at the bottom left corner of VS Code ([details](https://code.visualstudio.com/docs/remote/ssh)).

## Content

* [HOWTO Compile Programs With VS Code and CMake](Chapter1_Programming/HOWTO_compile_programs_with_CMake.md)
* [HOWTO Debug and Test](Chapter1_Programming/HOWTO_debug_and_test.md)

| Book Chapter |  Notes and Code |
| :-----: |  :--- |
| 1 | [Programming](Chapter1_Programming)  |
| 2 |[Algorithm Analysis](Chapter2_Algorithm_Analysis) |
| 3 | [Lists, Stacks, and Queues](Chapter3_Lists_etc) |
| 4 | [Trees](Chapter4_Trees) |
| 5 | [Hashing](Chapter5_Hashing) |
| 6 | [Heaps](Chapter6_Heaps) |
| 9 | [Graphs](Chapter9_Graphs) |

## License

<img src="https://licensebuttons.net/l/by-sa/3.0/88x31.png" alt="CC BY-SA 4.0" align="left">

All code and documents in this repository are provided under [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0) License.](https://creativecommons.org/licenses/by-sa/4.0/)
