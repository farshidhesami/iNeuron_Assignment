# iNeuron_Assignment
Assignment A for Job Guarantee Program Course


import pandas as pd

# Read the CSV file
csv_file = r'D:\iNeuron_Projects\Assignment\iNeuron_Assignment\Statistics_question\data.csv'
data = pd.read_csv(csv_file)

# Convert to JSON
json_file = r'D:\iNeuron_Projects\Assignment\iNeuron_Assignment\Statistics_question\data.json'
data.to_json(json_file, orient='records', indent=4)

# Convert to XLSX
xlsx_file = r'D:\iNeuron_Projects\Assignment\iNeuron_Assignment\Statistics_question\data.xlsx'
data.to_excel(xlsx_file, index=False)


-------------------------------------------
import pandas as pd

# Read the CSV file into a DataFrame
df = pd.read_csv('data.csv')

# Display the DataFrame
print(df)
-------------------------------------------
import pandas as pd

# Read the JSON file into a DataFrame
df = pd.read_json('data.json')

# Display the DataFrame
print(df)
-------------------------------------------

import pandas as pd

# Load the dataset
df = pd.read_csv('instagram_reach.csv')

# Clean missing data
df_clean = df.dropna()

# Save cleaned data to a new CSV file
df_clean.to_csv('instagram_reach_clean.csv', index=False)

--------------------------------------------
