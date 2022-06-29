# Installation and Usage Instructions
1. Move the MSC_Data folder to any desired location. Right click on the folder icon and copy the path, then open "MSCAutoFrame" and in the box next to "Folder Destination", paste the path and add a "/" to the end.

2. In the box next to "Factor Range", input the magnitude of your factor value. Upon data extraction, if any (replicate value / existing value) is greater than the factor value or less than 1/factor value, the compound is flagged with a red highlight and the index of the compound is placed beneath "Flagged Compound Indices". The factor value is also used when a third replicate value for an existing replicate set is added; if the new value is more orders of magnitude away from both values than either value is from one another, the new value is thrown out, and the index of the compound is placed beneath the "New Values Verification Indices". Otherwise, whichever replicate is farther away is thrown out (If requested, can remove cap for replicate numbers so that all replicate values that aren't thrown out are appended to the compound).

3. Format all files so that the first 8 digits in the filename represent the date (i.e. 06042022), and drag all files for extraction inside the MSC_Data directory. Create a folder named "Analyzed Files" in the MSC_Data folder; this will be where all Excel files wll be stored after data extraction.

4. Click the "Extract Data" button to extract all MSC data from the files into the spreadsheet. All files that have had data extracted are moved into the "Analyzed Files" Folder. MSC Compounds with empty AC50 values are highlighted in blue, flagged compounds are highlighted in red. 
 
5. To sort the data from AC50 values least to greatest, click the "Sort AC50" button.
 
6. All verified values that are thrown out and old values that are replaced are moved to a section starting at Column Index O at the same row indice of the MSC Compound ID. The total number of tests per compound is listed in the "# Tests for Compound" column.
 
7. If there are any problems with the macro, or you have any questions, contact me at defrondeville.c@northeastern.edu or 1-617-710-6138.

# Auto2Frame

Auto2Frame functions the same way as the automatic dataframe, except instead of handling AC50 and efficacy values, it handles % effect values, and does not account for replicates. Comes with a macro that automatically generates a waterfall plot of the data.
