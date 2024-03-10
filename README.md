
# ANALYSIS OF FUNDING FOR INDIAN STARTUP ECOSYSTEM

Welcome to my project, “Exploring Trends in the Indian Startup Funding Ecosystem.” Here, I delve deep into the Indian startup landscape, conducting a thorough analysis of data spanning from 2019 to 2021. India recently celebrated the 7th anniversary of the startup India initiative,and the release of the National Startup Report 2022 has brought to light a staggering growth and remarkable achievements in the country's startup ecosystem over the past seven years (2015-2022). The report showcases a 7x increase in the number of incubators, a 9x increase in the number of investors, and an impressive 15x increase in the total funding for startups.
With over 1,17,000 startups, the country has witnessed an exponential growth in entrepreneurship. These startups are not confined to metropolitan areas, as the report indicates their presence in 670+ districts, with 50% of them originating from Tier-2 and Tier-3 cities
Leveraging the power of Python and data visualization through Power BI, as a data analyst in this venture, aspire to uncover captivating trends within the expansive funding landscape of Indian startups. Join me on this exploration as we unravel the story behind the numbers, shedding light on the intricate patterns that have shaped the financial journey of startups in India during this critical period.


Installation

1. Clone the remote repository:
git clone https://github.com/Vaniskemunto/ecosystem/tree/main
2. Navigate to the project directory.
3. Set up a woking environment on Visual Studio code
4. Install libraries 
```
    
Data Sources
The Indian startup ecosystem has four data sources for the different four years.In these datasets there is startup's details, the funding amount received and the investor's information. The data sources are as follows:
2018: The 2018 dataset is stored in the Git repository 'https://raw.github.com/Azubi-Africa/Career_Accelerator_LP1-Data_Analysis/main/startup_funding2018.csv'

2019: For the 2019 dataset it was retrieved from one drive 'C:/Users/KEMUNTO/Downloads/startup_funding2019.csv'

2020 & 2021 : These two year periods have their datasets stored in the database. The database management system for the two datasets is Microsoft SQL SERVER. To access the database you can use open database connecting standard library pyodbc.The tabels are named as follows:
Table1: dbo.LP1_startup_funding2020
Table2: dbo.LP1_startup_funding2021
Code Structure
We start by connecting to all datasets separately we begin with the 2020 ,2021 ,2019 then the 2018 dataset .
We then import the necessary library packages. The individual datasets are then loaded as Pandas DataFrames. The datasets have different shapes i.e. columns and rows.
Next we make data connections using the pyodbc library for the 2021& 2020 datasats .We visualize on the data info to understand the datatype of the data sets then visualize the missing values The following datasats have the following characteristics which are cleaned with the function used:
The 2018 DataFrame:
• The DataFrame has 526 rows and 6 columns.
• Dashes were used in the amounts column for deals whose values were not known.
• The amounts in the 2018 DataFrame are a mix of Indian Rupees (INR) and US Dollars (USD), meaning they have to be converted into the same currency.
• The industry and location columns have multiple information.

The 2019 DataFrame
• The DataFrame has 89 rows and 9 columns.
• The data type of the “Founded” column is set to float64. It should be set to a integer for uniformity.
• The headquarter column has multiple information. 

The 2020 DataFrame
• There is an extra column called “column10”, giving it a total of 10 columns. It should be dropped to ensure complete alignme
nt with the other DataFrames for ease of concatenation.

The 2021 DataFrame
• The data type of the “Founded” column is set to float64. It should be set to a integer for uniformity.
The undisclosed values also have to be deleted and the 2018 dataframe had the Founders and the Investors colums missing which have to be filled with n/a
Results& Evaluation
The project was focussed on answering a few questions:

Which year has the highest amount of investment?
It is noted that the year 2019 had the most amount of money invested.
Which sector received the highest amount of funding collectively?
The finance and the education sector received the highest amount of funding as compared to other sectors.
Which region has the most startups?
The top three regions that received the most investments were Bangalore, Mumbai and Gurugraham.



 Acknowledgements

I acknowledge my project team contributors the Azubi Africa tutors and trainers. 


 License

 For the github repository, the License used is MIT License.



