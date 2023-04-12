# A startup selling food

## Data
The data is presented by the event log of the mobile application in the context of user IDs and their IDs of A/B test groups.

## Tasks
- explore the sales funnel,
- find out how users reach the purchase, 
- how many users reach the purchase, and how many are "stuck" on the previous steps (on which ones),
- to investigate the results of the A/A/B experiment (control groups 246 and 247 - groups A/A-test, 248 - test group B, in which the font of the interface was changed).

## Research progress
- data preprocessing was performed,
- according to the logging log, the period of data analysis relevant for the study was determined,
- the steps of the sales funnel were determined and conversions were calculated,
- the analysis of the A/A and A/B test results was carried out,
- taking into account the performed multiple comparison, the Shidak correction was calculated for the selected critical level of statistical significance,
- statistical hypotheses were tested by the z-test for equality of shares between control groups (A1/A2), between control and test group (A1/B, A2/B, A1+A2/B).

## Conclusions
- the sales conversion (from the landing page to the order payment page) was 50%,
- the division of users into control (A1 and A2) and test (B) groups was performed correctly (with minor comments),
- with the selected critical level of statistical significance of 5%, taking into account the Shidak correction, the indicator value was 0.32%,
- in the A/A test for funnel steps, no statistically significant difference was found between groups A1 and A2, so the minimum p-value of all steps was 11.4%,
- for tests in groups A1/B, A2/B, A1+A2/B, no statistically significant differences were also found, the minimum p-value of all steps was 8.1%,
- the font change in test group B did not affect the conversion in any way compared to the control groups.

## Used libraries
- pandas
- plotly
- scipy
- numpy
