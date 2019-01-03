# RawDataSolver_YUV
C# YUV format Solver 
What is Chroma Subsampling?
Chroma subsampling is a type of compression that reduces the color information in a signal in favor of luminance data.
This reduces bandwidth without significantly affecting picture quality.

4:4:4 VS 4:2:2 VS 4:2:0
The first number (in this case 4), refers to the size of the sample. 
The two following numbers both refer to chroma.
They are both relative to the first number and define the horizontal and vertical sampling respectively.

A signal with chroma 4:4:4 has no compression (so it is not subsampled) and transports both luminance and color data entirely. 
In a four by two array of pixels, 4:2:2 has half the chroma of 4:4:4, and 4:2:0 has a quarter of the color information available. 
The 4:2:2 signal will have half the sampling rate horizontally, but will maintain full sampling vertically.
4:2:0, on the other hand, will only sample colors out of half the pixels on the first row and ignores the second row of the sample completely.

![alt text](http://i.rtings.com/images/chroma-subsampling/subsampling.png)
