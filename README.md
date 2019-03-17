# CS110-Graphics

CS110-Graphics is a graphical addiction to Python written in Python 2.7, for use in teaching environments. It was originally developed by me during the summer of 2017 for Hamilton College's Computer Science department, and built upon and de-cluttered by Professor Alistair Campbell and Paul Magnus in later years.

The backing environment is based off of tkinter's canvas object. It also includes a Doxygen executable which builds a documentation using the cs110graphics.py file. The most up to date version of this executable (as well as the most up to date output files) have been included in the repository.

## Dependencies

This project uses tkinter, math, inspect, and Pillow (formerly PIL). Ensure these dependencies are installed before usage.

## Usage

Import it into a Python 2.7 file using "from cs110graphics import \*".

## Class & Method Hierarchy

* Event
  * get_button()
  * get_description()
  * get_key()
  * get_mouse_location()
  * get_root_mouse_location()

* EventHandler
  * handle_key_press()
  * handle_key_release()
  * handle_mouse_enter()
  * handle_mouse_leave()
  * handle_mouse_move()
  * handle_mouse_press()
  * handle_mouse_release()

* GraphicalObject
  * add_handler()
  * get_center()
  * get_depth()
  * move()
  * move_to()
  * set_depth()

* Fillable (extends GraphicalObject)
  * get_border_color()
  * get_border_width()
  * get_fill_color()
  * get_pivot()
  * rotate()
  * scale()
  * set_border_color()
  * set_border_width()
  * set_fill_color ()
  * set_pivot ()

* Circle (extends Fillable)
  * set_radius()

* Oval (extends Fillable)
  * set_radii()

* Polygon (extends Fillable)

* Square (extends Fillable)
  * set_side_length()

* Rectangle (extends Fillable)
  * set_side_lengths()

* Image (extends GraphicalObject)
  * resize()
  * rotate()
  * scale()

* Text (extends GraphicalObject)
  * set_size()
  * set_text()

* Timer
  * set_function()
  * set_interval()
  * start()
  * stop()

* Window
  * add()
  * remove()
  * get_height()
  * get_width()
  * set_background()
  * set_height()
  * set_title()
  * set_width()

* RunWithYieldDelay()
* StartGraphicsSystem()

More detailed information and code samples can be found [within the folders of this repository (produced by Doxygen)](https://github.com/matthewjenkins97/CS110-Graphics/blob/master/latex/refman.pdf).

## Goals for later implementation

Port this to Python 3.

