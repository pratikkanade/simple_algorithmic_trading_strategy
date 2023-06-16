# algobulls
AlgoBulls Assignemnt -  Simple Algorithmic Trading Strategy

This repository contains a simple algorithmic trading strategy implemented in Python. The strategy aims to determine the optimal selling or buying date and time for a given equity based on the moving averages of the equity's market price over a specified time period. It utilizes these moving averages to generate a resultant dataframe that provides insights for executing trades.

### Prerequisites

- python 3.
- jupyter notebook
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

2. Provide the equity name on which the trading stratergy is to be implemented as an argument to the functions wherever required.

   ```bash
   script_data.fetch_intraday_data('GOOGL')

4. Call the Kernel and click the Restart & Run All option to execute the entire file.
