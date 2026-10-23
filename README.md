# Restaurant-Market-Feasibility-Analysis-WIP-

## Background ## 

This project is an analysis of food prices in Metro Manila with a special focus from 2024 to 2026. This analysis is tailored to be a market feasibility analysis for a local restaurant in Metro Manila. To be specific, it will serve as a general outlook for stakeholders in order for them to determine which products, items, and dishes their restaurants can sell to consumers. The time period was chosen for this specific purpose; that is to provide an analysis of recent trends in food prices in the said region.

_Key Metric_
- Average Food Price in Philippine Peso Currency

### Metro Manila or the National Capital Region (NCR) ###

Metro Manila or NCR is the capital region of the Philippines. In spite of its name, the region is actually composed of multiple cities (including Manila) and one municipality. Metro Manila can be described as the heart of the country. Almost all economic and financial hubs in the Philippines are located in the region. It is also one of the most congested metropolises of the world, with millions of residents and non-residents alike located in the region.

Given this, Metro Manila as a market has special significance. Because of its status as a metropolis and with millions of citizens within, food prices in said region tend to be higher than provincial rates or other markets (see graph below). Such prices can also be volatile; economic, political, social, and environmental upheavals can immediately influence the local market.

While this analysis will focus from 2024-2026, stakeholders should be aware of the long-term outlook. As such, a brief overlook of Metro Manila’s market could be beneficial. 

<img width="1498" height="724" alt="Metro Manila vs  Other Markets - Yearly Avg" src="https://github.com/user-attachments/assets/c2164ebc-d4d0-4b3b-9aa5-ea653a757cd9" />

The chart above shows the annual average price of food in the region from 2000 to 2026. Inflation considered, Metro Manila’s annual average prices were steadily rising until the start of the 2020s when food prices began to increase dramatically. While the COVID-19 Pandemic certainly had its effects, other factors have probably caused this to continue late into the decade. Thus, while the data is not yet complete for 2026 (this explains the line’s sudden drop then), the general trend is that food prices might continue to increase in the next few years if not into the next decade. This can also be said of other markets in the country.

For a restaurant business, this is not ideal or even feasible. Stakeholders should carefully consider how expenses might continue to go up should they establish a restaurant. They should also consider the establishment’s location and target market; and they should pay special attention to their food products. 

## Data Structure Overview ##
Data for this analysis were extracted from two main sources. The datasets were sourced from:
- The Humanitarian Data Exchange website (https://data.humdata.org/dataset/wfp-food-prices-for-philippines); and
- the Philippine Statistics Authority (PSA) database (https://openstat.psa.gov.ph/PXWeb/pxweb/en/DB/DB__2M__NWSNEW/0052M4AWB08.px/?rxid=6eee1255-26f2-4eb6-98bc-0117e6b5c47b).

All datasets were then transformed (cleaned and organized) via Google Sheets in order to be more appropriate for PostgreSQL storage and analysis.

<img width="740" height="516" alt="ERD_Restaurant" src="https://github.com/user-attachments/assets/493dde6c-7c20-4d93-af85-b30d277ca29b" />

The Entity Relationship Diagram (ERD) for these datasets via PostgreSQL is shown above.

## Executive Summary ## 

A chicken-based menu is the most affordable menu for restaurant stakeholders. Prioritizing such a menu could also enable the restaurant to afford other commodities that can complement chicken-based dishes like onions, garlic, rice, and potatoes. Due to their unpredictable pricing, fruits and vegetable commodities should not be prioritized for the restaurant’s initial operations. 

The restaurant should also be placed in a location with large amounts of people, preferably places of interest for both residents and non-residents alike. Recommended places should be hubs for travelers, tourists, students, and employees in order for stakeholders to maximize sales and revenue. 

## Insights Discussion ## 
### Metro Manila Monthly Average Food Pricing and Change Rate ###
<img width="1978" height="909" alt="Monthly Avg  and Rate Change Pct (Metro Manila)" src="https://github.com/user-attachments/assets/84f37760-91fe-4822-985a-f53088f9ac62" />

- Within the last two years, food prices in the region have risen steadily with some fluctuations across the years.
- The graph suggests that average food prices reach their highest from November to January.
  - These months can be described as within the Philippine Christmas season.
  - Prices could rise during this season due to heightened demand for food products. 

- Meanwhile, food prices fall to their lowest around February to June.
  - Can be explained by the two intense seasons occurring during these months.
  - February to May are the local summer season.
    - Intense heat could cause other factors that influence food prices to fall.
    - The electric grid is usually strained during summer time, which can cause food farmers and vendors to promptly sell their produce rather than storing them.
    - June meanwhile is the beginning of the typhoon seasons when flooding is common.
  - In early 2026, prices for gasoline and diesel rose up.
    - While it should have a massive impact, the data shows that average food prices in the region did not rise.

- Actionable Insights
  - Stakeholders should try to balance high costs during the Christmas season.
    - Christmas marketing is highly recommended to ensure a steady flow of potential customers.
    - It might be beneficial to also invest in storage facilities (e.g. freezers) to ensure that food bought at cheaper prices from before can still be used if possible.

### Food Category Average Price Comparison ###
<img width="1962" height="981" alt="Category Avg Price (2024 - 2026)" src="https://github.com/user-attachments/assets/50e83d27-29db-4597-8c99-3487a5cdef87" />

- Meat, fish, and egg categories have the highest recorded average prices.
  - The cheapest being egg and the most expensive being shrimp.
  
- Regular, milled rice is the cheapest under cereals and tubers.
  
- Vegetables and fruits prices are more diverse.

### Seafood Monthly Average Prices ###
<img width="2047" height="909" alt="Seafood_comm (2)" src="https://github.com/user-attachments/assets/6c20e608-7577-46f7-9ad0-f071a7775b3d" />

- Analysis shows that the tiger shrimp variety is consistently the most expensive seafood product.

- Tilapia meanwhile is the cheapest and the overall most stable.
  - Tilapia’s monthly average prices do not fluctuate as much as the others’

- Actionable insights
  - Avoid including the tiger shrimp variety for the restaurant’s potential menu.
    - If shrimp is necessary, it is better to choose the endeavor variety which is significantly cheaper than the tiger one.

  - For fish, the restaurant can offer dishes that use either tilapia or milkfish (bangus).
    - These two fish are considered staples of a typical Filipino household.
    - Filipino customers should be familiar with them.

### Vegetables and Fruits Average Prices ###
<img width="1979" height="909" alt="Vegetables and Fruits" src="https://github.com/user-attachments/assets/58dfbb18-2444-4ec5-bf68-5de093a61741" />

- Price fluctuations are more common for vegetables and fruits.
  - Can be explained by the unstable agricultural economy of the country.

- Vegetables
  - Garlic, onions, and ginger.
    - Garlic is consistently the highest priced produce as per the data.
      - Though it decreased sharply in March 2026, its pricing is stable
    - White onions are cheaper than red onions.
      - Its change rates are also generally much more stable with minimal fluctuations.
     
    - Tomatoes
      - Tomatoes reflect the analysis that food becomes more expensive as December approaches; and it is the lowest during the summer seasons.
      - Though prices for tomatoes start to rise mid-year.

    - Other vegetables
      - Carrots show dramatic fluctuations across the period. 
        - In contrast to tomatoes, carrot prices fall as Christmas season approaches.
          
- Fruits
  - Data show unstable pricing for carabao mangoes and calamansi.
    - Carabao mangoes can be seen as the Philippines’ staple fruit, alongside bananas.
      - Usually used for dessert.
    - Calamansi is often used as a condiment.

- Actionable insights
  - Garlic and onions are necessary commodities for most kitchens.
    - Recommendable to buy as much garlic as possible whenever prices dip.
    - As for onions, given recent trends, white onions are considerably cheaper and their pricing is much more predictable.

  - As for other vegetables, stakeholders might have to consider seasonal-based menus in order to accommodate varying prices.
  - Unless the restaurant considers offering fruit-based desserts in its menu, it is advisable that fruits are not to be prioritized.
    - Mango prices are too volatile and too expensive as well as too limited as raw material.
    - Calamansi prices are the same and are traditionally considered as miscellaneous condiments in most Filipino restaurants.
    - Bananas have the most stability but are limited as a recipe item like mango.

### Meat Average Prices ###
<img width="2035" height="909" alt="Meat" src="https://github.com/user-attachments/assets/d59438fd-8233-4ac8-ba71-879f388f6b71" />

- Meat prices are also varied but each commodity priced significantly within a certain range.
  
- Chicken
  - The cheapest meat commodity and the stablest. 
  - Shows minimal inflation, the price being usually between 200 and 230 pesos.

 - Pork
  - Pork options are within the middle ranges.
  - Significantly more expensive than chicken and slightly cheaper than beef commodities.
  - Average pricing is much more unstable.
    - Data suggest that pork products become cheaper mid-year, around August specifically.
    - While Christmas 2025 shows pork prices to have dropped, they have also risen last year.

- Beef
  - By far the most expensive meat commodity.
  - Prices steadily rise for beef commodities with a sharp increase for beef without bones starting March 2026.

- Actionable insights
  - Chicken-based dishes are highly recommended to be prioritized.
    - They can also be easy to market to people interested in fitness as a good source of protein.
    - Chicken is also popular and familiar to potential customers.
    - It can also be eaten by people with dietary-restrictions due to religious beliefs (e.g. Muslims, Jews, Christians).
  - Avoid beef-based dishes due to its high pricing.
    - Can significantly increase restaurant expenses for minimal revenue.
  - Pork-based dishes can be included in the menu, but expenses will be higher than chicken-based ones even though the revenue they bring would be similar.
    - Both pork and chicken are similarly popular among Filipinos.
    - However, health-conscious customers like senior citizens would generally avoid pork due to their reputation as food with high-cholesterol count.

### Rice Average Prices ###
<img width="1983" height="909" alt="Rice" src="https://github.com/user-attachments/assets/397418ad-dc62-4d7a-bb0e-b17c8aa6a4b4" />

- All rice commodities show similar trends even though their prices are different.

- Actionable insights
  - Regular milled rice is the cheapest choice so stakeholders are advised to include it for menu products.

### Potato Variants Avg. Prices ###
<img width="1978" height="909" alt="Non-Rice" src="https://github.com/user-attachments/assets/537bf45a-8cc4-4acf-a155-eb51aa8e33ef" />

- Irish potatoes show more instability than sweet potatoes.
  - It is also considerably more expensive, with peak inflation as Christmas season approaches while being at its lowest during mid-year. 
- Actionable insights
  - Both commodities, while similar, are different in taste.
    - Sweet potatoes cannot be a complete substitute for Irish potatoes.
  - Stakeholders are advised to choose carefully between the two, if either one needs to be on the menu.
  - If potatoes are needed, consider offering more potato-based menu products around mid-year to reduce expenses and to maximize profitability. 

### Beans Avg. Prices ###
<img width="1984" height="909" alt="Sheet 14" src="https://github.com/user-attachments/assets/4f59a6cf-2521-44a4-b22d-2d69fb5b6f03" />

- For the past year, mung beans prices have exceeded shelled groundnuts, with a sharp increase in April 2026.
- Based on its recent trend, mung beans could return to how it was priced in 2024.
- Actionable insights
  - Mung beans are another popular staple product in the country, so it can be added to the restaurant menu if needed.
  - Shelled groundnuts are expected to continue its usual trend.
  - Both commodities, like above, cannot be substitutes of each other.
  - For consideration, shelled groundnuts are actually peanuts.
    - Including them on the menu might post risks for potential customers with peanut allergies.

### Coffee Beans Avg. Prices ###
<img width="2007" height="909" alt="Sheet 15" src="https://github.com/user-attachments/assets/02f1baf7-470e-411d-8d41-503dadc301bd" />

- Coffee bean prices per kilo are steadily on the rise.
- While Arabica beans are more expensive than Robusta beans, the gap between them is closer than it was two years ago.
  - Robusta bean prices increased sharply beginning March 2025.
  - As per recent data, Robusta beans might continue its trend and could even surpass Arabica prices.
- Actionable insights
  - Coffee Robusta is preferable due to its lower pricing.
  - Should Robusta beans exceed Arabica prices within the next months, stakeholders should switch bean commodities.

## Key Recommendations ##
**Chicken-based food menu**
- It is recommended for the restaurant to prioritize chicken-based dishes given its affordability, low-costs, and general popularity.
- Chicken is also a very versatile meat product.
  - Chicken can be combined with other low cost commodities like regular milled rice and eggs, as well as potatoes.
- The low cost of chicken might also allow stakeholders to buy additional and complementary commodities like onions and garlic.

**Metro Manila as a business location**
- Stakeholders are advised about the rising costs of food in the region.
  - As per the data above, it is expected for food prices to continue rising in 2026 and perhaps even beyond.
- To alleviate rising costs, it is recommended to choose a location within the region where both residents and non-residents alike can be potential customers of the restaurant.
  - Location should be a place where people go through everyday like transport hubs, student-centered areas, business-
  - Location recommendations:
    - Monumento, Caloocan City
    - University Belt Area, Manila City
    - Binondo, Manila City







