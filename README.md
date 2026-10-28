# Travel Booking Analysis (2023–2025)

## About the Project

This project looks at travel booking data from 2023 to 2025 to understand how booking activity changed over the three years, which travel packages performed best, and where most of the booking value came from.

I worked with booking records from three separate years and a packages dataset. Using Python, Pandas, and NumPy, I combined the records, cleaned the data, and analyzed booking activity and package performance.

The main focus was understanding how booking value was distributed across different travel package categories.

## Questions to Answer

1. Is the business growing?
2. Which travel packages perform best?
3. Where does booking value come from?

## Tools Used

- **Python** - data processing and analysis
- **Pandas** - cleaning, grouping, and merging datasets
- **NumPy** - reshaping the results into a table
- **Jupyter Notebook** - writing and documenting the analysis

## What I Did

I started by combining booking records from 2023, 2024, and 2025 into one DataFrame.

Before analyzing the data, I checked for missing values and duplicates. I removed duplicate booking IDs, replaced missing agent IDs with `"Unknown"`, filled missing discount values with zero, and standardized booking statuses and dates.

I then used the cleaned data to answer the three business questions.

### 1. Is the Business Growing?

I grouped the bookings by year and calculated total booking value, the number of bookings, and the number of travellers.

The results showed an increase in all three measures between 2023 and 2025.

### 2. Which Travel Packages Perform Best?

I grouped bookings by package ID and ranked the packages based on total booking value.

I then merged the results with the packages dataset to identify the package names and examine the top three performers.

### 3. Where Does Booking Value Come From?

For this part, I merged the package categories into the bookings data and grouped the results by year and category.

I calculated booking value, booking counts, and travellers served for each category. I then used NumPy to reshape the booking values and created a table comparing Budget, Mid-Range, and Luxury packages across the three years.

The results showed that **Luxury packages contributed the highest booking value in every year**, followed by Mid-Range and Budget packages.

Luxury booking value increased from $6,639,420 in 2023 to $14,115,070 in 2025.

Finally, I exported the reshaped results to a CSV file.

## Project Files

- `notebooks/analysis.ipynb` - the data cleaning and analysis notebook
- `outputs/booking_value_analysis.csv` - the exported booking value table
- `pyproject.toml` - Python project configuration