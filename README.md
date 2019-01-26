# Sources Quality Rank

## Intro

The objective of this project is to build a recommendation system to detect the best traffic sources (apps or websites) where a specific app can be promoted. An online advertising company X has a lot of historical information for a big number of apps that they promoted, such as app vertical (Games, Shopping, Transportation, etc.), Country, OS, and most importantly the results of promotion in terms of volumes (number of conversions) and traffic quality.

As a proxy for traffic quality the following metrics are used:

- KPI reach (how good was the traffic source in terms of reaching client's objective for the campaign)
- Fraud Index (how likely the conversions brought by the traffic source are fraudulent, based on a third-party fraud detection tool)
- Early Conversions (how many installs are coming within the first 2 hours after the click which is considered to be normal user behaviour). This will be used to calculate ClickSpam Index, which is another fraud indicator not accounted for by Fraud Index.

**NOTE**: all the names, such as sourceName, country, OS, app vertical were randomly generated and assigned.

## Project Structure

The project is divided into three parts:

1. Extract and Transform the data
2. Upload the resulting table to Google Sheets
3. Build Tableau dashboard based on the data

![Project Structure](https://github.com/annafedotova/sources-quality-rank/blob/master/pqr_dataflow.png?raw=true)

## Tableau Dashboard

You can find the final Source Quality Rank dashboard in my [Tableau Public profile](https://public.tableau.com/views/PQR_0/GlobalSourceQualityRank?:embed=y&:display_count=yes&publish=yes).

By specifying the app vertical and the OS of the app you would like to promote, as well as the country where you want to promote it, you will get the list of all the sources that can be used for promotion and their corresponding Quality Score.

<iframe src="https://public.tableau.com/views/PQR_0/GlobalSourceQualityRank?:showVizHome=no&:embed=true"
 width="955" height="645"></iframe>
