# analysis_of_Moscows_foodservice_market

**PROJECT DESCRIPTION**

**Client:** "Shut Up and Take My Money" investment fund, which plans to open a foodservice establishment in Moscow.

**Research Objective:** To study the market in Moscow, identify interesting features, and present the findings that will assist in selecting a suitable location for potential investors.

**Research Tasks:**
 - Study the data and perform data preprocessing.
 - Analyze Moscow's foodservice market, identify patterns, and draw conclusions.
 - Conduct a detailed analysis of coffee shops and assess the feasibility of opening a coffee shop in Moscow.
 - Prepare a presentation for the client.

**Data Description**

For the research, a dataset of foodservice establishments in Moscow is provided. The dataset was compiled based on data from Yandex Maps and Yandex Business services, collected in the summer of 2022.

**File: moscow_places.csv:**
- name: the name of the establishment.
- address: the address of the establishment.
- category: the category of the establishment, such as "cafe," "pizza place," or "coffee shop."
- hours: information about the days and hours of operation.
- lat: latitude of the geographical location of the establishment.
- lng: longitude of the geographical location of the establishment.
- rating: the establishment's rating based on user reviews in Yandex Maps (highest rating is 5.0).
- price: price category of the establishment, such as "average," "below average," "above average," and so on.
- avg_bill: a string that represents the average order cost in a range format, for example:
     1. "Average bill: 1000–1500 ₽";
     2. "Price of a cup of cappuccino: 130–220 ₽";
     3. "Price of a beer glass: 400–600 ₽"
- middle_avg_bill: a number indicating the estimated average bill, which is only specified for values in the avg_bill column that start with the substring "Average bill."
If a price range of two values is given in the string, the column will contain the median of those two values.
If a single number is given in the string (without a range), that number will be entered in the column.
If there is no value or it doesn't start with the substring "Average bill," the column will be empty.
 - middle_coffee_cup: a number indicating the estimated price of a single cup of cappuccino, which is only specified for values in the avg_bill column that start with the substring "Price of a cup of cappuccino."
If a price range of two values is given in the string, the column will contain the median of those two values.
If a single number is given in the string (without a range), that number will be entered in the column.
If there is no value or it doesn't start with the substring "Price of a cup of cappuccino," the column will be empty.
- chain: a binary value (0 or 1) indicating whether the establishment is part of a chain (there may be errors for small chains):
0: the establishment is not part of a chain.
1: the establishment is part of a chain.
- district: the administrative district where the establishment is located, such as the Central Administrative District.
- seats: the number of seats available.
