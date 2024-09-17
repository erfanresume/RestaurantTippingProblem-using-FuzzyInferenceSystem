# RestaurantTippingProblem-using-FuzzyInferenceSystem
In this project, I create a fuzzy control system which models how you might choose to tip at a restaurant
## Overview
### Fuzzification
- Antecednets (Inputs)
  - service
    - Universe (ie, crisp value range): How good was the service of the wait staff, on a scale of 0 to 10?
    - Fuzzy set (ie, fuzzy value range): poor, acceptable, amazing
  - food quality
    - Universe: How tasty was the food, on a scale of 0 to 10?
    - Fuzzy set: bad, decent, great
- Consequents (Outputs)
  - tip
    - Universe: How much should we tip, on a scale of 0% to 25%
    - Fuzzy set: low, medium, high
### Rules
- IF the service was good or the food quality was good, THEN the tip will be high.
- IF the service was average, THEN the tip will be medium.
- IF the service was poor and the food quality was poor THEN the tip will be low.
### Defuzzification
In this part, we worked on defuzzification which is the process of converting a fuzzy set (with grades of membership) into a crisp value (single numerical output).
### Usage
- If I tell this controller that I rated:
  - the service as 9.8, and
  - the quality as 6.5,
- it would recommend I leave:
  - a almost 19% tip.
