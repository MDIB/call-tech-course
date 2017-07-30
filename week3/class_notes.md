- Traning vs Testing 

  - Testing (Math desc.)
    P[|Ein - Eout| > þ] <= 2 e^(-2þ²N)
        |     |____ > how well you understand the material proper 
	|     
	V
    How well you did on final	
 - Training -> same as tests but with M (number of hypotesis in the Hset)

 - The problem is, usualy M tends to infinity, lets recap how we computed M:
 
  - Hoeffding inequality cames from the wish to prove that our Ein will track 
    Eout fairly. 
  - So we say that |Ein - Eout| is less than þ (a small quantity)
  - The hoeffding states that þ quantitty will exponentially increase the probability that 
    P(|Ein - Eout | < þ) to be false (bad event), so you would have to increase N in order 
    to satisfy the probability to be small.
  - So, bad events, what do they mean? Well they mean that we didn't tracked Eout well, mostly.
  So for that hypotesis X we couldn't achieve learning. 
  - So the M is simply the union bound between hipotesis and by the
  rules of probability of DISJOINT events (P1 or P2 = P1 + P2).
  - But the thing is, the hipotesis are not DISJOINT, in most cases they overlap A LOT.
  - Now we just have to use this in our favor to have something meaningful about feasibility of 
  learning even with (~ infinity Hset)

  - What can we haplace M with?
    - Instead of the whole input space (infinity), that aways generate infinite hypotesis, we 
    could use DICHOTOMIES between hypotesis within the IN-SAMPLE dataset.
    - This has the upper hand of at most 2^n hypotesis.

  TODO anotate -> growth function, break point ... validation table on perceptron, convex space and rays...

