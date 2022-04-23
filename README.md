# Raylib Setup using Premake5
This is a simplified set of instructions for how to setup a project using premake.

## Video Tutorial
A video covering this process is here
https://youtu.be/oHIh01L6xQQ

# Download this repository
Download the game premake repository from 
https://github.com/raylib-extras/game-premake/tree/no_edit
Download the zip file, or clone the repository. It doens't matter what one you use.
Rename the folder whatever you want. This will be the name of your game.

#(OPTIONAL) Get Raylib
If you wish to use a specific version of raylib, follow the instructions below. If you want the current developmetn version, skip this section and premake will download raylib for you.

## Download Raylib
Get the raylib sources from 
https://github.com/raysan5/raylib
Download the zip file, or clone the repository. It doens't matter what one you use.
Put the raylib sources in a folder called raylib inside your game folder (The same folder this file is in). The folder must be named raylib, it can not be raylib-master. The raylib folder should contain all the sources from raylib (including the 'src' folder)

# Example app
This repository is pre-populated wit the raylib game template. It is a great starting point for your game.
https://github.com/raysan5/raylib-game-template

If you want to have a different starting point, simply repalce the files in the game folder with your own files.

## Using C++
By default this process is setup to build a project using C. If you want to use C++, you can replace these files with cpp files.

# Generate Projects
For windows users, there are two batch files you can use depending on what compiler you are using. For linux users you can simply use a terminal.
Only do ONE of these options depending on your compiler and platform.
## Windows Users
Visual Studio users should run

    premake-VisualStudio.bat
	
This will generate a Visual Studio project.
	
## MinGW-w64 Users
Run the batch file.

    premake-mingw.bat

This will generate a makefile for you
	
## Linux users
cd to the game folder and run

    ./premake5 gmake2

This will generate a makefile for you.
	
# Build your game
Only do ONE of these options depending on your compiler and platform.
## Windows Users
Double click the .sln file that was generated in the folder. If you are using Visual Studio 2022 you will be asked to upgrade the project, the defaults are fine, accept them and it will load.
From here you can use the prouject as normal.
	
## MinGW-w64 Users
Open your compiler terminal (w64devkit if you are using it), change to the game folder and type 

    make
	
This will build your game
	
## Linux users
Open your terminal, change to the game folder and type.

    make
	
This will build your starting game template
	
