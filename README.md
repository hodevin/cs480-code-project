# PMG Maze Game

## Devin Ho

A coding project that serves as the other half of the final assignment.

## Goal

For our project, we are going to further experiment with graph theory. Our plan is to randomly generate nodes and edges to create a maze. We will be able to create both complex and simple mazes in order to produce a wide range of data. After we generate the maze, we will randomly generate a maze-runner. The goal of this maze-runner is simply to make it to the end of the maze. Upon completion of the maze, we will collect and store the output. Utilizing this output, we will be able to calculate the time of completion and store the maze solution for further use.

The solutions to the maze can be further looked into in order to apply further problem solving. This project will reflect the concept of shortest path problem in graph theory. According to the article, this concept is actually called Dijkstra’s algorithm, which finds the shortest path between node A and node B. In relation to our discrete structures class, this project will be written in Python. It also holds content within graph theory which is relevant to our class.

## Approach

In order to make a maze, we can use the python package called `pygames`. This link is the tutorial of how to use `pygames` package to design a maze: https://pythonspot.com/maze-in-pygame/. However, the tutorial only showed an example of making a SNEED to discuss the process of making a simple maze

We would want the maze to be randomly generated to make it more complex. We can use another python package called `hypothesos`.  The package is a strategy to generate any kind of data. Based on the graph theory in python, the maze will just be a dictionary. The way to randomly generate a dictionary by using `hypothesos` is with using the following link: https://hypothesis.readthedocs.io/en/latest/_modules/hypothesis/strategies.html#dictionaries.

To analyze the time for the maze runner to run, we can use the python package called `perf`. It is a module in python that can write, run, and analysis benchmarks. Here is the user guide for `perf`: https://perf.readthedocs.io/en/latest/ . It will store the output in the `JSON` format, so we probably need to use `JQ` to make the output be readable. This the `JQ`'s official website: https://stedolan.github.io/jq/. There is a package we can use in python to analysis JSON code.
