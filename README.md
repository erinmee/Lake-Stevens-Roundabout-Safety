# Lake-Stevens-Roundabout-Safety

Erin Mee

December 9, 2025

UW MSDS - DATA 512 Human Centered Data Science Project

## Summary & Findings

Analysis of car crash frequency and severity surrounding the Lake Stevens WA roundabouts installed in 2023. With the completion of the Lake Stevens two lane roundabouts on Highway 9 and State Route 204, car accidents were found to have increased, with the month following the completion having nearly an accident a day compared to 2-5 accidents a month. Car crash data was taken from [Washington State Patrol Collision Analysis Tool](https://collisionanalysistool.wsp.wa.gov/) and a negative binomial model was fit to the data. Although, crashes significantly increased imediately following the roundabout completion, accident frequency has been dropping 3% per month in the two years following the roundabout completion.

## Contents

```
./data
./data/collision_data/
./data/data_retrieval.ipynb
./data/CAT_DataDictionary.xlsx
.data/collision_analysis_tool_lookup_tables.xlsx
./images
Lake-stevens-roundabout-analysis.ipynb 
environment.yml
README.md
LICENSE
```

## Environment Setup

create the `roundabout-env` to run the `Lake-stevens-roundabout-analysis.ipynb` notebook

```bash
conda env create --file environment.yml
```

## Data Used

[Washington State Patrol Collision Analysis Tool](https://collisionanalysistool.wsp.wa.gov/)

Anonymized collision data is made available to the public through the Public Records Act found in Chapter 42.56 of the Revised Code of Washington State.

## License

MIT License