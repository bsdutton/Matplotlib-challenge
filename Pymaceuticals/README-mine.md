# Matplotlib-challenge

## Complete solutions are provided pymaceuticals-main.ipynb
  * Working file is pymaceuticals-working.ipynb

## I noticed in the data with this homework
  1) Each chart has different attributes that can be looked at to see how to proceed with further data analysis.
    * I found the bar charts created directly from the Pandas Groupby DataFrames much easier to generate.
    * There is much aid given with the filtering and indexing in these DataFrames.
  2) I spent much time trying to get more detail in the pie charts.  I felt it might be worthwhile knowing if the sex of the mice  had any relationship to the effectiveness of the drug regimen.
    * I tried to get pie charts that showed the percentage of female mice were used for each drug regimen.
    * I got the labels to show the percentage of female mice, but I could not get the size of the slices to reflect these percentages.
    * I think the exploded pie chart with the legend showing up at the "best" location had some effectiveness in showing this; but, when I tested how well this chart would look when exported, much more formatting would be required for what is shown in the Jupyter Notebook to show up well in a PNG or PDF.
    * I believe a donut pie chart would be a good representation of this data, but this was beyond the scope of the homework, and I am really far behind already.
  3) I think the simple straight-forward line chart as a timeline tells answers the question most would ask regarding the effectiveness of each drug regimen.
    * I think all 25 lines on one figure would be two busy.  Perhaps, 3 lines based on the max, min, and mean would be a good way to show the trend which would be reinforced with the linear regression on a scatter plot.
  4) I definitely learned it is very important how the data is filtered, indexed, and sliced when trying to put together the most effective charts.
  5) I initially thought the histogram on the drug Capomulin migh indicate some outlier because of the separation of the min and max from the rest of the data, but that did not prove to be when I did the boxplot for Capomulin.



## Some notes about my homework
  1) The way the homework was written was to drop the one mouse ID with duplicate information.  This would result in 248 mice.
    * However, I chose to look at where the data was duplicated; and, and I chose to remove the duplicate timepoints for that mouse ID, g989.
    * Afterall, I did not want that mouse to die in vain!
    * This does bring up a topic of interest.  Shouldn't the data be looked at for the duplicates first to see if there is still information that is useful?
  2) In the last section of the homework where we were trying to find outliers we were supposed to merge the Groupby DataFrame with the last timepoint for each Mouse ID with the original.
  	* I really looked at the results of the merge, and I kept getting NaN values.
  	* Perhaps, they were the result of me not indexing properly or me focusing on largest tumor instead of last timepoint.
  	* Regardless, I decided the original cleaned dataframe could be filtered in order to give me the proper results, and I think they look correct.
  	* But, how would I know? 
  	* Is this another aspect of Data Analytics?  To pick apart analysis done by others to see if it is correct or not?  Whether the correct assumptions were made?  Are there audits done in Data Analytics?   