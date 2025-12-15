# Linear regression with multiple feature


Linear regression can have multiple features. 

e.g : predict the price of a house, based on size , # of bedrooms, age of the house, # of floors etc

In this example we have mutliple features. 

x_j, x_j+1, x_j+2 , ......, x_n 

j = 1 

x_1, x_2, x_3,......, x_n




- x_j = jth feature.
- n = numbers of features 
- x^i = the features of the ith training examples.
- (x^i)_j = feature j of the ith training example 

e.g : (x^4)_1 = the value of the feature 1 (x_1) in the 4th training examples. 

SInce we are dealing with multiples features and values, Now we have vectors. 

x is now a vector = [x1,x2,x3,x4,...,xn]

Therefore the model or function becomes f(w,b) = wx + b is now a vector 

w1x1+ w2x2 + w3x3 + ... + wnxn + b 

W . X + b 

dot product between the vector w and vector X 



                        ### Vectorization ##### 

Implementation : 

W = [w1,w2,w3] [1,2,3]
X = [x1,x2,x3] [1,2,3]

b = number , 4

f = np.dot(W,X) + B 

this will run faster than 

for i in range(0,n):
    f += w[i]x[i]
    
f=f+b

