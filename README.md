# CUDA implementation of Conway's Game of life in Google colab
This project implements Conway’s Game of Life using CUDA to demonstrate GPU parallelism for
fast and large-scale simulations on Google collab

* You can follow the [Report](Report.pdf) for detailed explanation of the concept and the implementation along with the results.

## What is Conway's Game of life?
Conways game of life is a cellular automaton; in simple words it’s a game with 4 rules. Those
rules are:
1. Any live cell with fewer than two live neighbors dies, as if by underpopulation.
2. Any live cell with two or three live neighbors lives on to the next generation.
3. Any live cell with more than three live neighbors dies, as if by overpopulation.
4. Any dead cell with exactly three live neighbors becomes a live cell, as if by
reproduction.

The best way to undertsand is to try it yourself!! try it online at [Conway's game of life](https://playgameoflife.com/)

## CUDA
I wrote this in Cuda as its one of the most popular framework to interact with GPU's. Understanding how to leverage cuda can be crucial when you
need to improve performance or scale things up. Take a look at the perfromace improvement below:

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/87a09aed-e4d3-4d29-8d47-f9551395ae9a" />

You can see that the GPU takes the same amount of time,while the CPU takes significantly longer! <br>
This also happened to one of my assignments but we will conviently ignore that :)


## Why Google Colab?
I recognise that not everyone has access to GPU's( i didn't!) and that's why I decided to write the code in Google colab. This way anyone can change the code and run it,irrepctive of thier machine.

Colab also gives you the flexibility to experiment!,you can always change the code and see how diffrent the performance is affected.


## Future Improvements 
In later version, I will add the following:
* Implement the same with a proper UI and smooth transitions.
* Add inputs for width and lenght ,and iterations.
* Display just how fast the GPU is when compared to the CPU
* Change the 4 basic rules themselves!

Below is the animation that I have captured.
Its a little janky,but runs a lot smoother usually.



![animation-GOL](https://github.com/infinite08/CUDA_Game_of_life/blob/main/animation-GOL.gif?raw=true)

