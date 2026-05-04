simple_examples.ipynb has examples of the Forward Algorithm, the Forward-Backward Algorithm and Viterbi Algorithm.

All are used in Hidden Markov Models, where the Markov Chain is not directly observable, but each state will produce an observable output.
ie We have sunny, rainy, cloudy states. We live inside, and can't see what the weather is (hidden states), but we can see the emotions of our colleague (observable output).
If it is rainy, there is 1/5 chance our colleague is happy, 3/5 chance they are sad, and 1/5 chance they are neutral.

The Forward Algorithm, given a sequence of observed outputs ("happy", "neutral"), calculates the probability of being in a specific hidden state X at a time T, given the the observable outputs from time 1 to T.
By summing the probabilities of all the hidden states at the final time step, we get the probability of getting this sequence of observed outputs.

The Forward-Backward Algorithm, calculates the probability of being in a specific hidden state X at a time T, given the entire sequence of observable outputs (not just the outputs from 1 to T). This is done by combing both "forwards" and "backwards" passes through the chain.

The Viterbi Algorithm, given a sequence of observed outputs ("sad", "sad", "happy"), calculates the most likely sequence of hidden states corresponding to the observed outputs ("rainy", "rainy", "cloudy").
