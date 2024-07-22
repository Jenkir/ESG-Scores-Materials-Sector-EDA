# Exploratory Data Analysis of ESG scores 
## For companies in the "Materials" sector
See the "Materials.ipynb" file for an exploratory data analysis (EDA) of ESG scores &amp; stock market data for companies in the Materials sector.
 
![heatmap2](https://github.com/user-attachments/assets/4d5c712e-3a53-4c5e-bb05-88df91f9851c)



When comparing ESG scores of different companies, it's important to compare a company against its peers in the same sector or industry. One framework used for classifying companies is the Global Industry Classification Standard (GICS) which includes 11 overarching sectors, and then further narrows down the classfication to 25 industry groups, 74 industries, and then into 163 subindustries. The way that a company is classified primarily depends on its main revenue source.

Each industry has different material issues that are the most pertinent to how it conducts business as well as the most important to stakeholders. ESG metrics will vary depending on what a company considers its material issues to be. Each industry or sector will have similar material issues. For example, the material issues of a bank (Financial sector) will be different than that of a company that produces cleaning products (Consumer Staples sector). A bank will track different ESG metrics than a cleaning products company although some metrics will be the same (such as how the board of directors is governed).

In this project, we explore the ESG ratings of companies in the GICS 'Materials' sector. The data was primarily pulled from [ESGAnalytics.io[(https://www.esganalytics.io/), Finazon.io, and Yahoo Finance APIs. ESG Analytics extracts over 1 million data points per month to "to deliver a third-party perspective on company ESG performance." Using AI, they generate ESG scores based on unstructured text from media stories, press releases, and other publicly available information. They provide data for over 10,000 companies (mostly public and some private). Finazon is a "marketplace for global financial data APIs "providing real-time stock market data." Yahoo Finance is well-known as a source of up-to-date stock and financial information.

This project also includes ESG scores from other ratings providers such as Sustainalytics, S&P Global, and MSCI. Each of the providers compiles data and scores companies differently. Normalized scores are provided (by ESGAnalytics) to make comparing companies' scores easier. 
For more details about providers' ESG ratings processes, see https://cherrytreelaneanalytics.io/help-and-faqs/how-to-compare-scores/

### FAQs
**What is considered a "good" score?**

ESGAnalytics (dataset column is named "ESG_AI_score"): ranges from -1.0 to 1.0 with 1.0 being the "best" score possible
MSCI: ranges from CCC to AAA with AAA being the "best" score possible
S&P Global (dataset column is named "SNP"): ranges from 0 to 100 with 100 being the "best" score possible
Sustainalytics: ranges from 0-40 BUT the LOWER the score, the better (lower means less risk for investors)

**When was the data extracted?**

The stock market data was extracted the last week of June 2024 from Finazon.io and Yahoo Finance. 
The company details (address, etc.) were extracted from ESGAnalytics.io and Yahoo Finance the last week of June 2024.
The ESG ratings were extracted for the year 2023. Most providers update ESG ratings for companies once per year unless there is a drastic development.

The EDA for this project includes discovering the mean and median ESG scores for companies in this sector, which subindustries are included in this sector (such as Industrial Machinery, Trucking, and Commercial Printing), the frequency of ESG ratings for companies in this sector, and which companies in the trucking subindustry have the highest and lowest scores.

**Is there a data dictionary available?**
