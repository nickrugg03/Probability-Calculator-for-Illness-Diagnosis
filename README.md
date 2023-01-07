# bayes-theorem-from-external-data
This code reads values from an excel file, converts them to probabilities, and uses Bayes' theorem to calculate the probability of being ill given that you test positive (p(ill|pos)). The excel file contains the following values:

prob_pop: the population of a city (in millions)
prob_ill: the number of ill people in the city (in millions)
prob_pos_given_ill: the probability of testing positive given that you are ill
prob_neg_given_ill: the probability of testing negative given that you are ill
prob_healthy: the number of healthy people in the city (in millions)
prob_neg_given_healthy: the probability of testing negative given that you are healthy
prob_pos_given_healthy: the probability of testing positive given that you are healthy
The probB function calculates the probability of testing positive (p(pos)) using the probabilities of testing positive given that you are healthy or ill. The bayestheorem function uses Bayes' theorem to calculate p(ill|pos) using the probability of testing positive given that you are ill (p(pos|ill)), the probability of being ill (p(ill)), and the probability of testing positive (p(pos)). The resulting probability values are then printed to the console.
