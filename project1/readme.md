# Code Review for _Insert Name Here_

## Project Repo

https://github.com/cavacado/poc


#### Project Purpose

_List the purpose and components of the project here_
P.O.C is an exciting game that require player to construct a pipeline system. The main goal of this game is to channel the flowing fluid from the inlet to the outlet. The player can do so by switching the position of two tiles.

The project structure are as follow:

* HTML
  * index.html
    * The main project html site.
* Javascript
  * main.js
    * The main javascript file.
    * Hold main game logics.
  * randomColor.js
    * Random color generator library by David Merfield.
    * Employed to generate the color scheme of tiles in this project.
  * vanilla-notify.js
    * Vanilla-Notify library by MLaritz.
    * Employed to handle notifications in this project.
* css
    * style.css
      * Holds majority of the style in this project.
    * flow.css
      * Holds keyframes style for flow animation.
    * vanilla-notify.css
      * Holds style got all notifications.


#### Project Organization

#### Features

* Flowing Fluid Animation.
  * The animation is achieved via keyframes and css clip-path. The developer uses clip-path: polygon to set the initial and final shape of the images, allow it to create a fluid-flow-like animation.
  * The clip-path property in CSS allows you to specify a specific region of an element to display, rather than showing the complete area. For example:

  ```
  clip-Path: polygon (x1 y1, x2 y2, x3 y3, x4 y2)
  ```
  This forms a square with the x and y coordinate inputed.

* Switching of tiles
  * The switching of tiles is done by currying methods.
  * Currying refers to the process of taking a function with n arguments and transforming it into n functions that each take a single argument.

  ```
  function swapFunc(id1,class1){
    //Code here
      return function (id2,class2){
        //code here
      }
  }
  ```
  The function will invoke when the 2nd pair of parameter are available.


#### Areas of Success (Code, Organization)

* Flowing Fluid Animation.
  * The animation form a Wow factor in the game. It enhance the overall user experience.
  * The use of keyframe and clip-path to form the fluid flow animation is eye opening, especially for the elbow-like pipe.

* The multiplier Feature.
  * The length multiplier add some excitement to the original game. It motivates player to form a longer pipeline and thus made the game more challenging.

#### Areas for Improvement (Code, Organization)

* Disable Used Tiles
  * The player are still able to select the used tiles. It will be better if it could be disabled.
* Factoring of Code
  * Some part of the code can be refactored to make it more readable.

## Additional Notes

_Place any additional notes here_
