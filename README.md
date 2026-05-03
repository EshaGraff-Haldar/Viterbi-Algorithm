The repo has simple examples of both the Forward Algorithm and Viterbi Algorithm.

Both are used in Hidden Markov Models, where the Markov Chain is not directly observable, but each state will give produce an observable output.
ie We have sunny, rainy, cloudy states. We live inside, and can't see what the weather is (hidden states), but we can see the emotions of our colleague (observable output).
If it is rainy, there is 1/5 chance our colleague is happy, 3/5 chance they are sad, and 1/5 chance they are neutral.

The Forward Algorithm, given a sequence of observed outputs ("happy", "neutral"), calculates the probability of getting this sequence of observed outputs.

The Viterbi Algorithm, given a sequence of observed outputs ("sad", "sad", "happy"), calculates the most likely sequence of hidden states corresponding to the observed outputs ("rainy", "rainy", "cloudy")
