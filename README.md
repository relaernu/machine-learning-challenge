For this challenge, I have tested 3 different models with all the feature columns as input:

1. Linear kernel grid search; (0.802|0.818)
2. RBF kernel grid search; (0.787|0.801)
3. Poly kernel grid search; (0.494|0.520)

And then to test if different category of features has any effect to the model. By the 
By the Kepler Objects of Interest Table, the features can be split to 4 differenct groups: Disposition Flags, Transit Properties, Stellar Parameters and KIC Parameters. So I then make the following Linear kernel grid search model by fiting different X input:

4. Without any Flags; (0.639|0.641)
5. Without any Transit; (0.777|0.811)
6. Without any Stellar; (0.792|0.804)
7. Without any KIC; (0.790|0.802)

By comparing all this models, I found that all the features have effect to the model, and the Flags features have the greatest effect. And the best kernel is linear kernel. 