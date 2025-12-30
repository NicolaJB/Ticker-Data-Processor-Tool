Ticker Data Processor Tool
==========================

This Python application processes and organises instrument data from multiple input files, making it searchable through a generated CSV file.

Overview

This script:
- parses instrument data from data.txt, StaticFields.txt, and DynamicFields.txt.
- Extracts and maps static and dynamic field values.
- Generates a CSV report with extracted information.
- Allows users to search for specific instrument codes interactively.

Files Structure: 

Ensure the following files are present in the working directory:
- InstrumentDataProcessor.py   # Main Python script
- data.txt                  # Input data file
- StaticFields.txt          # Static field mappings
- DynamicFields.txt         # Dynamic field mappings

Setup Instructions:
1. Ensure Python is Installed. Check Python 3 is installed:

python --version

If not installed, download it from python.org.

2. Clone the Repository
   
git clone https://github.com/NicolaJB/Ticker-Data-Processor-Tool.git

cd Ticker-Data-Processor-Tool

3. Run the Program
   
python InstrumentDataProcessor.py

For systems to specify Python 3 (ie Mac):

python3 InstrumentDataProcessor.py

Usage Instructions:
1. Process Data: The program reads the input files, maps fields, and generates an output CSV.
2. Search Data: After processing, you can search by instrument code interactively.

Example Workflow:
1. Run the script.
2. Enter an instrument code (as listed in data.txt) to search for its details.
3. Type exit to quit the search.

Output:

The CSV output is saved as output_DDMMYY.csv, where DDMMYY is the date from the first record in data.txt. If the date is missing, the output is saved as output.csv.

Cleanup:

To remove generated CSV files:
rm output_*.csv

Troubleshooting:
* File Not Found: Ensure data.txt, StaticFields.txt, and DynamicFields.txt exist in the same directory as the script.
* Python Version Issues: Confirm Python 3.x is being used.

## License

This project is licensed under the MIT License. 

