# WebScraping
## 1. ETL with Python
Creating a dataframe to analyze from a XML file. 
From the OptaF24.xml file stored on an FTP server, which contains the events of a specific match, we need to create a dataframe containing all the passes made during that match.

To achieve this, we would typically follow these steps:

Retrieve the XML file from the FTP server: Use FTP client libraries or tools to download the OptaF24.xml file from the FTP server to your local environment or directly into your programming environment.

Parse the XML data: Use an XML parsing library (e.g., BeautifulSoup in Python) to parse the XML file and extract relevant information, such as events with type_id="1" (passes).

Extract pass data: Iterate through the parsed XML data to extract pass events along with their attributes (period_id, min, sec, outcome, x, y) and any relevant qualifiers (qualifier_id="140" and qualifier_id="141").

Create a dataframe: Use a dataframe library (e.g., Pandas in Python) to organize the extracted pass data into a structured dataframe.

Filter data: Filter out any unnecessary information and focus solely on pass events.

Visualize or analyze the dataframe: Once the dataframe is created, you can visualize it, perform analysis, or further manipulate the data as needed.

## Scraping financial data

Implementing a Python script to extract via Web Scraping the total investment value, calculated as:

TOTAL VALUE = ∑ fund x shares

BlackRock Global Funds - Euro Short Duration Bond Fund A2 EUR: https://www.morningstar.es/es/funds/snapshot/snapshot.aspx?id=F0GBR04AS2 iShares Europe Equity Index Fund (LU) A2 EUR: https://www.morningstar.es/es/funds/snapshot/snapshot.aspx?id=F00000OYMI iShares Euro Government Bond Index Fund (LU) A2 EUR: https://www.morningstar.es/es/funds/snapshot/snapshot.aspx?id=F00000OYMY
