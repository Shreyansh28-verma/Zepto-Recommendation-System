
# Zepto Recommendation System

This repository contains the code for a recommendation system designed for Zepto. The system uses various techniques to suggest products based on user queries.

## Requirements

To run the code, you need to have the following Python packages installed:

- `mlxtend`
- `fuzzywuzzy`
- `scipy`
- `numpy`
- `pandas`
- `scikit-learn`
- `matplotlib`
- `joblib`

You can install these packages using `pip`:


``` ! pip install mlxtend fuzzywuzzy scipy numpy pandas scikit-learn matplotlib joblib ```


## Overview

The recommendation system consists of three main components:

1. **Finding Similar Products**: Utilizing `fuzzywuzzy` to identify products similar to the user's query. This is particularly useful when the exact word is not present in the dataset (e.g., "Milk") but related terms like "Milk bread" are present. `fuzzywuzzy` helps find and match these related words.

2. **Interactive Recommendations**: Offering a list of similar products for the user to choose from and subsequently generating recommendations based on the selected product. This component encompasses three parts:
   - **Session Data Processing**
   - **Product Data Processing**
   - **Historical Sales Data Processing**
   
   A hybrid model is then constructed to integrate these data processing types, resulting in tailored recommendations.

## Usage

### Interactive Recommendations

To test the interactive recommendation system, execute the provided script. It will prompt you to enter a product name and subsequently offer recommendations based on the selected product.



