- Summary :

  - Input representation (sample DataSet will be used to show how important feature representation are)
  - Linear Classification (Generalize to non separable data)
  - Linear Regression (Real valued learning function) 
  - Non Linear transformations

Try ideas on real data.

Dataset of images of zipcode numbers, different ways to write numbers
256 real numbers = one 16x16 image, not optimal representation, 

- `PLA Pocket algorithm` -> Used when PLA doesn't converge (the dataset is not linearly separable), 
picks the best hypotesis (less errors) whitin an range of iterations on the PLA.

- `Linear Regression` "bread and butter" error measure is `squared errors (h(x) - f(x))` and we use it to approximate Ein to Eout better 
(minimize the error).
Expr for Ein: `Ein(w) = (1/N)Sum(n=1,N)(w^t * Xn - Yn)^2 => (1/N)*||Xw-y||^2` where ```X = | x1^t| Y = | y1 |
                                                                                           | x2^t|     | y2 |
										           | x3^t|     | y3 | 
										             ...        ....
										           | xN^t|     | yN |``` 
"||" =>  the vector is transposed and them multiplied by itself (the square is not really a square).


Since you want the minimum Ein (`h` approximating `f` well, you will take the derivative of Ein ) 
 `Ein'(w) = (2/N) X^T(Xw -y) = 0` you want all the elements in the result vector to be zero, so:
 `X^T*Xw = X^Ty` => `w=X^þ*y` where `Xþ= ((X^T*X)^-1) XT` because you can eliminate (X^T*X) multiplication of w by multipling it by its
 inverse matrix so the other side of the equations turns into `((X^T*X)^-1) * X^T` also Xþ is know as the `pseud-inverse` of X
														 
- The pseudo-inverse 
  Xþ




Questions 
Why we have a threshold even when we are working to get real valued data like numbers, I mean it 
makes sense to have this for binary classification but I can't really see it working on real data.

