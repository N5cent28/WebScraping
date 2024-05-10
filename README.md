Oligo Analyzer Automation

This repository contains a Python script designed to automate the interaction with the IDT's Oligo Analyzer Tool. The program uses Selenium WebDriver to automate browser actions for analyzing oligonucleotide interactions and hairpin structures directly from sequence data provided in an Excel file.

Features

Automated Login: Automatically logs into the IDT website to access the Oligo Analyzer tools.
Sequence Analysis:

Dimer Analysis: Analyzes potential dimer formations between pairs of sequences.

Hairpin Analysis: Checks for potential hairpin structures within single sequences.

Concentration Parameter Customization: Allows specification of oligo, sodium (Na), magnesium (Mg), and dNTP concentrations, with the ability to revert to default values when necessary.

Excel Integration: Reads sequences from an Excel file and writes the analysis results back to the same or a new file, including Delta G values and custom parameter settings.

Full Screen Mode: Operates in full screen to ensure all web elements are accessible.

Prerequisites

Python 3.8+
Selenium WebDriver
OpenPyXL
ChromeDriver compatible with the installed version of Chrome

Setup

Python Packages: Install the required Python packages if not already installed:
bash
Copy code
pip install selenium openpyxl httpcore
ChromeDriver: Ensure ChromeDriver is downloaded and its path is correctly set in the script.

Usage

Excel File Format:
Place the sequences and their corresponding labels in the Excel file.
Ensure the file path and sheet names are correctly set in the main() function.

Results:
The results will be written back into the specified Excel file in designated columns for easy comparison and further analysis.

Important Notes
Ensure your IDT account credentials are securely handled within the script.
Adjust the Selenium timeouts and waits based on your network speed and website response times.
The script sets the browser to full screen to avoid elements not being visible due to screen resolution limitations.


Contributions to enhance the functionality or efficiency of this script are welcome. Please fork the repository and submit a pull request with your changes.

License
This project is licensed under the MIT License - see the LICENSE.md file for details.
