# CPPND: Capstone Snake Game

This is repo for the Capstone project in the [Udacity C++ Nanodegree Program](https://www.udacity.com/course/c-plus-plus-nanodegree--nd213). he initial code for this project was provided by Udacity. The code for this repo was inspired by [this](https://codereview.stackexchange.com/questions/212296/snake-game-in-c-with-sdl) excellent StackOverflow post and set of responses.

<img src="snake_game.gif"/>

In this project, I have buildt my extended the version of Sanke game provided by UDacity by following the principles I have learned throughout Udacity's Nanodegree Program.


## Class Structure  
* This code has 4 main classes
    1) Snake - This class handles all activites related to snake in the game. Like the size of snake, speed of snake, etc 
    2) Game - This class handles all the activity related to game play for the game of snake. Like to see if we need new food, where to place new food, etc
    3) Renders - This class handles the graphics for the game using SDL library
    4) Controller - This class handles the hardware input for game play which in this case will be keyboard
## Game Play behaviour
*  GamePlay 
    * The game is a simple snake game. When the app is launched you will be see snake and food placed on the gridd. 
    * The goal for the user should be to eat the food and keep the snake growing without the head and tail get in contact with each ither becuase taht is hwo the game will end for the user 
    * User will be able to control the motion of snakes using the arrow keys on their keyboard

## RUbric Points addressed 
    * In game.cpp, renderer.cpp, snake.cpp and controller.cpp the code uses appropirate class structure
    * In snake.cpp the code uses OOP concept of data encapsulatoin 
    * In main.cpp concept of concurrecy is used by allowing only one instance of game to be played at a time 
    * In method ChangeDirection in controller.h and method UpdateBody in snake.h concepts of passing data by reference have been used 
    * The class Renderer in renderer.cpp has a destructr defined
## Dependencies for Running Locally
* cmake >= 3.7
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1 (Linux, Mac), 3.81 (Windows)
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* SDL2 >= 2.0
  * All installation instructions can be found [here](https://wiki.libsdl.org/Installation)
  * Note that for Linux, an `apt` or `apt-get` installation is preferred to building from source.
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)

## Basic Build Instructions

1. Clone this repo.
2. Make a build directory in the top level directory: `mkdir build && cd build`
3. Compile: `cmake .. && make`
4. Run it: `./SnakeGame`.