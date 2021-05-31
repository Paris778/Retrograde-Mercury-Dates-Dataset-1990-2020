# Retrograde Mercury Dates Dataset 1990-2020

This is public dataset compiled by Paraskevas Solomou listing all periods during which the planet Mercury followed a retrograde course (according to Astrology) between January 1st 1990 and December 31st 2020

## Dataset Aim

This dataset was created in order to encourage Astology related research. 

## Dataset Overview

The retrograde mercury period dataset was compiled manually using an open source restful API [1] exclusively for the needs of this project. A python script was developed which repeatedly sent remote requests to the API and documented the results in a CSV format.
That API unfortunately, could not provide data regarding the retrograde periods prior to 2016, therefore all the retrograde periods from January 1990 to December 2015, had to be inserted semi-manually. The dates of the retrograde periods found online at [2] were inserted into a script which compiled a new dataset in the same format as the one made using the API, in order to compensate for the missing data. 

It was also found that various sources listed different dates regarding the start and end of any given mercury retrograde period during the years this project is concerned with. After intense analysis and the crossing over of information from various famous astrology sources [1,2,3] with the final mercury retrograde dataset, it was determined that an additional 3% uncertainty will be introduced to the results of this project in order to compensate for this great variance and inconsistency among data sources. 
The final retrograde mercury dataset is made publicly available at [3] in order to encourage further research and discussion. 

## Dataset Description

The present dataset consists of two features those being: 

- DATE         | date format (yyyy/mm/dd)
- isRetrograde | boolean (0 or 1) 
- 
<picture> 
  
isRetrograde has a value of 1 (one) when mercury was in retrograde during the respective date and 0 (zero) when it was following a normal course.

## Usage Example (Python 3)

##### 1. Download Dataset
##### 1.5. Set up a virtual environment (Anaconda / MiniConda for Python) 
  Tutorial: https://katiekodes.com/setup-python-windows-miniconda/

  ##### 2. Download Dependencies
  - pandas
  - matplotlib
  
##### 3. Load dataset
```python
# Imports
import pandas as pd
import datetime
import matplotlib.pyplot as plt

########################################################
# Load dataset 
########################################################

file_path = (inset path here)
df_short = pd.read_csv(file_path)
```
## 

#### References

[1] Anon, Mercury Retrograde API. Available at: https://mercuryretrogradeapi.com/about.html [Accessed May 23, 2021]. 

[2] Anon, Free Horoscopes & Astrology online: Astro-Seek.com. Astro. Available at: https://horoscopes.astro-seek.com/ [Accessed May 23, 2021]. 

[3] AstroTwins, 2021. Retrogrades: When Planets Go Backward: Astrostyle: Astrology and Daily, Weekly, Monthly Horoscopes by The AstroTwins. Astrostyle. Available at: https://astrostyle.com/learn-astrology/retrogrades/ [Accessed May 31, 2021]. 

[12] Solomou, Paraskevas, Paris778/Retrograde-Mercury-Dates-Dataset-1990-2020. GitHub. Available at: https://github.com/Paris778/Retrograde-Mercury-Dates-Dataset-1990-2020


