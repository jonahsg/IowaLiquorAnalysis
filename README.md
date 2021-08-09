# Iowa Liquor Analysis

The purpose of this project was to analyze liquor sales in Iowa from 2012 - 2017 in order to make recommendations for liquor stores and distilleries on business practices.

## Dataset Used

https://www.kaggle.com/residentmario/iowa-liquor-sales

## Methodology and Findings
- Cleaned raw data via Python initially due to low speed of R with high volume datasets (about 13,000,000 x 24)
  - **Python script pulled out only 1 out of every 5 rows in order to shrink dataset to be usable in R for the remainder of this analysis
- Analyzed data by category of liquor and yearly trends
  - Found whiskey to be most popular followed by vodka
      - Good for liquor stores and distilleries to understand most popular alcohol types
  - Found no significant changes in consumption by category
      - Could've been helpful for distilleries to capitalize on new trend with what they produce and liquor stores for what they buy
  - Found all categories have an average profit margin between 50.0 and 50.3%
      - Liquor stores seem to price alcohol universally at around 50% profit regardless of type of liquor
  - Found significant variance for % unsold between liquor categories
      - Schnapps and Gin severely undersell to consumers compared to what liquor stores buy (near 40% unsold)
      - Vodka sells the most to consumers proportional to what liquor stores buy
      - Whiskey and Rum are also well sold to consumers proportional to what liquor stores buy
      - Can create significant model (p-value < 0.05 for intercept, coefficient, and overall model) showing more sales by category correlates with less unsold
 - Analyzed data by specific alcoholic product
   - Very strong majority (and all of the most popular liquors) are sold at about 50% margin
      - Helpful for liquor stores to understand what they should be pricing products at based on what they buy them for
   - Products sold at higher margins do not sell well (high % unsold compared to category's average)
      - Further proof that liquor stores should be pricing products at 50% margins
      - Specifically looked at Shellback Spiced Rum and Silver tequila (high margin products with the highest sales)
        - Found that these sell poorly (high % unsold) when compared with the average for rum and tequila categories
   - Found top sellers
      - Helpful for new liquor store to understand what they should be stocking
 - Analyzed Sales per Store
   - Found counties with high sales per store in addition to high sales in totality
      - Helpful for new distilleries and liquor stores to understand where they want to locate themselves
   - Looked at best counties as candidates for a new distillery or liquor store and analyzed their liquor type preferences
      - Found that all counties have very similar tastes in line with total preferences found initially - Whiskey then Vodka are most popular
      - Helpful for new distilleries and liquor stores starting in these counties to understand the specific county's preferences
   - Found counties with high sales per store in addition to high sales in totality
      - Helpful for new distilleries and liquor stores to understand where they want to locate themselves
 - Analysis of Price for Most Popular Liquor Types (Whiskey and Vodka)
   - Found popular price points for whiskey and vodka
   - Honed in on popular price points for higher end whiskey and vodka
      - New distilleries should know how they should be pricing their product - most new distilleries will not be able to match cheap price points
   - Identified popular whiskey and vodka in higher end popular price range
      - New distilleries should know who they will be competing with at given price range
 - Analysis of Month-by-month trends for each liquor category
   - Found all deviations by month and liquor type from mean monthly sales
   - Found months and liquor types that deviate from their mean monthly sales by 10%
   - Found months and liquor types that deviate from their mean monthly sales by 20%
      - Major finds (helpful for liquor stores in what they stock month to month and distilleries in what they make month to month):
        Gin:
          - Increase by over 20% in June
          - Decrease by over 20% in January and November
        Tequila:
          - Increase by over 20% in April and June
          - Decrease by over 20% in November
        Liqueur:
          - Increase by over 20% in October and December
        Rum:
          - Decrease by over 20% in November
        Vodka:
          - Decrease by over 20% in November
        Whiskey:
          - Increase by over 20% in October
        
