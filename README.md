# jupyturtle2
Python Turtle graphics for Jupyter notebooks

For a quick demo, open [the lab notebook](lab.ipynb).

`jupyturtle2` is a fork of [`jupyturtle`](https://github.com/ramalho/jupyturtle)
replacing SVG output with rendering on an `ipycanvas` widget.

It solves the problem of rendering SVG drawings that grow increasingly slow.

But it introduces two other problems:

1. A limited number of steps per second, which requires using `delay=0.01` for complex drawings.
2. The final state of the canvases is not saved with the notebook.

I used metaprogramming techniques to build the procedural API
with global functions like `fd()` to move the turtle.
The techniques are easier to understand in the didactic project
[abacus](https://github.com/fluentpython/abacus).


@ramalho
