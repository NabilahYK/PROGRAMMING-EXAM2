# PROGRAMMING-EXAM2
Programming exam 2, freeform
https://www.ons.gov.uk/peoplepopulationandcommunity/healthandsocialcare/mentalhealth/datasets/costoflivinganddepressioninadultsgreatbritain
i chose this data from the gov.uk website and found it through google data search
the excel file presents variant factors that could lead to depression and presents them as a percentage 
i first imported my drive and imported modules as i went along
i imported the modules:
pandas
seaborn 
matplotlib pyplot
plotlyexpress
from scipy.stats import f_oneway


i placed the file into a variable
i first used one sheet from the entire excel file
every sheet had data summary and clerical notes, i pulled each table as needed through skip row and pandas
i checked the shape, info of the sheets
i checked the null values
i filled in the null values
i confirmed at each step
i renamed messacy columns using pandas ans renamed
i reset index as needed to plot, i used set index to set the index as year alwaysand always used inplace=TRue as to not create too many variables
i dropped any duplicate columns
i dreopped rows named 'no or mild symptoms' because it was uneeded, using percentages shows the difference already and when comparing in analysis, it is not needed
i also changed floats to integeres using apply round and as commands so the values were able to be used in plotting
i added a year column to show timelines
df7, my first plot showed depressive symptoms with mupltple variables, all, persons, ages, gender and disability and country, this gives a goood oversight and is in solid colors to show intial analysis
i then pulled data with each factor and experimented the best visual
i decided to create a chloropleth map for england scotland wales
i tried to make it animated
i created stacking faceted bars and deemed then unsuitable
i also creaed a box plot to show variaton
i created a parellel coordinates plot to show movement over the years and ages
i created bar charts for gender, disability, region, educational status and home owndership
i decided to create a heatmap to enphasise disability 
to highlight the sheer difference in disabled vs non disbaled depression symptoms, i used mann whitney u then added a t test
i could not present my dataframe directly into the code so i had to create another
the tests showed a small p value indicating the sheer difference
i then decided to do an anova test
i had to import 'from scipy.stats import f_oneway' 
i used the website geeksforgeeks to navigate how to do this as a reference
again i decided to create a whole new dataframe 
this time i was viewing the changes across the year
for men  and women, i couldnt disprove the null hypothesis of any significant change over the years

