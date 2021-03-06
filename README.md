# SelectScript_OpenRAVE

| Author      | André Dietrich                                                                           |
| ----------- | ---------------------------------------------------------------------------------------- |
| Source      | `git clone` https://gitlab.com/andre-dietrich/SelectScript_OpenRAVE.git                                 |
| Email       | <mailto:andre.dietrich@ovgu.de>          |
| Publication | 1. SelectScript: A query language for robotic world models and simulations               |
|             | http://eos.cs.ovgu.de/wp-content/uploads/2015/06/SelectScript-A-Query-Language-for-Robotic-World-Models-and-Simulations.pdf |
|             | 2. Reasoning in complex environments with the SelectScript declarative language          |
|             | http://arxiv.org/pdf/1508.04159v1.pdf                                                    |
| Slides      | 1. http://eos.cs.ovgu.de/wp-content/uploads/2015/06/ICRA2015-presentation-slides.pdf     |
|             | 2. to appear ...                                                                         |
| Misc        | https://pythonhosted.org/SelectScript_OpenRAVE                                           |

## Overview

It is an implementation of the SelectScript query language for robotics
simulation environment OpenRAVE.

## Installation

First of all you need to install the [SelectScript](https://gitlab.com/andre-dietrich/SelectScript.git)!

via Python setuptools:
```
$ sudo python setup.py build
$ sudo python setup.py install
```

If the Installation was successful can be checked from an IPython
interactive shell:

``` pyhton
# should work also for demo1, demo2, ...
import SelectScript_OpenRAVE.examples.demo0 as demo0
demo0.start()
```

## Tutorial

Please visit the package information site:

http://pythonhosted.org//SelectScript_OpenRAVE

## Media

The videos are screencasts of the examples provide within this project and shall
provide a first insight on the application of SelectScript.

#### [`examples/demo0.py`](SelectScript_OpenRAVE/examples/demo0.py) : simple (interactive) queries

[![YouTube](http://img.youtube.com/vi/R_PThP0gwOc/0.jpg)](http://www.youtube.com/watch?v=R_PThP0gwOc "watch on YouTube")

#### [`examples/demo1.py`](SelectScript_OpenRAVE/examples/demo1.py) : user defined relations:
Query for all objects that are "on" the table and in reachable distance to the
manipulator. And use the result as input for trajectory planning.

[![YouTube](http://img.youtube.com/vi/jSaoCXRNVNg/0.jpg)](http://www.youtube.com/watch?v=jSaoCXRNVNg "watch on YouTube")

#### [`examples/demo2.py`](SelectScript_OpenRAVE/examples/demo2.py) : defining situations by using triggers and callbacks:
Which sensor had perceived a robot during the last 2 seconds)? The result set is
used as input for the defined callback function, whereby the callback is only
executed, if the result has changed. The result set in this video is visualized
by the sensor beams.

[![YouTube](http://img.youtube.com/vi/Bk8TaOQQdZM/0.jpg)](http://www.youtube.com/watch?v=Bk8TaOQQdZM "watch on YouTube")

#### [`examples/demo3.py`](SelectScript_OpenRAVE/examples/demo3.py) : query for a sub-environment

[![YouTube](http://img.youtube.com/vi/k5NXVv6O3tU/0.jpg)](http://www.youtube.com/watch?v=k5NXVv6O3tU "watch on YouTube")

#### [`examples/demo4.py`](SelectScript_OpenRAVE/examples/demo4.py) : query for an OccupancyGridMap

[![YouTube](http://img.youtube.com/vi/MYQppe9E9Es/0.jpg)](http://www.youtube.com/watch?v=MYQppe9E9Es "watch on YouTube")

## Note

If you change the code, improve this project, fix bugs, or just have comments,
feel free to contact us ...
