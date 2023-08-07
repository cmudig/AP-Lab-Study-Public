# AutoProfiler Lab Study Materials
Dataset and materials used in AutoProfiler user study.

In our user study, participants used either [AutoProfiler](https://github.com/cmudig/AutoProfiler) or [InlineProfiler](https://github.com/cmudig/ProfileInline) to perform a data cleaning and analysis task.

## Dataset
For this task, they used a housing dataset included in [dataset_housing.csv](./dataset_housing.csv). This dataset is a sample of a larger dataset of rental prices in the bay area originally from [here](https://www.katepennington.org/data) with additional errors added. 

The below table contains a description of each of the errors and insights on our "rubric" of participant performance.
We include the percentage of participants that discovered each error/insight, noting that some discoveries were found far more often than others, and whether the error was found with our tool or the participant writing the code themselves.
The first 13 insights and errors were things we expected participants to discover ahead of time, and the last 3 were valid extra findings discovered by participants. 
Please see our paper for more details about dataset errors and participant performance.


| No. | Type | Category | Origin | Description |  Found | Found with tool |
| --- | ---- | -------- | ------ | ----------- |  ----- | --------------- |
| 1 | Missing  | Error | Inherent | Small number of missing values in county, beds, title | 56\% | 100\% |
| 2 | Missing  | Error | Inherent  | Mostly missing in baths, sqft, description | 56\% | 100\%|
| 3 | Inconsistent  | Error | Added | City has values that are lower and upper case | 69\% | 91\% |
| 4 | Inconsistent  | Error | Added  | Negative prices | 69\% | 100\% |
| 5 | Incorrect  | Error | Inherent  | Date could be parsed to DateTime format | 63\% | 90\%  |
| 6 | Incorrect  | Error | Added  | County has default values of "---" | 81\% | 85\%  |
| 7 | Incorrect  | Error | Added  | Sqft has string values and should be converted to an int | 69\% | 82\%  |
| 8 | Outliers | Error | Inherent | Outliers in sqft | 6\% | 100\%|
| 9 | Outliers  | Error | Inherent | Outliers in price | 44\% | 100\%|
| 10 | Schema   | Error | Added | Duplicate datapoints (duplicate post_ids) | 38\% | 100\%  |
| 11 | Distribution  | Insight | Inherent  | Room_in_apt is almost all 0 | 56\% | 100\% |
| 12 | Scope  | Insight | Inherent | Dataset is only apartments in California | 31\% | 100\%|
| 13 | Correlation  | Insight | Inherent | Inspect correlations between any variable and price | 13\% | 0\%|
| 14 | Distribution | Insight | Inherent | Data is not evenly distributed across years | 38\% | 100\% |
| 15 | Inconsistent | Error | Inherent | Year and date column correspond (ensure consistency) | 19\% | 67\% |
| 16 | Inconsistent | Error | Inherent | The price is not properly extracted from title for some rows | 6\% | 0\% |
    

## Task
The participants were first shown a demo of the system, and then given a notebook with instructions in [AP Lab Study - Dataset 1.ipynb](./AP%20Lab%20Study%20-%20Dataset%201.ipynb) to complete the task.

## Questions
For any questions about this dataset, task, or data please contact Will Epperson at [willepp@cmu.edu](mailto:willepp@cmu.edu).