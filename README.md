# Stairway_plot2_tutorial
Workshop for using demographic inference analysis Stariway Plot2 on RAD-seq data from Quercus insignis

This is a tutorial for using Stairway Plot2.
We will go over six main steps for conducting this analysis.

1) Overview of the site freuquency spectrum (sfs) and the .sfs file
2) Downloading STWP2.
3) The .blueprint file: parameters and sequence length estimation
4) Commands for running the analysis
5) Graph the results with ribbon plots on R studio
6) Interpreting the results and comparing population/regional histories

#Downloading STWP2

You can download the executable files of STWP2 v 1.1 in this github repository https://github.com/xiaoming-liu/stairway-plot-v2/tree/master
No installing needed, only place your .sfs files inside the stairway_plot_v2.1.1 folder.

#The Blueprint File

Clone this repository with the command git clone https://github.com/Sergio-Marrugo/Stairway_plot2_tutorial/tree/main
In the sfs folder you will find a file Example_folded.blueprint. During the session we will get familiar with this file, for it is the place where we specify the parameters to use during the analysis.

We will need to modify the following entries:
popid: id of population, no whitespace allowed
nseq: number of chromosomes in the population
L: sequence length
SFS: copy and paste the sfs from your population without the first column of invariant sites.
nrand: number of randomization break points according to the manual
project_dir: name of the directory you want the results in
mu: mutation rate
year_per_generation: generation length
plot_title

#Estimating the sequence length

In the sfs folder you will find the seqLength.txt file with the rationale for estimating parameter L
The number of total sites and polymorphic sites are found in the file populations.sumstats_summary.csv

#Commands for running the analysis

STWP2 folder comes with a pdf manual where you can find the steps and commands for running this analysis

Create ribbon plots in R

Download the results and the ribbon_plots.r file into your PC and follow the steps for creating the graph.
