# Table of Contents

1. [Problem Statement](#Problem-Statement)
2. [Executive Summary](#Executive-Summary)
3. [Data Acquisition](#Data-Acquisition)
4. [Required Libraries](#Required-Libraries)
5. [Opportunities for Future Improvements](#Opportunities-for-the-Future)

## Problem Statement

Given over 80 features inclusive of both categorical and numerical varieties, a predictive model for the sale price of houses in Ames, Iowa needs to be created within 4 business days using regression analysis for a small Kaggle competition with only certain techniques on the table. RFE, unsupervised learning and any sort of auto ML was explicity not allowed.

## Executive Summary

Given the sheer amount of features included in the sample set and the short time frame, deep investigation of the features wouldn't be feasible to manually review and in each feature interaction. To this end, custom transformer classes and a pipeline was created that maximizes the amount of features that would otherwise not be able to explore. This was accomplished by using multiple stacks of lasso regression and determining the features with the strongest coefficients then passing those features for other processing to eventually an elasticnet model.

The number of features for the most consistent results with the lowest RMSE scores ended up being 22 for the final model.

## Data Acquisition

Data comes from the [AMES dataset.](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt)

The results of this analysis are [here](https://www.kaggle.com/c/ames-iowa-housing-louisville/)

## Opportunities for the Future

Entering the general global Kaggle competition for the AMES Housing Market data, but using more techniques.