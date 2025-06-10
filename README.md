# Edison Robot v3

This is where we put all of the resources for the Edison robots.
If you're looking for helpful information about the robot, check out the Wiki!

A helpful base with convenient aliases to common functions is available in `edbase.edpy`.

Note: We no longer use the Edison v3 robots as the programming language used 
for them is too limiting.

While the EdPy language is based off the MicroPython project, which aims to
implement many Python 3.6 language features, the EdPy version has many artificial
restrictions.

For example, lists cannot contain more than 256 items. In fact, the number of
references seems to be globally limited to around 256, so you can't refer to
more than 255 things globally (i.e. number of all variables, list elements, dict entries, etc.
must total less than 256)

Additionally, many common Python code patterns are forbidden, likely as they were deemed
too complex for K-12 students.

There are many more limitations which make these robots difficult to use for
swarm robotics and complex controls tasks. So, we have instead moved on to using
Hiwonder's TurboPis.