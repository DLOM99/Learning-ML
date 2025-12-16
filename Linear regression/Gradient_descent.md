
#### Linear regression model :
    f_w,b(x) = wx + b 

    w  = weight
    b  = biais

### cost function  :

    Y(hat)^i =f_w,b(xi) = wxi + b

    1/2mSum((Y(hat)^i - Y^i)^2) from 1 to m

    w = w - alpha d(J(w,b))/dw (1)

    b = b - alpha d(J(w,b))/db (2) 


alpha is the learning rate 
    a number that could be between 0 and 1  
    It represent how big of a step we are taking down to find the local or global (lowest possible value) minima 
    IT should not be :

    - To small : slower to converge 
    - To large : overshoot and may never converge, diverge

    When we reach a local minima or if we started with a point that is a local minima, there is no need for further update because the function doesn't get updated. Meaning the slope (the derivative) will be equal to zero, now we have " W - alpha (J(w,b)')" which we be equal to W.

    Also this could be accomplished with a fixed learning rate, because the closer we get to the minima, the smaller the slope is and the smaller the step is.


Step 1 and 2 are updtated up until it converges (there is no significant changes)

The best practice to update the value of 1 and 2 is by doing SIMULTANEOUS update :

    tmp-w = w - alpha d/dw(J(w,b)) 

    tmp_b = b - alpha d/db(J(w,b)) 

    w = tmp_w 
    b = tmp_b 


## Intuition Gradient descent 


## Implementation 


    tmp-w = w - alpha d/dw(J(w,b)) 

    tmp_b = b - alpha d/db(J(w,b)) 

   J(w,b) =  1/2mSum((Y(hat)^i - Y^i)^2)


Ran until convergence

## type of gradient descent :

1. Batch : gradient descent is ran on all the training example for each iteration. 









