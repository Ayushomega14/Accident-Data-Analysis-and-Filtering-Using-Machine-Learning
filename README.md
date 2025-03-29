# Data-Filtering-and-Saving-Utility

## Table of Contents
- [Overview](#overview)
- [Project Structure](#project-structure)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Data](#data)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## Overview
This project provides a Python utility for filtering and saving CSV datasets based on specified conditions. The script enables data cleaning by removing unwanted rows, filtering specific conditions, and handling outliers using the Interquartile Range (IQR) method. The final filtered data can be saved at a user-defined location via a graphical file dialog.

---

## Project Structure
```plaintext
.
├── data/
│   └── input_data.csv        # Raw input CSV file (to be provided by the user)
├── scripts/
│   └── data_filtering.py    # Main script for data filtering and saving
├── notebooks/
│   └── data_filtering.ipynb  # Jupyter notebook for interactive data filtering
├── requirements.txt       # Dependencies required to run the project
├── README.md              # Project README file
└── LICENSE                 # Project License
```

## Features

- **Flexible Filtering:**
  - Removes rows where 'Age' is less than 18.
  - Filters data to include only 'Severe' or 'Fatal' cases in 'Accident_Severity'.
  - Removes outliers from numerical columns using the IQR method.

- **Interactive File Saving:**
  - Users can choose the save location for the filtered data using a graphical file dialog.

- **Missing Value Handling:**
  - Automatically drops rows with missing values in numerical columns.

---

## Technologies Used

- **Python:** Core programming language.
- **Pandas:** For data manipulation and analysis.
- **NumPy:** For numerical operations and handling missing values.
- **Tkinter:** For file dialog interface to select save location.

---

## Installation

To run this project locally, follow these steps:

1. **Clone the repository:**
```bash
git clone https://github.com/your-username/Data-Filtering-and-Saving-Utility.git
```

2. **Navigate into the project directory:**
```bash
cd Data-Filtering-and-Saving-Utility
```

3. **Install the required dependencies:**
```bash
pip install -r requirements.txt
```

Make sure to have the `input_data.csv` dataset in the `data/` folder or load your own dataset during runtime.

---

## Data

The dataset used should be in CSV format and can contain various columns. For this script to work optimally, it expects the following (modifiable as per user needs):

- **Age:** Numeric column to filter individuals aged 18 and above.
- **Accident_Severity:** Categorical column with values such as 'Severe' or 'Fatal'.
- **Numerical Columns:** Any columns with numerical data will be processed for outlier removal.

---

## Usage

To run the script and filter your dataset, follow these steps:

1. **Run the Script:**
   - If using a script:
   ```bash
   python scripts/data_filtering.py
   ```

   - If using a Jupyter notebook:
   ```bash
   jupyter notebook notebooks/data_filtering.ipynb
   ```

2. **Select the CSV File:**
   - A file dialog will prompt you to select the input CSV file.

3. **Choose Save Location:**
   - After filtering, a file dialog will allow you to choose where to save the filtered dataset.

4. **Output:**
   - The filtered CSV file will be saved at your chosen location.

---

## Results

The script outputs a filtered dataset based on the specified conditions:

- Rows with 'Age' < 18 are removed.
- Only rows with 'Accident_Severity' of 'Severe' or 'Fatal' are retained.
- Outliers from numerical columns are filtered using the IQR method.

The final dataset is saved as a CSV file in the location chosen by the user.

---

## Contributing

Contributions are welcome! If you’d like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new feature branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

## Contact

For any questions or suggestions, please contact:

	•	Ayush Raj
	•	Email: ar5787@srmist.edu.in
	•	GitHub: Ayushomega14

 	•	Arya Pratap Singh Chauhan
	•	Email: Arya.pratap.chauhan@gmail.com
	•	GitHub: ARYA-0

