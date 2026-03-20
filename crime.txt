import csv

# Sample data (you can replace this with your API data)
data = [
    ["Channel", "Title", "Published"],
    ["The Tribune", "Crime News 1", "2026-03-19"],
    ["NDTV", "Crime News 2", "2026-03-18"]
]

# File name
filename = "crime_data.csv"

# Writing to CSV
with open(filename, mode='w', newline='', encoding='utf-8') as file:
    writer = csv.writer(file)
    
    # Write rows
    writer.writerows(data)

print("Data successfully saved to crime_data.csv")
