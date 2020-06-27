# Predicting COVID-19 patient outcomes with clinical data
The COVID-19 pandemic caused by the novel coronavirus SARS-CoV-2 has spread to 216 territories worldwide, with over 7 million
cases of infection [1]. This has wreaked havoc in underprepared nations, such as Brazil, the epicenter of the pandemic in Latin
America, where the case count has surpassed 600,000 [2]. We obtained a publicly available dataset of patients admitted to a
Brazilian hospital [3], with information on the patients’ SARS-CoV-2 status, along with a battery of routine medical tests. Due to the
scarcity of SARS-CoV-2 tests, we aimed to identify SARS-CoV-2 status based on typical laboratory tests carried out in hospitals. We
used 16 haematological features in logistic regression and neural network models to determine SARS-CoV-2 status. Taking into
account the highly infectious nature of COVID-19, we preferred recall as a performance metric, since it would be better to
overestimate the number of positive cases, than to fail to quarantine even a single SARS-CoV-2(+) patient. The neural network and
logistic regression models performed similarly on our dataset, obtaining recall values of 0.84 and 0.82 respectively in the training set.
As for the test set, logistic regression achieved a slightly lower recall of 0.737, compared to 0.789 by the neural network. The neural
network produced marginally higher recall, accuracy, and precision, making it the marginally better model. While these results may
not be the most ideal, they still demonstrate that both models have some utility in distinguishing SARS-CoV-2(+) from SARS-CoV-2(-)
patients upon hospital admission, especially if COVID-19 testing is limited.

References
1) World Health Organisation. (2020, June 11). Coronavirus disease (COVID-19) pandemic. Retrieved from
https://www.who.int/emergencies/diseases/novel-coronavirus-2019
2) Horton, J. (2020, June 5). Coronavirus: What are the numbers out of Latin America? BBC News. Retrieved from
https://www.bbc.com/news/world-latin-america-52711458
3) https://www.kaggle.com/einsteindata4u/covid19/data
