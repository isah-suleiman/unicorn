# **Unicorn Companies: A Data Analysis**

### **Introduction**
This project explores what makes a company a unicorn—a privately held startup valued at $1 billion or more. Unicorns are rare and extraordinary, characterized by:
- **High Valuation**: Achieving a valuation of $1 billion or more while remaining private.  
- **Innovative Products and Services**: Disrupting industries with cutting-edge solutions.  
- **Rapid Growth**: Scaling operations at an exceptional pace.  
- **Venture Capital Investment**: Attracting significant funding from investors.  
- **Technology Focus**: Leveraging technology to drive growth and innovation.

![cover](images/unicorn_cover.jpg)

### **Disclaimer**  

The dataset used for this analysis was sourced from publicly available information and third-party platforms, such as Crunchbase or CB Insights. While every effort was made to ensure the accuracy and completeness of the data, it may contain inaccuracies, outdated information, or missing values.  

This project is intended for educational and exploratory purposes only. The insights and conclusions derived from the analysis should not be used for investment decisions or business strategies without further validation from authoritative sources.  

The analysis does not guarantee the comprehensiveness or representativeness of the dataset, as it may not include all unicorn companies globally or reflect the latest updates in the startup ecosystem.

---

### **Problem Statement**
1. **Number of companies by industry**: Which industries dominate the unicorn landscape?  
2. **Time to Unicorn Status**: How long does it typically take for a startup to achieve unicorn status?  
3. **Funding vs. Valuation**: How much funding do unicorns receive, and how does it compare to their valuations?  
4. **Yearly Growth**: How many companies achieved unicorn status each year?  
5. **Top Industries**: Which industry has the most unicorns?  
6. **Geographic Distribution**: What continents are home to the majority of unicorns?  
7. **Value Over Time**: How has the valuation of individual companies evolved over time?  
8. **Timeline to Unicorn**: How many months did it take companies to reach unicorn status?  

### **Tools and Technology Stack**
- **Power BI**: 
  - **Data Transformation and Modeling**: Cleaned and prepared the dataset for analysis.  
  - **Measures and Calculated Columns**: Created custom metrics to derive meaningful insights.  
  - **Visualizations**: Designed interactive dashboards to display findings effectively.  

---

### **Data Model Description**

The data model for the unicorn companies project is composed of three main tables:

1. **Unicorn_Companies Table**  
   - This is the primary table containing key information about each unicorn company, including:
     - **City, Country, and Continent**: Geographic details of each company.
     - **Company**: Name of each unicorn company.
     - **Date Joined**: The date each company achieved unicorn status.
     - **Industry**: The industry each company operates in.
     - **Funding**: Total funding received by each company.
     - **New Funding**: Additional calculated field for specific analysis needs.
     - **Date Difference**: Likely a calculated measure showing the time taken for each company to achieve unicorn status, derived from the date joined and possibly a company founding date.

2. **Date Table**  
   - This is a standard date dimension table used to support time-based analysis.
   - Key fields include:
     - **Date**: The individual dates.
     - **MonthName** and **MonthNumber**: Names and numbers of months to support sorting and filtering by month.
     - **Year**: Year for grouping by year in the analysis.

3. **Measures Table**  
   - This table is dedicated to storing custom measures created for the analysis, such as aggregations, percentages, or calculated metrics related to funding or growth rates.
   - The single column placeholder "Column1" implies that measures are being created here without additional columns or fields.

### **Relationships**
The primary relationship is between the **Unicorn_Companies** table and the **Date Table** on the **Date Joined** field, which allows for time-based analysis, such as tracking the growth of unicorn companies over time, comparing funding amounts by year, or analyzing trends by month.

### **Visualizations**

I created this Power BI dashboard to visualize the insights I discovered

![Row count check](assets/images/Unicorn_page-0001.jpg)

---
![Row count check](assets/images/thank-you.png)
