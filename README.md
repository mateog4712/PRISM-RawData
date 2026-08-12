# PRISM-RawData
This repository holds all of the data for the PRISM project.

ProofOfConcept holds the all input and output files to show that pseudoknot-free version of PRISM produces the same result as RNAFold given the same input. As a measure of correctness, we look at MFE, ensemble energy, MEA, and centroid distance, in that order.

FrequencyValidation validates the results for sampling. We look at the sampling derived frequency of the MFE structure vs the calculated Boltzmann contribution of MFE / total Boltzmann ensemble. We compare for 1000, 10000, and 100000 samples. The results are shown in two columns with the first being calculated and the second being estimated.

Sampling validates the effect of increased samples have on the PRISM runtime and posterior probability estimates. Fasta gives the sequence/structure pair for their respective size. 100000samples is the baseline that is compared against. NumSamples is the list of sample sizes i.e. each number describes the number of samples at that step. RMSD gives the RMSD at each of those steps. Time gives the time and memory at each of those steps.

TimeAndMemory shows the comparison between PRISM, RNAFold, and NUPACK 3.0 when observing time (s) and memory (KB).