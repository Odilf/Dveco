# Dveco
A recursive lossy image compressor based on standard deviation, clearly worse than JPEG.

## How it works
It calculates the standar deviation of the color value of the pixels in an image. Then, it splits the screen in four and calculates the standard deviation for each quadrant. When it is below a certain threshold, it stores the average value and the size of the image portion currently being evaluated. It has around 10-50% size reduction at a acceptable threshold. 

## Should I use it?
No. JPEG is smarter, more sofisticated and better in every single way. 

## Credits

Original concept and implementation done by sr. Sánchez. As it was done originally in JavaScript, this is a much faster reimplemantation written in Julia. 
