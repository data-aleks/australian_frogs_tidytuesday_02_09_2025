# Australian Frogs - Tidy Tuesday - 02.09.2025
This week we're exploring 2023 data from the sixth annual release of FrogID data.

FrogID is an Australian frog call identification initiative. The FrogID mobile app allows citizen scientists to record and submit frog calls for museum experts to identify. Since 2017, FrogID data has contributed to over 30 scientific papers exploring frog ecology, taxonomy, and conservation.

Australia is home to a unique and diverse array of frog species found almost nowhere else on Earth, with 257 native species distributed throughout the continent. But Australia’s frogs are in peril – almost one in five species are threatened with extinction due to threats such as climate change, urbanisation, disease, and the spread of invasive species.

## Dataset
* **Source:** [Tidy Tuesday - 02.09.2025](https://github.com/rfordatascience/tidytuesday/blob/main/data/2025/2025-09-02/)

## Tech Stack
* `pandas`
* `power bi`

## Key Steps
1. **Step 1. Exploring Dataset**
2. **Step 2. Cleaning Data**
3. **Step 3. Exporting data for Power BI Dashboard**
4. **Step 4. Power BI Dashboard Creation**

## Project Objective
This week i will be improving my workflow from doing same work twice in both python and power bi to utilising python for data cleaning and preprocessing and then visualising the data within power bi. This will hopefully let me save some time. Here are some of the questions i am hoping to answer using this dataset: 

* Are there species that are endemic to certain regions?
* Do different frog species have distinct calling seasons?
* Which species has the widest geographic range? Which is the rarest?

## Exploring Dataset
This is a fairly clean dataset, with minimal missing values. There is a date, time and time_zone columns which i think best to combine in to a single datetime column. We will rename all column names in to snake_case and go over the existing data types to ensure correct data types are selected. 

## Data cleaning
* Renamed all columns to snake_case
* Removed date, time, and time_zone columns from id dataset, created a combined datetime column instead
* Converted scientific_name, state_province data types to category
* Converted occurance_id, event_id, recorded_id to int32 data type
* Converted sub_family, tribe in names dataset to category
* Dropped 1 record from names dataset as missing scientific_name
