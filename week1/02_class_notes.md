Is learning feasible?

Yes, in a probabilistic sense.

Image we have a opaque bin (maybe infite extensivly) 

And we catch marbles in this bin, (independently, with reposition).

Will the in-sample (marbles we check) performance tell us anything about the out-sample
(that we don't saw yet) performance?

Yes, as the hoefling equation proves that the probability of E(in) deviates from E(out) by more then e' 
where e' is provided by us is less than a small number :

`Hoefling Eq : P(|E(in) - E(out)| > e') < e^(2e'².N)`

But when we have lots of hypotesis we have to add an M factor (where M is the number of hypotesis in the 
hypotesis set) because we say that |E(in(Hm)) -E(out(Hm))| > e or ... for each m in M that means that we
are looking for the probability within disjoint events so we apply the probability laws that say that the
upper bound of probabilities that are disjoint related by `or` are going to be the sum of the probabilites
so now we have :

`Hoefling Eq : P(|E(in) - E(out)| > e') < M.[e^(2e'².N)]`
