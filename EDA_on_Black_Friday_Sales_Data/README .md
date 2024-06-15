
# Exploring Black Friday Sales: A Basic EDA

Description:

This repository contains a basic exploratory data analysis (EDA) of Black Friday sales data. The analysis is conducted using Python programming language and popular data analysis libraries such as Pandas, NumPy, Matplotlib, and Seaborn.

The EDA process begins with analyzing the raw data provided for Black Friday sales, followed by installing necessary libraries using pip. The CSV file containing the Black Friday sales data is then read into a Pandas DataFrame for further analysis.

Various aspects of the dataset are explored, including the total number of rows and columns, identification of missing values, and handling of missing values. Columns with significant missing values, such as 'Product_Category_2' and 'Product_Category_3', are removed from the DataFrame to ensure data integrity.

The analysis then delves into exploring different columns of the dataset, such as 'Gender', 'Age', 'Occupation', 'City_Category', 'Marital_Status', and 'Product_Category'. Visualizations such as bar plots, pie charts, and count plots are utilized to gain insights into the distribution and trends within these columns.

Furthermore, multi-column analysis is performed to uncover relationships between different variables. Visualizations are used to explore relationships between variables such as 'Age' and 'Gender', 'City_Category' and 'Purchase', 'Stay_In_Current_City_Years' and 'Gender', among others.

The readme.md file provides a comprehensive overview of the analysis process and findings, along with instructions for replicating the analysis. It also includes information on the dataset, libraries used, and how to contribute to the project.



## Acknowledgements

I would like to express our gratitude to the following individuals and organizations for their contributions and support:

- Kaggle: For providing the Black Friday sales dataset, which made this analysis possible. The dataset can be found here.
- Pandas Development Team: For creating and maintaining the Pandas library, which played a crucial role in data manipulation and analysis.
- NumPy Development Team: For developing the NumPy library, which facilitated efficient numerical computations.
- Matplotlib and Seaborn Developers: For creating powerful visualization libraries that helped in visualizing the data and gaining insights.
- The Python Community: For their continuous contributions to the open-source ecosystem, making tools and resources available to the data science community.

Finally, I extend our heartfelt thanks to all data scientists and analysts who continuously share their knowledge and expertise, contributing to the growth and development of the data science field.


## API Reference

#### Get all items
#### Pandas : pd.read_csv()

```http
GET /api/items
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `filepath_or_buffer` | `string` | **Required**. Path or URL of the CSV file|

#### Pandas : DataFrame.head()

```http
GET /api/items/${id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `n` | `int` | Number of rows to return. Default is 5|

#### Pandas : DataFrame.info()

```http
GET /api/items/${id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
|  |   |Provides a summary of the DataFrame|

#### Pandas :DataFrame.describe()

```http
GET /api/items/${id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
|  |   |Generates descriptive statistics|

#### NumPy : np.array()

```http
GET /api/items
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| object | array-like  |**Required**  Input data    |
		
#### NumPy : np.mean()

```http
GET /api/items/${id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| axis| int |Axis along which the means are computed |        

#### Matplotlib : plt.figure()

```http
GET /api/items/
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| figsize| tuple |Size of the figure (width, height) |  

#### Matplotlib : plt.plot()

```http
GET /api/items/${id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| x| array-like |X-axis values |  
| y| array-like |Y-axis values | 

#### Seaborn : sns.barplot()

```http
GET /api/items
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| x   | string |Name of variable in data for x-axis |  
| y   | string |Name of variable in data for y-axis | 

#### Seaborn : sns.histplot()

```http
GET /api/items/${id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| data   | DataFrame |Data to plot |  
 
		




## Appendix

#### Here's an overview of the project structure to help you navigate the files and directories
```http

project_root/
├── data/
│   ├── raw/                # Raw data files
│   ├── processed/          # Processed data files
├── notebooks/              # Jupyter notebooks for data analysis
├── scripts/                # Python scripts for data processing
├── reports/                # Generated reports
│   ├── figures/            # Figures and plots
├── README.md               # Project description and setup instructions
├── requirements.txt        # Python package dependencies



```

#### Further Reading and References

```http

- Pandas Documentation: https://pandas.pydata.org/pandas-docs/stable/
- NumPy Documentation: https://numpy.org/doc/stable/
- Matplotlib Documentation: https://matplotlib.org/stable/contents.html
- Seaborn Documentation: https://seaborn.pydata.org/
- Scikit-learn Documentation: https://scikit-learn.org/stable/

```


## Authors

- [Shubham Saxena](https://github.com/Shubham-Saxena-16)

## Badges

Add badges from somewhere like: [shields.io](https://shields.io/)

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)

## Deployment

To deploy this project run,follow these steps:

####1. Clone the Repository:

```bash
  git clone https://github.com/Shubham-Saxena-16/datafluency.git
```
####2. Navigate to the Project Directory:

```bash
 cd datafluency/EDA_on_Black_Friday_Sales_Data
```

####3.Install Dependencies:

```bash
 pip install -r requirements.txt
```

####4. Run the Application:

```bash
 python main.py
```

####5. Access the Application:

- Once the application is running, open your web browser and go to http://localhost:5000 to access the application.

## FAQ

#### Question 1 : What is this project about?

Answer 1 : WThe project aims to perform Exploratory Data Analysis (EDA) on Black Friday sales data to uncover insights and patterns in consumer behavior during this shopping event.

#### Question 2 : What tools or libraries are used for analysis?

Answer 2: The analysis is conducted using Python programming language and various libraries such as Pandas, Matplotlib, and Seaborn for data manipulation and visualization.

#### Question 3 :What insights can be gained from the analysis?

Answer 3: The analysis provides insights into various aspects of Black Friday sales, including popular products, customer demographics, sales trends over time, and correlations between different variables.

#### Question 4 :Is the dataset provided with the project?

Answer 4: Yes, the project includes the Black Friday sales dataset for analysis. However, users can also use their own dataset by replacing the provided one.

#### Question 5 :How can I contribute to the project?

Answer 5: Contributions to the project are welcome. You can contribute by adding new features, improving existing code, fixing bugs, or suggesting enhancements. Simply fork the repository, make your changes, and submit a pull request.


## Features

Here are some key features of the project:

- Data Loading: The project provides functionality to load the Black Friday sales dataset into memory for analysis.

- Exploratory Data Analysis (EDA): It performs comprehensive EDA on the dataset, including summary statistics, data visualization, and identifying patterns and trends.

- Data Visualization: Utilizes various plotting libraries such as Matplotlib and Seaborn to create informative visualizations, including histograms, bar plots, and heatmaps.

- Customer Segmentation: The project includes functionality to segment customers based on their purchasing behavior, demographics, and other attributes.

- Product Analysis: Analyzes product categories, sales volumes, and popular items during the Black Friday sales event.

- Correlation Analysis: Identifies correlations between different variables such as age, gender, occupation, and purchase amounts.

- Insights Generation: Generates actionable insights and conclusions from the analysis, providing valuable information for businesses and marketers.

- Customization: Users can customize the analysis by adding or removing features, modifying plotting styles, and exploring different aspects of the dataset.

These features collectively provide a comprehensive understanding of Black Friday sales data and help in making data-driven decisions for businesses and retailers.
## 🚀 About Me
I'm Shubham Saxena, a performance analyst specializing in web technologies and data analysis. With a background in computer science, I excel in optimizing systems and processes to enhance performance and efficiency. I'm passionate about leveraging data-driven insights to drive strategic decisions and improve outcomes. Let's connect on LinkedIn to explore potential collaborations!

