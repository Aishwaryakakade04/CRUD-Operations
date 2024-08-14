# CRUD-Operations
---

# Coffee Sales CRUD Operations

This repository contains a Python script that performs CRUD (Create, Read, Update, Delete) operations on a coffee sales dataset stored in a CSV file. The script uses the `pandas` library for data manipulation and provides a basic framework for managing the dataset.

## Requirements

Before running the script, ensure you have the necessary Python packages installed. You can install them using pip:

```bash
pip install pandas
```

## Script Overview

The script performs the following CRUD operations:

1. **Create**: Inserts new records into the dataset.
2. **Read**: Retrieves and displays specific records from the dataset.
3. **Update**: Modifies existing records in the dataset.
4. **Delete**: Removes specific records from the dataset.

### File Structure

- `coffee_sales.csv`: The CSV file containing the coffee sales data.
- `crud_operations.py`: The Python script performing the CRUD operations.

### CSV File Format

The CSV file (`coffee_sales.csv`) should contain the following columns:

- `date`: The date of the transaction (e.g., `2024-08-13`).
- `datetime`: The exact date and time of the transaction (e.g., `2024-08-13 14:53:45`).
- `cash_type`: The type of payment used (`card`, `online`, `cash`).
- `card`: The masked card number (e.g., `ANON-0000-0000-0902`).
- `money`: The amount of money spent on the transaction.
- `coffee_name`: The name of the coffee purchased (e.g., `Cappuccino`, `Latte`).

### CRUD Operations

#### Create

- Reads the existing CSV file into a DataFrame.
- Appends a new record to the DataFrame based on the provided data.
- Saves the updated DataFrame back to the CSV file.

#### Read

- Retrieves records from the CSV file based on specified conditions.
- Supports both label-based (`loc`) and index-based (`iloc`) filtering.

#### Update

- Modifies records in the dataset that match specified conditions.
- Updates specified columns with new values.
- Saves the updated DataFrame back to the CSV file.

#### Delete

- Removes records from the dataset that match specified conditions.
- Saves the updated DataFrame back to the CSV file.

## Usage

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/coffee-sales-crud.git
    ```

2. **Navigate to the repository**:
    ```bash
    cd coffee-sales-crud
    ```

3. **Run the script**:
    ```bash
    python crud_operations.py
    ```

Ensure the `coffee_sales.csv` file is present in the same directory as the script or adjust the file path in the script accordingly.

### Example of Adding a New Record

In the script, the following dictionary represents the data to be added:

```python
new_record = {
    'date': date.today(),
    'datetime': datetime.now(),
    'cash_type': 'card',
    'card': 'ANON-0000-0000-0902',
    'money': round(data['money'].mean(), 2),
    'coffee_name': data['coffee_name'].mode()[0]
}
```

This new record will be appended to the existing dataset.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Contact

For any issues or inquiries, please contact [Aishwarya kakade](aishwarya04kakade@gmail.com).

---
