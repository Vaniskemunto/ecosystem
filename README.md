
## ANALYSIS OF FUNDING FOR INDIAN STARTUP ECOSYSTEM

Welcome to my project, “Exploring Trends in the Indian Startup Funding Ecosystem.” Here, I delve deep into the Indian startup landscape, conducting a thorough analysis of data spanning from 2019 to 2021. India recently celebrated the 7th anniversary of the startup India initiative,and the release of the National Startup Report 2022 has brought to light a staggering growth and remarkable achievements in the country's startup ecosystem over the past seven years (2015-2022). The report showcases a 7x increase in the number of incubators, a 9x increase in the number of investors, and an impressive 15x increase in the total funding for startups.
With over 1,17,000 startups, the country has witnessed an exponential growth in entrepreneurship. These startups are not confined to metropolitan areas, as the report indicates their presence in 670+ districts, with 50% of them originating from Tier-2 and Tier-3 cities
Leveraging the power of Python and data visualization through Power BI, as a data analyst in this venture, aspire to uncover captivating trends within the expansive funding landscape of Indian startups. Join me on this exploration as we unravel the story behind the numbers, shedding light on the intricate patterns that have shaped the financial journey of startups in India during this critical period.


 SETUP

Getting started -->
Create a remote Github repository
https://github.com/Vaniskemunto/ecosystem/blob/main/ecosystem.ipynb

Clone the remote repository to the local 

Create a virtual environment<python -m venv env>

Activate the virtual environment
 <env/Scripts/activate>
 
Install the necessary packages


DATA SOURCES

The Indian startup ecosystem has four data sources for the different four years.In these datasets there is startup's details, the funding amount received and the investor's information. The data sources are as follows:
2018: The 2018 dataset is stored in the Git repository 'https://raw.github.com/Azubi-Africa/Career_Accelerator_LP1-Data_Analysis/main/startup_funding2018.csv'

2019: For the 2019 dataset it was retrieved from one drive 'C:/Users/KEMUNTO/Downloads/startup_funding2019.csv'

2020 & 2021 : These two year periods have their datasets stored in the database. The database management system for the two datasets is Microsoft SQL SERVER. To access the database you can use open database connecting standard library pyodbc.The tabels are named as follows:
Table1: dbo.LP1_startup_funding2020
Table2: dbo.LP1_startup_funding2021


CODE STRUCTURE

We start by connecting to all datasets separately we begin with the 2020 ,2021 ,2019 then the 2018 dataset .

Next we make data connections using the pyodbc library for the 2021& 2020 datasats .We visualize on the data info to understand the datatype of the data sets then visualize the missing values The following datasats have the following characteristics which are cleaned with the function used:

The 2018 DataFrame:

• The DataFrame has 526 rows and 6 columns.
• Dashes were used in the amounts column for deals whose values were not known.
• The amounts in the 2018 DataFrame are a mix of Indian Rupees (INR) and US Dollars (USD), meaning they have to be converted into the same currency.
• The industry and location columns have multiple information.

The 2019 DataFrame:

• The DataFrame has 89 rows and 9 columns.
• The data type of the “Founded” column is set to float64. It should be set to a integer for uniformity.
• The headquarter column has multiple information. 

The 2020 DataFrame:

• There is an extra column called “column10”, giving it a total of 10 columns. It should be dropped to ensure complete alignme
nt with the other DataFrames for ease of concatenation.

The 2021 DataFrame:

• The data type of the “Founded” column is set to float64. It should be set to a integer for uniformity.
The undisclosed values also have to be deleted and the 2018 dataframe had the Founders and the Investors colums missing which have to be filled with n/a

 🙏ACKNOWLEDGEMENTS

I acknowledge my project team contributors the Azubi Africa tutors &trainers and all the free available resource made available online


 📝LICENSE

 This project is [MIT](./LICENSE) licensed.




AUTHORS

🕵🏽‍♀️ **Vanis Kemunto Makori**

- GitHub: [GitHub Profile](https://github.com/Vaniskemunto)
- Twitter: [Twitter Handle](https://twitter.com/Vanis Kemunto)
- LinkedIn: [LinkedIn Profile](https://www.linkedin.com/in/vanis-kemunto-b05974146/)

