#Exercises

The [Cancer Diagnosis](./archives/Cancer-Diagnosis.xlsx) spreadsheet works the same way as the bombers and seagulls scenario. 
It is designed to provide a realistic simulation of the cost-benefit assumptions that must be made to set the classification threshold for a medical diagnostic product. 
Download the spreadsheet and investigate the contents, below are details of what is contained in the file:

- The file has 10,0000 rows of data.
- The ranked scores in columnA are the level of a certain protein as measured by the diagnostic test.
- The true condition for each protein level is given in column C [Cancer=1, No Cancer=0].
- A threshold for a positive classfication can be set between any two protein levels.
- For each threshold in column A, the resulting number of false negative classification errors is given in column H, and the false positive classification errors in column F.

There are 100 correct cancer diagnosis out of the 10,000, resulting in 9900 correct no cancer diagnosis.
If you look at row 19, protein value 18636.922. If the threshold is set to greater than this amount there would be 1 true positive diagnosis and 9 false positive diagnosis.
This can also be read as saying at that threshold there would be for the sample, 9 false positives and 99 false negatives (only one true positive at that threshold out of the 100 total).

This spreadsheet is designed to allow you to observe how changing costs inputs impacts both:

- the overall costs of using a cancer diagnostic test at each threshold, and
- what threshold should be chosen as optimal thus minimizing costs.

Cell G3  contains the cost per False Negative (missing a cancer case) and cell H3 for the cost per False Postive (a false alarm).
Total costs as each threshold are given in column K.

The minimum total cost, and minimum cost per event (per diagnosed classifiction reported), are displayed in cells K4 , and L4, and the optimum threshold - the lowest protein level score that should be classfied positive is displayed in cell M4.

At the default costs of €50,000 per false negative error and €500 per false positive error, the minimum cost per event is €119.90, and the optimal threshold for positive classification is 16551.930.

##To Do

Try changing the inputs yourself. If you keep the cost per False Negative (FN) the same, but raise the cost per False Positive, would you in general expect the new optimum threshold to be higher (fewer total positive classifications) or lower (more total positive classficiations)?

- Change the cost per False Positive (FP) to  $1500 and you wll see that the optimum threshold is higher. It moves from 16551.930 to 16824.137.
- Reset the cost per FP to $500 and raise the cost per FN to $500,000, the optimum threshold drops to 13307.537


##Answer the following questions:

Change the cost per FN to $20,000 and change the cost per FP to $1,000

- What is the new minimum cost per event/cost per test (rounded to the nearest dollar)?
- What is the lowest level of protein that should be classified "Positive" to achieve the minimum cost per test at the new cost per error given the above?
- Can a change in classification threshold change a diagnostic test's True Positive Rate? Use logic - no need to calculate any numbers.
- "Condition Incidence" is the portion of a population that has the condition being studied. Can a change in the threshold change the condition incidence? Use logic.
- Does the change in threshold change the test's Area under the ROC curve? Use logic.
 


 This work is to be submitted to Moodle