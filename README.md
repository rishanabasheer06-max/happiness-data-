📊 Data Analysis using Histograms

# Data source:https://drive.google.com/file/d/1Fxf8Wo4jccGiZO_VKpRj8_QZcrGTcMKE/view?usp=classroom_web&authuser=0

📌 Project Overview
This project focuses on analyzing numerical data using histograms. Histograms help to understand the distribution, spread, and patterns of different variables in the dataset.

📂 Dataset
The dataset contains multiple numerical features such as:

GDP per Capita

Life Expectancy

Social Support

Happiness Score

Freedom

Generosity

Dystopia + Residual

🛠️ Tools Used
Python

Pandas

Seaborn

Matplotlib

📈 Methodology
Selected all numerical columns from the dataset

Used histogram plots to visualize distributions

Applied KDE (Kernel Density Estimation) for smooth curves

Analyzed shape, spread, and outliers

🔍 Key Insights
GDP shows high inequality with a right-skewed distribution

Life expectancy is mostly consistent across countries

Social support values are closely grouped

Happiness scores are normally distributed

Some variables show outliers indicating extreme values

📊 Visualization Code
import seaborn as sns
import matplotlib.pyplot as plt

for col in df.select_dtypes(include='number'):
    plt.figure(figsize=(5,4))
    
    sns.histplot(
        data=df,
        x=col,
        bins=20,
        color="purple",
        kde=True
    )
    
    plt.title(col)
    plt.show()
✅ Conclusion
Histograms provide a clear understanding of data distribution. This analysis helps identify patterns, variation, and outliers across different features.

