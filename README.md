# OS-simulation
Simple OS/terminal simulation with basic system functionality (similar to linux)

# This is a college project codebase.
This code shouldn't be ran just as it is, this is a stable version that contains basic functionality
and should be expanded further. No external libraries were used so some functionality of the program
is rather ghetto. One thing that this codebase is missing is the multithreading capabilities (easily
implementable, _https://github.com/kmalbasic/Multithread-Base_)

# Programming language used?
**C++** with some **C** tossed into the mix. Not fancy, but it gets the job done.

# Functionality of the program
Program itself can do lots of basic things, using command "help" when you run it lists some functions that
you can use. All functions are currently stored in _User_cmd.hpp_ and they are stored in a namespace so you
can easily declare/define new ones. Cool thing you can add: make the program automatically recognize math expressions
and print out the answer!

# How to use it?
Place the OS into a folder named OS. The OS will probably ask you to create a new user account and simply run after you
create one. Type in "_help_" and select what command you want to run! (big sorry for everyone having issues with "_ls_"
printing out blank directories and files, reason being the way OS sees the files (OS folder is meant to simulate a disk,
directory which contains OS.exe is considered root)

# Current known bugs

- Command "ls" will crash the program when trying to list out directories within a non-existent path. Will add a check when
I grab some time.
- Currently only BMP files are being rendered in terminal, you will need to add BMP conversion functions to actually render other
file types. External libraries are not allowed for this project (college rules yaaay) so either write a conversion library.
- **somewhat of a bug** "ls" will output blank directories/files if OS executable is not placed and ran in a folder named **OS**
