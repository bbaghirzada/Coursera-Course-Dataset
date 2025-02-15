# COURSERA DATA EDA ANALYSIS Using Pandas and Visualization with python libraris
---
### Overview

The dataset is sourced from Kaggle, specifically focusing on Coursera course listings.
It contains structured data on various online courses offered on the Coursera platform.

> This dataset contains mainly 6 columns and 890 course data. The detailed description:

    course_title : Contains the course title.
    course_organization : It tells which organization is conducting the courses.
    course_Certificate_type : It has details about what are the different certifications available in courses.
    course_rating : It has the ratings associated with each course.
    course_difficulty : It tells about how difficult or what is the level of the course.
    course_students_enrolled : It has the number of students that are enrolled in the course.

---

    > WHAT Questions asked before starting the analysis?
* What is this data telling about?
* What universities has the highest number of courses?
* Is that having the highest number of courses means you have the highest average rate?
* What are the student enrollment division between certification types? How the average rating changes based on these types?
* What are difficulty levels of the certification types? and how is the divison of enrollment between those difficulty levels?
* And lastly correllation between numbers to find are they actually influence each other?

## Data Analysis Process and Setting the environment
1. First Python Jupyter environment set up
2. All necessary libraris such as

```python 
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px
import plotly.graph_objects as go


from scipy.stats.mstats import winsorize
%matplotlib inline

```
### The data downloaded as a zip file attached and accessed using pandas

```python
df = pd.read_csv("/Users/boryabaghir/Downloads/coursea_data.csv", index_col=0)
df

```

3. The Data Analysis started with checking and handling the missing and duplicate values
```python 
df.info() 
df.isna().sum()
df.duplicated()
```

4. Handling Outliers
5. and EDA with plotyly and pyplot started
6. Some Internal Markdown languages used for the explanation of the visualizations and code.

---

**Data Visualization**

To illustrate the findings, the following charts were used:

* Bar Charts: Course distribution by difficulty level.
* Histograms: Rating distributions.
* Scatter Plots: Relationship between enrollment and rating.
* Pie Charts: Share of courses by organization.

Tools & Technologies Used

* Python: Data analysis & manipulation.
* Pandas: Data cleaning and transformation.
* Matplotlib & Seaborn: Data visualization.

Conclusion

This analysis provided key insights into Coursera courses, helping to understand what factors influence student engagement and course popularity. The findings can be useful for content creators, education providers, and learners looking for high-rated courses.
