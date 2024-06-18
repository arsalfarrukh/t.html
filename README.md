file_path =r"C:\Users\14167\Downloads\CH06PR18.txt"
with open(file_path, 'r') as file:
    lines = file.readlines()

# Step 2: Process each line and store data in a list
data = []
for line in lines:
    line = line.strip()
    if line:  # Check if line is not empty
        values = line.split()
        # Convert values to appropriate data types if needed
        values = [float(val) for val in values]  # Convert to float if all are numeric
        data.append(values)

# Step 3: Verify data read
# Print first few rows of data to verify
print("First few rows of data:")
for row in data[:5]:  # Print first 5 rows
    print(row)

# Example: Calculate mean, median, standard deviation of X2
X2_values = [row[2] for row in data]  # Extract X2 values
mean_X2 = sum(X2_values) / len(X2_values)
median_X2 = sorted(X2_values)[len(X2_values) // 2]
std_X2 = (sum((x - mean_X2) ** 2 for x in X2_values) / len(X2_values)) ** 0.5

print("\nCalculations for X2:")
print(f"Mean of X2: {mean_X2}")
print(f"Median of X2: {median_X2}")
print(f"Standard deviation of X2: {std_X2}")

# Example: Draw boxplot for Y, X1, X2, X3, X4 (if needed, using matplotlib and seaborn)
import matplotlib.pyplot as plt
import seaborn as sns

# Prepare data for boxplot
data_df = pd.DataFrame(data, columns=['Y', 'X1', 'X2', 'X3', 'X4'])

# Draw boxplot using seaborn
plt.figure(figsize=(10, 6))
sns.boxplot(data=data_df[['Y', 'X1', 'X2', 'X3', 'X4']], orient='v', palette='Set3')
plt.title('Boxplots of Y, X1, X2, X3, X4')
plt.ylabel('Values')
plt.grid(True)
plt.show()
