# UNL Research
This notebook contains all the research I did at University of Nebraska - Lincoln. It contains information on how to work with root files and apply a kinematic study for Effective Field Theory (EFT) analysis of Top Quark Events. Here is a very brief description of what each notebook does.

## Uproot tutorial: 
Mirrors tutorial found at https://hsf-training.github.io/hsf-training-uproot-webpage/02-files/index.html. In this notebook, we learn how to open root files, extract information from branches, and apply cuts.

## Accessing root files:
Puts into practice the skills learned in Uproot tutorial but in the context of EFT. In this file, I worked with the EFTfitCoefficients branch and plotted different pieces of relevant information.

## Json WC:
There are 561 pairs of EFT Coefficients that come from the cross terms of 32 EFT Coefficients + 1 SM Coefficient. Each of the 33 coefficients has a different name that we gathered from this json file: https://github.com/TopEFT/topeft/blob/run3_test_mmerged/input_samples/sample_jsons/signal_samples/ND_SRskim2023/ttH_NDSkim_2023.json
In this notebook, we make all 561 pairs, and create useful tools that we will be using in the other notebooks. Some of these tools include: how to find an index given a pair and vice-versa and how to find in which pairs a coefficient is found.

## Mean and Median

## High vs Low Jet $p_t$ EFT Coefficients:
Applies a cut to events with a total Jet $p_t$ above 500 GeV and finds the EFT Coefficients from these events. From these EFT Coefficients, we append the largest one to another list. From this list, we plot the frequency of finding a pair being in this list. We repeat this procedure for the events with a total Jet $p_t$ below 500 GeV.

## Leading Lepton $p_t$ and $\eta$:
Finds the two leading lepton $p_t$ and their corresponding $\eta$. We append all the EFT Coefficients from these coefficients and take the pair with the largest value to another list. From this list, we plot the frequency of finding a pair being in this list. We do this for leptons with $p_t$ above 50 GeV and leptons above 30 GeV.

