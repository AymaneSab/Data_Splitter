# CSV Data Splitter

## Overview

This Python script is designed to split a CSV file containing data into three parts: JSON, a database, and CSV. The script allows for customization of the distribution percentages among these three destinations. It ensures a random distribution of data to maintain diversity in each output.

## Features

- **Data Loading**: The script can load data from a CSV file with a header in the first line.

- **Data Distribution**: It shuffles the rows of the CSV file to achieve a random distribution of data. The user can specify custom distribution percentages.

- **JSON Output**: 30% of the data is saved in a JSON file. Each line in the JSON file represents an entry from the CSV data.

- **CSV Output**: The remaining data is saved in a CSV file. The header is excluded from this file.

- **Database Transfer**: 30% of the data is stored in a specified database table. The user can provide the database name and table name as arguments.

## Usage

```bash
python data_splitter.py --csv_file input_data.csv --json_file output_data.json --db_name my_database --table_name my_table --distribution 30 30 40
