# Brazil No-show Appointments Analysis

## Introduction
This project analyzes the Brazil No-show Appointments Dataset, which contains information on over 100,000 medical appointments in Brazil. The dataset includes patient demographics, medical conditions, SMS reminders, and whether patients attended their appointments. The analysis focuses on understanding factors influencing no-show rates, such as SMS reminders, gender, medical conditions, neighborhoods, and age.

## Project Goals
The analysis addresses the following questions:
1. What is the overall no-show rate?
2. What is the effect of SMS reminders on the no-show rate?
3. What is the effect of gender on the no-show rate?
4. What is the effect of medical conditions on the no-show rate?
5. Which neighborhoods have the highest no-show rates?
6. How does age affect the likelihood of missing an appointment?

## Repository Structure
```
├── data/
│   └── KaggleV2-May-2016.csv      # Dataset file
├── notebooks/
│   └── No_show_Analysis.ipynb     # Jupyter notebook with analysis
├── reports/
│   └── Final_Project.pdf          # Final report in PDF format
├── README.md                      # Project documentation
└── .gitignore                     # Git ignore file
```

## Installation
To run the Jupyter notebook locally, ensure you have Python and the required libraries installed. Follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/brazil-no-show-appointments.git
   cd brazil-no-show-appointments
   ```

2. **Install dependencies**:
   Create a virtual environment and install the required packages:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install pandas matplotlib seaborn jupyter
   ```

3. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```
   Open `notebooks/No_show_Analysis.ipynb` in the browser.

## Usage
- **Dataset**: The dataset (`KaggleV2-May-2016.csv`) is stored in the `data/` folder. Ensure it remains in this location for the notebook to run correctly.
- **Notebook**: The `No_show_Analysis.ipynb` notebook contains data wrangling, cleaning, exploratory data analysis, and visualizations for the six questions listed above.
- **Report**: The `Final_Project.pdf` in the `reports/` folder provides a detailed write-up of the analysis, including conclusions and limitations.

To reproduce the analysis:
1. Open the Jupyter notebook.
2. Run all cells to execute the data cleaning, analysis, and visualization steps.
3. Review the outputs and visualizations to understand the no-show patterns.

## Results
Key findings from the analysis:
- **Overall No-show Rate**: 28.52% of patients missed their appointments.
- **SMS Reminders**: Patients receiving SMS reminders had a slightly lower no-show rate (27.57%) compared to those who did not (29.44%).
- **Gender**: No significant difference in no-show rates between females (28.45%) and males (28.67%).
- **Medical Conditions**:
  - Hypertension: Lower no-show rate (23.52%) compared to non-hypertensive patients (29.84%).
  - Diabetes: Lower no-show rate (24.96%) compared to non-diabetic patients (28.81%).
  - Alcoholism: Higher no-show rate (34.08%) compared to non-alcoholic patients (28.37%).
  - Handicap: Varies by level, with level 4 showing a 50% no-show rate.
- **Neighborhoods**: "ILHAS OCEÂNICAS DE TRINDADE" had the highest no-show rate (100%), possibly due to data issues.
- **Age**: Younger patients tend to have higher no-show rates, as shown in the age distribution plot.

## Limitations
- The analysis identifies correlations, not causation.
- Data quality issues, such as potential errors in neighborhood no-show rates, may affect results.
- Confounding variables (e.g., socioeconomic status) were not considered.
- Findings may not generalize to other populations.

## Future Work
- Conduct causal analysis to identify factors driving no-show rates.
- Explore additional variables like socioeconomic status or distance to clinics.
- Test interventions (e.g., enhanced reminders) to reduce no-shows.
- Improve data quality through better validation processes.

## Contributing
Contributions are welcome! Please:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m "Add your feature"`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.

## Citation
If you use this project in your research, please cite:
```
Your Name. (2025). Brazil No-show Appointments Analysis. GitHub Repository. https://github.com/your-username/brazil-no-show-appointments
```

## Acknowledgments
- Dataset source: [Kaggle Brazil No-show Appointments Dataset](https://www.kaggle.com/datasets/joniarroba/noshowappointments)
- Libraries: pandas, matplotlib, seaborn, Jupyter Notebook
