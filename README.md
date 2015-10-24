# GettingandCleaningDataProject
In Step 1, we read each table of data into R without headers.  We then created three new data tables by row-binding each similar table (i.e. all subject tables, all activity tables, and all feature tables).  We then re-named the columns of the combined tables, and column-binded the master subject table, master activity table, and master feature table into one tidy-data table.

In Step 2, we used column bind to extract only columns containing mean and standard deviation data and added it to a new data table called "extractmeansd".

In Step 3, we assigned label values to each value in the activity column, using the activity_labels.txt table.  We matched the activity number with the corresponding label and appended the activity labels to both the tidy data set and the extractmeansd data set.

Step 4 simply required us to rename the data sets using the names() operation in R.

In Step 5, we aggregated the renamed subject and activity tables with the extracted mean and standard deviation values from step 2 to create the table titled "final."  Using the write.table() operation in R, we created a .txt file of the "final" data table.
