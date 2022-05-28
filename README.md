# multilevel-venn
Rectangular Venn Diagrams for Comparing Across and Within Cases Simultaneously

Sometimes we are interested in analyzing simultaneously differences between and within cases. For example, perhaps we want to compare the proportion of people who are (a) living alone, (b) single, and (c) feeling lonely within a given society. We are interested in all the possible overlaps between these and how much of the sample resides in each of the 8 possible subgroups (a, b, c, ab, bc, ca, abc, or none of these overlaps). This is easy enough with a scaled Venn Diagramme. However, what if we want to at the same time compare this information across countries? Enter the multi-level Venn diagramme. Using scaled regular Venns we can look at within- and between country proportions at the same time, thus allowing us to spot patterns we might not otherwise see. 

#To run a random demonstration:
Simply source the 'supervenn v5.R' file within RStudio. You will get some output of the rectangle coordinates as well as their closely approximated visualizations.The state accuracy corresponds to how close the visualization corresponds to the actual proportions in the data. You can increase the accuracy (at the cost of increasing  run-times by changing the 'perm' value (permutations) on line 15 of the code to 4 or 5. 

#To run your own data on this:
I have not adapted this yet, but you would want to take a look at the structure of the dt datatable on line 46 of the 'fake data generation portion'. Make your data match this structure, change the labels for your categories with 'mylabel' (line 8) and the overall graphic label on line 319, and you should be good to go. Note that this is not built to handle more than 3 overlapping categories. 
