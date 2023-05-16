# KSON

Kohonen Self Organizng Map: Unsupervised Learning



We need to design a Kohonen self organizing map (SOM), which gives as an output some shades of color mapped over 100 by 100 grid of neurones. The training input of the SOM are 24 colors (use shades of red, green, blue, with some yellow, teal and pink) which you can choose from the "RGB Color Table: Basic Colors" section of this page: http://www.rapidtables.com/web/color/RGB_Color.htm

Using a time varying learning rate 𝛼(𝑘)= 𝛼(0)exp (−𝑘𝑇) (where k is the current training epoch (starts with epoch 0), 𝛼(0) = 0.8 , and T is the Total number of training epochs equal to 1000. Note that the epoch training involves all twenty four input samples for the 24 chosen colors to the network (hint: calibrate the color codes to values between 0 and 1, instead of being
between 0 and 255). Initial weights are randomized.

The topological neighbourhood 𝑁𝑖,𝑗(𝑘) of node (j) around the winning unit (i) is given by
exp(-d^2/(2sigma^2) and sigma update is = sigma = sigma_not*exp(-k/T)
and 𝑑𝑖,𝑗 is the distance between winning node i and surrounding node j. Initial value of 𝜎0=1


Generate, a figure of the original grid (randomly selected) followed by figures of the SOM grid after 20, 40, 100, 1000 epochs.
