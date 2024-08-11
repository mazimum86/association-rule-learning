# Association Rule Learning

This repository contains an implementation of Association Rule Learning algorithms, commonly used in data mining to discover interesting relationships, patterns, and associations within large datasets. 

## Dataset

The dataset used in this implementation typically consists of transactional data, where each transaction includes a list of items. The goal is to find rules that imply certain items are likely to be purchased together.

## Contents

- **association_rule_learning.py**: The main script that implements Association Rule Learning using algorithms like Apriori and Eclat. The script includes data preprocessing, rule generation, and visualization of the results.
- **data.csv**: The dataset file used for generating association rules.
- **requirements.txt**: A list of Python dependencies required to run the code.
- **results/**: A directory containing the generated association rules and their visualizations.

## Implementation Details

The implementation follows these steps:

1. **Data Loading**: The dataset is loaded from `data.csv` and prepared for rule mining.
2. **Data Preprocessing**: The dataset is preprocessed to convert it into a suitable format for association rule learning, typically a one-hot encoded dataframe.
3. **Rule Generation**: Association rules are generated using the Apriori or Eclat algorithm. Key metrics like support, confidence, and lift are calculated to evaluate the strength of the rules.
4. **Rule Filtering**: The generated rules are filtered based on minimum thresholds for support, confidence, and lift to retain only the most significant rules.
5. **Visualization**: The resulting association rules are visualized using bar plots, scatter plots, or network graphs to highlight relationships between items.

## Usage

To use this code, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/mazimum86/association-rule-learning.git
    ```
2. Navigate to the repository directory:
    ```bash
    cd association-rule-learning
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
4. Run the Association Rule Learning script:
    ```bash
    python association_rule_learning.py
    ```

## Dependencies

The following Python packages are required to run the code:

- pandas
- mlxtend
- numpy
- matplotlib
- seaborn

These dependencies are listed in the `requirements.txt` file and can be installed using `pip`.

## Results

The output includes:

- **Association Rules**: A list of association rules with their corresponding support, confidence, and lift values.
- **Rule Visualizations**: Visualizations of the most significant rules, highlighting the relationships between items in the dataset.

## Contributing

Contributions are welcome! If you have any ideas for improvements or additional features, feel free to submit a pull request or open an issue.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
