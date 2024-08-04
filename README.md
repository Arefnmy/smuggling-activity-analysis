# Investigating the Relationship Between Fuel Price Disparities and Traffic Flow on Border Roads

_This project was completed during the course "Introduction to Statistical Learning" at Sharif University of Technology (Spring 2024)._
## Project Overview

This project consists of two distinct phases: practical and theoretical. The first phase involves data analysis, evaluating regression models, and reporting results. The second phase includes a critical review of the first phase and a reformulation of the problem within the context of **Causal Inference**.

## Phase 1

In this phase, we examine the relationship between fuel prices in Turkey and traffic flow on the border roads between Iran and Turkey. Our hypothesis is that an increase in fuel prices in Turkey leads to higher levels of fuel smuggling from the country, which in turn affects traffic flow on the border roads.

We extracted fuel price data for Turkey from [tradingeconomics.com](tradingeconomics.com) and Iran traffic data from [141.ir](141.ir), organizing and summarizing the data monthly from 2016 to 2023.

To investigate the meaningful relationship between fuel prices and traffic flow, we first converted Turkish fuel prices to Iranian rials using the website [tgju](tgju.org). This conversion improves the accuracy of our results, as the price discrepancy between Turkey and Iran drives smuggling. Using correlation and simple linear regression models, we demonstrated a significant relationship between the two variables at a 95% confidence interval.

To further validate that this relationship could indicate smuggling in border provinces, we conducted the same analysis for some non-border roads. Our results showed no significant relationship between traffic flow and fuel prices on non-border roads. We argued that this method might suggest the presence of smuggling in border provinces.

## Phase 2

In this phase, we aimed to explicitly frame the problem in terms of Causal Inference. We then critically reviewed and improved upon our previous results.

It is clear that correlation does not imply causation, as there may be confounding variables affecting both our independent and dependent variables. In this case, the dependent and independent variables are traffic flow and fuel prices, respectively.

Initially, we attempted to establish a causal relationship between fuel prices and traffic flow using various acceptable methods in causal inference, including multiple regression, instrumental variables, and the backdoor criterion. We reviewed different types of these methods in our project through various articles.

Next, we sought to identify the presence of a smuggling variable, which in causal inference is referred to as a mediator. To handle this variable, we considered various methods, including mediator analysis.

## Project Structure

- `codes`: Contains files for cleaning, scraping, and analyses.
- `datasets`: Includes the datasets we worked with or generated.
- The first project's report can be found in `Smuggling_Activity_Analysis_Report.pdf` .
- The second project's paper can be found in `Fuel Prices and Traffic Flow on Border Roads: Uncovering Smuggling Patterns.pdf`
