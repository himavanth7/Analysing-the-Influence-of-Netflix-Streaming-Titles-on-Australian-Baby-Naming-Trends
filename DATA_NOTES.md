# **Data Notes**

## **1. Data Sources**

### **South Australian Baby Names (2014–2024)**  
- **Source:** Government of South Australia – Data.SA  
- **URL:** [https://data.sa.gov.au/data/dataset/popular-baby-names](https://data.sa.gov.au/data/dataset/popular-baby-names)  
- **Description:** Contains yearly lists of popular baby names registered in South Australia, split by gender.  
- **Format:** CSV files for each year, separated into `male` and `female` folders.

### **Netflix Titles Metadata**  
- **Source:** Kaggle – Netflix Movies and TV Shows Dataset  
- **URL:** [https://www.kaggle.com/shivamb/netflix-shows](https://www.kaggle.com/shivamb/netflix-shows)  
- **Description:** Metadata for Netflix movies and TV shows, including title, type, cast, release year, rating, duration, genres, and descriptions.  
- **Format:** Single CSV file.

---

## **2. Preprocessing & Cleaning**

1. **Loading and Merging**
   - Read all male and female baby name CSVs for 2014–2024.
   - Combined male and female datasets into a single dataset with gender tags.

2. **Standardisation**
   - Converted all text to lowercase.
   - Removed non-alphabetic characters from names and titles.
   - Trimmed whitespace.

3. **Filtering**
   - Filtered to **single-word names only**.
   - Removed duplicates in both baby name and Netflix datasets.

4. **Matching**
   - Identified exact matches between baby names and Netflix titles.
   - Annotated matches with Netflix release year.

5. **Feature Engineering**
   - Created categorical encoding for `type` (movie/TV show).
   - Added binary label for “influenced” names (match found).

---

## **3. File Structure**

```
baby_names/
    male/
        male2014.csv
        ...
        male2024.csv
    female/
        female2014.csv
        ...
        female2024.csv
netflix_data/
    netflix_titles.csv
processed_data/
    matched_names.csv
    cleaned_baby_names.csv
```

---

## **4. Notes & Limitations**
- The baby name dataset only includes registered names in South Australia.
- No popularity or viewership statistics for Netflix titles were available — matches are based solely on name presence.
- Analysis excludes multi-word names and character names not matching titles exactly.
