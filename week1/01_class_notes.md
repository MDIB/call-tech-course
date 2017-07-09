- The learning problem

   - how viewer will rate a movie (netflix) , 10% inc -> 1 million dollars prise
    - the essence of machine learnign 
      - A a pattern exists (in this case: there's a question that relates the way a person rates a movie and to how he rated other movie and other people rate this movie
      - B We cannot pin it down mathematically
      - C We have to have data
      

``` UNKNOWN TARGET FUNCTION (IDEAL)
           |
           |
           |
           V
   TRAINING SAMPLES
           |
           |
           ----- > LEARNINNG ALGORITHM -----> FINAL HYPOTESIS (Trained model)
           |
           |
           |
   HYPORTESIS SET```
    
- Perceptron Learning Algorithm 

Xn is some property that the customer has (e.g. salary, years livin at same house etc.)
Wn is some weight interwined with that Xn property

the h(x) = wT.x (the vector of weights transposed to be multplied by the vector of properties)

the linear leaning algorithm

all the weights start at a random value.

everytime a weight results into some invalid state the weight is sum or subtract by x depending on wheater the weight was -> or <- the property vector (vector theory)


supervised learning -> Learning from data and correct outputs e.g. set of coins mesures and correct coin representations (1,5,10,25)


unsupervised learning -> learning from unclassified data, you have a set of coins mesures and your cluster into different (approximatedely) categories based on this measures so when someone tells you that a coin of size x and weight y is a dime you know all the coins that you've classifed equally to that one its a dime too. downside is that sometimes is hard to distinguish clusters because they can be very approximated.


reinforcement learning -> learning from classified data and some output (not necessarely the correct one) and then your algorithm output is graded with a percentage of correctness.


