
# Titanic Dataset Statistical Analysis

This project demonstrates statistical analysis of the Kaggle Titanic dataset. It calculates key statistics—**mean**, **median**, **mode**, and **standard deviation**—for relevant columns, after handling missing data. The analysis is performed using Python with libraries like `pandas`, `numpy`, and `scipy`.

---

## Features

- **Data Cleaning**:
  - Handles missing values in the dataset by:
    - Dropping columns with excessive missing values (e.g., `Cabin`).
    - Imputing missing numerical values (e.g., `Age`) with the median.
    - Imputing missing categorical values (e.g., `Embarked`) with the mode.
  
- **Statistical Calculations**:
  - Calculates **mean**, **median**, **mode**, and **standard deviation** for numerical columns like:
    - `Age`
    - `Fare`
    - `SibSp`
    - `Parch`
  - Allows column-specific and dataset-wide calculations.

---

## Setup

### Prerequisites
- Python 3.x
- Required Libraries:
  - pandas
  - numpy
  - scipy

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/titanic-statistics.git
   ```
2. Navigate to the project folder:
   ```bash
   cd titanic-statistics
   ```
3. Install dependencies:
   ```bash
   pip install pandas numpy scipy
   ```

---

## Usage

1. Download the Titanic dataset from Kaggle ([Link](https://www.kaggle.com/competitions/titanic/data)).
2. Place the dataset file (`train.csv`) in the project directory.
3. Run the Python script:
   ```bash
   python analysis.py
   ```
4. The script will:
   - Clean the dataset by handling missing values.
   - Calculate and display the **mean**, **median**, **mode**, and **standard deviation** for numeric columns.
   - Provide results for both individual columns (e.g., `Age`) and all numeric columns.

---

## Example Output

For the `Age` column:
```
Statistics for 'Age':
Mean: 29.70
Median: 28.00
Mode: 24.00
Standard Deviation: 14.52
```

For all numeric columns:
```
Statistics for 'Fare':
Mean: 32.20
Median: 14.45
Mode: 8.05
Standard Deviation: 49.69
```

---

## File Structure
```
titanic-statistics/
│
├── train.csv             # Titanic dataset (downloaded from Kaggle)
├── analysis.py           # Python script for data cleaning and statistical analysis
├── README.md             # Documentation
└── requirements.txt      # List of dependencies
```

---

## Customization
- Modify the `analysis.py` script to add advanced imputation techniques or include new statistical metrics.
- Use visualization libraries like `matplotlib` or `seaborn` to visualize the distribution of numeric columns.

---

## Contributing
1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your feature"
   ```
4. Push to your branch:
   ```bash
   git push origin feature/your-feature
   ```
5. Create a Pull Request.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
