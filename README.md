# Dveco
A recursive lossy image compressor based on standard deviation, clearly worse than JPEG.

Name stands for *Deviation Compressor*. 

It is a [Pluto notebook](https://github.com/fonsp/Pluto.jl) written in [Julia](https://julialang.org/). Has a live demo and everything. 

## How it works
It calculates the standard deviation of the color value of the pixels in an image. Then, it splits the screen in four and calculates the standard deviation for each quadrant. When it is below a certain threshold, it stores the average value and the size of the image portion currently being evaluated. It has around 10-50% size reduction at a (more or less) acceptable threshold. 

## Should I use it?
No. JPEG is smarter, more sofisticated and simply better in every single way. 

## Demo

With a compression threshold of 0.064: 

<div>
  <img width="188" alt="Newton" src="https://upload.wikimedia.org/wikipedia/commons/3/39/GodfreyKneller-IsaacNewton-1689.jpg">
  <img width="188" alt="compressed image of Newton" src="https://user-images.githubusercontent.com/53334434/165480375-5483e015-924d-4831-a70b-3a010c22659d.png">
</div>


## Credits

Original concept and implementation done by the great sr. Sánchez, my math teacher. However, his version used JavaScript, so this is a much need, much faster reimplemantation written in Julia. 
