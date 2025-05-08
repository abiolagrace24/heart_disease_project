# The Heart Disease Data Analysis

![image](https://github.com/user-attachments/assets/4bd30b41-9a29-4527-9394-3c59a39da82f)

I'm sharing another project to walk through my hands-on analysis of a real-world heart disease dataset using Python. I created this as part of my personal learning journey in data analysis and more importantly, to understand how data can help answer health-related questions.
I have worked on a dataset on heart disease. This problem helps us identify patterns and potential risk factors related to heart disease using visualizations and pandas operations. Which features (like age, cholesterol, chest pain, etc.) show the strongest differences between people with and without heart disease?


## The Problem Statement

Heart disease is a serious global issue — but what if we could identify key factors that indicate whether someone might be at risk? 

I started with a simple but impactful question:

> Which health measurements most clearly separate people who have heart disease from those who don’t?

The idea isn’t to build a prediction model (yet), but to understand the data, spot meaningful patterns, and visualize differences. This is what real data analysis is about — asking the right questions and letting the data tell the story.

## Tech Stack(Tools & Libraries)

I used:
- `pandas` for reading and exploring the data
- `matplotlib` and `seaborn` for visualizing trends and differences
- `Jupyter Notebook` to break the work down step-by-step

These are standard tools used by data analysts and data scientists for a reason — they’re reliable, easy to learn, and powerful enough to find real insights.

## Workflow and Justification

Here’s how I approached the problem, and why I chose each step:

### Load the data
I started by reading the `heart_data.csv` file using pandas. This gave me a table with patient info — things like age, cholesterol, chest pain type, and whether or not the person had heart disease (`target` column).

### Understand the structure
I used `df.info()` and `df.head()` to check for missing values, data types, and get an initial sense of what I'm working with. This helps prevent surprises later in the analysis.

### Check for missing data
Before analyzing anything, it’s essential to make sure the dataset is clean. I used `df.isnull().sum()` to confirm there were no gaps that might affect my visualizations.

### Explore the target variable
I used a count plot to see how many patients had heart disease (target = 1) and how many did not (target = 0). This told me whether the dataset is balanced or skewed.

### Compare age and cholesterol
Next, I visualized how age and cholesterol levels differ between those with and without heart disease. I used:
- `histplot()` for age (to see distributions)
- `boxplot()` for cholesterol (to show value spread and outliers)

These plots made it easy to visually spot trends like whether older people or those with high cholesterol are more likely to have the disease.

### Correlation heatmap
Finally, I used a correlation matrix to see which features move together. This helps identify strong relationships for example, if cholesterol and heart disease are correlated, we might explore that deeper in future work.

## Why This Approach Works

Instead of jumping straight into machine learning or modeling, I took a data-first approach. This lets me:
- Understand the shape and quality of the data
- Ask questions that help explain, not just predict
- Use visualization to communicate insights clearly

In real-world analysis, this step is often the most important knowing why something happens is just as important as predicting that it will.

## Final Thoughts

This project isn't just about plotting graphs, it’s about learning how to think like an analyst. I’ve written every step intentionally so I can come back to it, build on it, and use it as a reference as I grow.

If you're a recruiter or someone reviewing this, I hope this shows that I care about clarity, curiosity, and continuous learning. Let’s connect if you want to chat more!


