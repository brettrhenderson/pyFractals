# PYFractals
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/brettrhenderson/pyFractals/master?filepath=Sierpinski_Triangle.ipynb)
<p align="center">
    <img src="videos/Sierpinsky.png" width=400/>
</p>
![Sierpinsky](videos/Sierpinsky.png?raw=true)

This was just a fun Jupyter Notebook that I played around with while
procrastinating on my chemistry research. While trying to find a video of when
Professor Oliver Knill created a [Miley Cyrus Wrecking Ball animation](https://www.thecrimson.com/flyby/article/2013/10/9/the-cyrus-infection-miley-crashes-math-21a/)
in Mathematica to show some friends, I stumbled across his Mathematics in Movies
page on his website, and his quick nod to [Annihilation](http://people.math.harvard.edu/~knill/various/annihilation/index.html)
and the iterated function system-like animation during the end credits. This sent
me down a rabbit hole of finding fractal-generating software, and I figured I would
try to generate some rudimentary fractals of my own in the language I know best:
Python!

I vaguely remembered this awesome
[Doodling in Math Class](https://www.youtube.com/watch?v=e4MSN6IImpI&list=PLF7CBA45AEBAD18B8)
video on binary trees that I had seen back in high school and thought that would be
cool thing to implement in code.

## The Sierpiński triangle
As mentioned in the Doodling in Math Class video, drawing a binary tree with
consistent horizontal and vertical spacing for branches, and in which the branches
that meet have no children, is one method of constructing the [Sierpiński triangle](https://en.wikipedia.org/wiki/Sierpi%C5%84ski_triangle).
The Wikipedia page also details some other pretty cool constructions and is worth
a look!  Using the binary tree construction, however, adds the cool element of
practicing and *animating!* some basic tree traversal algorithms.

## Accessing the Notebook
### On Your laptop
First, set up a virtual environment to run the notebook. I have tested this Notebook
using python 3.7, but it will ~probably~ work wit 3.5 or newer. Its only external
dependencies are numpy, matplotlib, and Jupyter, so if you are an Anaconda user
you should be set with a basic environment.  I have frozen my working environment
in [full_env.txt](requirements.txt) though as well, so if you are getting errors
or are using a python virtualenv, run

```pip install -r full_env.txt```

in your virtualenv to get the necessary dependencies. Alternatively, `requirements.txt`
has the base requirements but does not include jupyter. This is used for building the
notebook on [Binder](#on-binder) and means that if you were to run `pip install -r requirements.txt`,
you would have to also install jupyter separately.  Now you can explore the
notebook with

```jupyter notebook```

and then clicking on Sierpinski_Triangle.ipynb in the navigator.

### On Binder
A fully interactive version of the notebook is also available on [Binder](https://mybinder.org/v2/gh/brettrhenderson/pyFractals/master?filepath=Sierpinski_Triangle.ipynb).
Binder builds an environment for and allows you to run and change the notebook interactively
without needing to install anything on your own machine!

## Some Examples
