# UNL Research
This notebook contains all the research I did at University of Nebraska - Lincoln. It contains information on how to work with root files and apply a kinematic study for Effective Field Theory (EFT) analysis of Top Quark Events. Here is a very brief description of what each notebook does.

## Uproot tutorial: 
Mirrors tutorial found at https://hsf-training.github.io/hsf-training-uproot-webpage/02-files/index.html. In this notebook, we learn how to open root files, extract information from branches, and apply cuts.

## Accessing root files:
Puts into practice the skills learned in Uproot tutorial but in the context of EFT. In this file, I worked with the EFTfitCoefficients branch and plotted different pieces of relevant information.

## Json WC:
There are 561 pairs of EFT Coefficients that come from the cross terms of 32 EFT Coefficients + 1 SM Coefficient. Each of the 33 coefficients has a different name that we gathered from this json file: https://github.com/TopEFT/topeft/blob/run3_test_mmerged/input_samples/sample_jsons/signal_samples/ND_SRskim2023/ttH_NDSkim_2023.json
In this notebook, we make all 561 pairs, and create useful tools that we will be using in the other notebooks. Some of these tools include: how to find an index given a pair and vice-versa and how to find in which pairs a specific coefficient is found.

## Mean and Median
Plots for the mean and median of each EFT Coefficient. 

## FINAL High vs Low Jet $p_t$ EFT Coefficients:
Selects events with a total Jet $p_t$ above 500 GeV and finds the EFT Coefficients from these events. From these EFT Coefficients, we append the index of the largest coefficient to another list. From this list, we plot the frequency of finding a specific index (0-560) in this list. We repeat this procedure for the events with a total Jet $p_t$ below 500 GeV.

## FINAL Leading Lepton $p_t$ and $\eta$:
Finds the two leading lepton $p_t$s and their corresponding $\eta$s. We append all the EFT Coefficients from these events and take the index from the largest value to another list. From this list, we plot the frequency of finding a specific index (0-560) in this list. We do this for leptons with $p_t$ above 50 GeV and also leptons above 30 GeV. There are two methods in the notebook.

## FINAL Number of leptons EFT Coefficients:
Categorizes events based on the number of leptons and their charge. Then we append all the EFT Coefficients from these events and take the index from the largest value to another list. From this list, we plot the frequency of finding a specific index (0-560) in this list. We do this to events with 3 leptons, events with 2 leptons with the same charge, events with 2 leptons with the opposite charge. At the end, the mean and median from each of the three categories is plotted.

## Slow Code:
The files found here have two versions of the code: one optimized and one slow. Since the optimized version is our interest, I made their own version with the name "FINAL..." in the main folder, but still saved the slow versions for future reference or possible mistakes.

## General coefficients:
Combines all of the different kinematic effects mentioned and cuts in one single notebook and outputs a list of the coefficients of interest (based on the frequency we choose). Currently has slow versions of code. Will try to update with optimize version in the future.

## Testing other file:
Uses another root file (still ttH) to confirm patterns or inconsistencies.

## Pytorch Tutorial.
Follows tutorial on how to build a toy Neural Network from https://www.youtube.com/watch?v=JHWqWIoac2I . 