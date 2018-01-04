Q1. *Picture missing*
**Detect image contrast**
 
Q2. Suppose your input is a 300 by 300 color (RGB) image, and you are not using a convolutional network. If the first hidden layer has 100 neurons, each one fully connected to the input, how many parameters does this hidden layer have (including the bias parameters)?
**(300\*300\*3 + 1) \* 100 = 27,000,100**

Q3. Suppose your input is a 300 by 300 color (RGB) image, and you use a convolutional layer with 100 filters that are each 5x5. How many parameters does this hidden layer have (including the bias parameters)?
**(5\*5\*3 + 1) \* 100 = 7,600**

Q4. You have an input volume that is 63x63x16, and convolve it with 32 filters that are each 7x7, using a stride of 2 and no padding. What is the output volume?
**(63-7)/2 + 1 = 29**
**29\*29\*32**

Q5. You have an input volume that is 15x15x8, and pad it using “pad=2.” What is the dimension of the resulting volume (after padding)?
**15+2\*2 = 19**
**19\*19\*8**

Q6. You have an input volume that is 63x63x16, and convolve it with 32 filters that are each 7x7, and stride of 1. You want to use a “same” convolution. What is the padding?
**(63+2p-7)/1 + 1= 63 => p = 3**

Q7. You have an input volume that is 32x32x16, and apply max pooling with a stride of 2 and a filter size of 2. What is the output volume?
**(32-2)/2+1 = 16**
**16\*16\*16**
 
Q8. Because pooling layers do not have parameters, they do not affect the backpropagation (derivatives) calculation.
**No**
 
Q9. In lecture we talked about “parameter sharing” as a benefit of using convolutional networks. Which of the following statements about parameter sharing in ConvNets are true? (Check all that apply.)
- **It reduces the total number of parameters, thus reducing overfitting.**
- **It allows a feature detector to be used in multiple locations throughout the whole input image/input volume.**
 
Q10. In lecture we talked about “sparsity of connections” as a benefit of using convolutional layers. What does this mean?
- **Each activation in the next layer depends on only a small number of activations from the previous layer.**
