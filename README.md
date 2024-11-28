# Simple Algorithmic Trading Strategy

This repository contains a simple algorithmic trading strategy implemented in Python. The strategy aims to determine the optimal selling or buying date and time for a given equity based on the moving averages of the equity's market price over a specified time period. It utilizes these moving averages to generate a resultant dataframe that provides insights for executing trades.

### Prerequisites

- python 3.10.11
- jupyter notebook 1.0.0
- numpy 1.24.3
- pandas 2.0.2
- requests 2.31.0

### Installation

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/pratikkanade/algobulls.git

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt

### Usage

1. Open jupyter notebook using the path where the AlgoBulls.ipynb file is located
   ```bash
   jupyter notebook

2. Provide the equity name on which the trading stratergy is to be implemented and the time period as arguments to the functions wherever required.

3. Fetch the intraday data for required equity   
   ```bash
   script_data = ScriptData()
   script_data.fetch_intraday_data('GOOGL')

4. Convert the fetched data into a pandas dataframe
   ```bash
   script_data.convert_intraday_data('GOOGL')

5. Call the indicator1 function to calculate moving averages for specified time period.
   ```bash
   indicator1(script_data['GOOGL'], 5)   

6. Get the intraday data of the specified equity using the ScriptData class
   ```bash
   strategy = Strategy('GOOGL')
   strategy.get_script_data()

7. Get the resultant dataframe containing the signal column
   ```bash
   strategy.get_signals()
   
8. Call the Kernel and click the Restart & Run All option to execute the entire file.
