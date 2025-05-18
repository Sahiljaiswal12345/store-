# store-import pandas as pd

# Define store inventory data
data = {
    'Product ID': [101, 102, 103, 104],
    'Product Name': ['Apples', 'Rice', 'Milk', 'Bread'],
    'Category': ['Fruits', 'Grains', 'Dairy', 'Bakery'],
    'Price (₹)': [50, 80, 45, 30],
    'Quantity in Stock': [100, 200, 50, 75],
    'Supplier': ['Fresh Farms', 'Local Vendor', 'Dairy Co.', 'Baker Bros.'],
    'Last Restocked': ['12-May-2025', '10-May-2025', '15-May-2025', '14-May-2025']
}

# Create DataFrame
df = pd.DataFrame(data)

# Save to Excel file
df.to_excel("store_inventory.xlsx", index=False)

print("Excel file 'store_inventory.xlsx' has been created successfully!")
