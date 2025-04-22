# Provider Aggregate Table & Success Modeling

This repository contains code and methodology for constructing an aggregate provider table from healthcare claims data, 
enabling business insights and machine learning modeling of provider success outcomes.

## Overview

This project was developed to:
- Build a comprehensive provider feature table using NPI as the unique identifier.
- Enable Product, Clinical, and Operations teams to answer key business questions about provider performance, cost-effectiveness, and network optimization.
- Serve as a feature store for downstream machine learning models, such as predicting provider success rates for specific procedures and employer networks.

## Data Sources

- **encounters_details.csv**: Detailed records of healthcare encounters, including NPI, CPT code, and payment.
- **adverse_events.csv**: List of encounter IDs flagged as adverse events.
- **providers.csv**: Provider metadata, including NPI, name, and zip.
- **employer_in_network.csv**: Mapping of employer IDs to in-network NPIs.

## Technologies Used

*   Python
*   Pandas
*   NumPy
*   Scikit-learn
*   Matplotlib
*   Seaborn

## Findings

The analysis reveals that certain procedures are likely have a better a success outcome (>95%)
with certain employer id indicating strength and weaknesses of contracted provider networks. 
For eg. the heatmap indicates that procedure CPT 20610 has a much
higher chance of succeeding with a provider network of 80914. 


## Next Steps

As next steps the recommendation is to include personalized clinical data for each patient 
such as number of chronic disease or other metric that increases risk of unsuccessful procedure.
This can allow a more isolated provider specific risk analysis.

## Author

Ambreen Zaver
