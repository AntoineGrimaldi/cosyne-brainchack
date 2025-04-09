# OBJECTIVES: 
[x] extract statistics from [this dataset](https://datadryad.org/dataset/doi:10.5061/dryad.ksn02v76h#usage) : ISI and FRs
[] check if these statistics relate to the statistics of the generative model. If not, improve the model to go in this direction (final objective would be to generate data with a ground truth for the motifs using stats from real data)
[x] check how the different types of noise are implemented and improve if necessary
[x] add time wrapping (strech and compress spiking motifs), especially relevant here for hippocampal replay
[] assess the changes in statistics with behavior (optional)

# OUTCOMES:
- the generative model does not take into account the burstiness of the neurons and this should be taken into account. To solve this, we added a coefficient such that the FRs are increased during the occurrence of a motif (quick solution that links this event with the increase in spiking activity, realistic ?)
- we also added some warping (stretching or compression of the sequences) as an additional noise type in the model
- study of the statistics of different datasets was performed

# THANKS

[Deying Song](https://github.com/deyingsong), Jiayue Yang and [Zuzanna Slonina](https://www.researchgate.net/profile/Zuzanna-Slonina-2) where involved in this project
