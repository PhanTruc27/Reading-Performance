# EDA Notes – Reading Performance Dataset

First, the dataset was checked for missing values and duplicated rows.
No NaN values or duplicate records were found, so the data was complete and clean at the initial stage.

Next, all columns were reviewed to make sure their data types were correct.
Numeric, categorical, and ordinal variables were all properly defined, and no type mismatches were detected.

Basic descriptive statistics were then examined.
All values fell within reasonable ranges, and there were no negative values in variables where they would be illogical (such as reading time or pages read).

Each column was also inspected individually to ensure that the values made sense in the context of reading behavior.
No abnormal or unrealistic values were observed.

After that, the distributions of continuous variables were analyzed.
Several variables showed noticeable skewness, especially mental break duration, reading time, and number of pages read.
To address this issue, log transformations were applied to these three variables in order to reduce skewness and improve their distributions.

Ordinal variables were encoded by assigning numerical orders that reflect their natural ranking (for example, from low to high).
This allows them to be used in correlation analysis while still preserving their ordinal meaning.

Once the log-transformed variables were created, the original versions of those columns were removed to avoid redundancy and multicollinearity.

A correlation matrix was then computed and visualized to explore relationships between reading performance metrics and other related factors.

Finally, a general logic check was performed to ensure that the observed patterns and relationships were consistent with realistic reading behavior.
Overall, the dataset appears coherent, well-structured, and ready for further analysis or modeling.
