# Gini Index Impurity

This repository contains an implementation of the Gini Index Impurity calculation in Python. Gini Index is a measure of impurity or purity used in decision tree algorithms to decide the optimal split for classification tasks.

## Table of Contents
- [Gini Index Impurity](#gini-index-impurity)
  - [Table of Contents](#table-of-contents)
  - [Overview](#overview)
  - [Dataset](#dataset)
  - [Code Explanation](#code-explanation)
    - [Functions](#functions)
    - [Main Steps](#main-steps)
    - [Outputs](#outputs)
  - [Usage](#usage)
  - [Code Explanation](#code-explanation-1)
    - [Functions](#functions-1)
    - [Main Steps](#main-steps-1)
    - [Outputs](#outputs-1)
  - [Usage](#usage-1)
  - [Example Output](#example-output)
    - [Dataset:](#dataset-1)
    - [Example Impurity Calculations:](#example-impurity-calculations)
  - [License](#license)
  - [Example Output](#example-output-1)
    - [Dataset:](#dataset-2)
    - [Example Impurity Calculations:](#example-impurity-calculations-1)
  - [License](#license-1)

## Overview
The script calculates the Gini Impurity of a dataset and determines the optimal split point based on minimizing impurity. This implementation supports both binary and continuous features.

## Dataset
The dataset is represented as a NumPy array and contains the following columns:
1. Binary Feature 1
2. Binary Feature 2
3. Continuous Feature
4. Target Variable

Example dataset used in this implementation:
```python
[[1, 0, 18, 1],
 [1, 1, 15, 1],
 [0, 1, 65, 0],
 [0, 0, 33, 0],
 [1, 0, 37, 1],
 [0, 1, 45, 1],
 [0, 1, 50, 0],
 [1, 0, 75, 0],
 [1, 0, 67, 1],
 [1, 1, 60, 1],
 [0, 1, 55, 1],
 [0, 0, 69, 0],
 [0, 0, 80, 0],
 [0, 1, 87, 1],
 [1, 0, 38, 1]]
```

## Code Explanation
### Functions
1. **`calc_wighted_average(im1, imp1_multiplier, im2, imp2_multiplier)`**
   - Calculates the weighted average of impurities for two subsets.

2. **`calc_impurity(data)`**
   - Calculates the Gini Impurity for a given dataset. Supports both binary and continuous features. For continuous features, it evaluates possible split points and selects the one with the lowest weighted impurity.

### Main Steps
- The dataset is split into subsets based on a feature and evaluated for impurity.
- For continuous features, all possible split points are considered to minimize impurity.

### Outputs
- The function returns the best split point and the corresponding impurity for the feature under consideration.

## Usage
1. Clone the repository:
   ```bash
   git clone # Gini Index Impurity

This repository contains an implementation of the Gini Index Impurity calculation in Python. Gini Index is a measure of impurity or purity used in decision tree algorithms to decide the optimal split for classification tasks.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Code Explanation](#code-explanation)
- [Usage](#usage)
- [Example Output](#example-output)
- [License](#license)

## Overview
The script calculates the Gini Impurity of a dataset and determines the optimal split point based on minimizing impurity. This implementation supports both binary and continuous features.

## Dataset
The dataset is represented as a NumPy array and contains the following columns:
1. Binary Feature 1
2. Binary Feature 2
3. Continuous Feature
4. Target Variable

Example dataset used in this implementation:
```python
[[1, 0, 18, 1],
 [1, 1, 15, 1],
 [0, 1, 65, 0],
 [0, 0, 33, 0],
 [1, 0, 37, 1],
 [0, 1, 45, 1],
 [0, 1, 50, 0],
 [1, 0, 75, 0],
 [1, 0, 67, 1],
 [1, 1, 60, 1],
 [0, 1, 55, 1],
 [0, 0, 69, 0],
 [0, 0, 80, 0],
 [0, 1, 87, 1],
 [1, 0, 38, 1]]
```

## Code Explanation
### Functions
1. **`calc_wighted_average(im1, imp1_multiplier, im2, imp2_multiplier)`**
   - Calculates the weighted average of impurities for two subsets.

2. **`calc_impurity(data)`**
   - Calculates the Gini Impurity for a given dataset. Supports both binary and continuous features. For continuous features, it evaluates possible split points and selects the one with the lowest weighted impurity.

### Main Steps
- The dataset is split into subsets based on a feature and evaluated for impurity.
- For continuous features, all possible split points are considered to minimize impurity.

### Outputs
- The function returns the best split point and the corresponding impurity for the feature under consideration.

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/AlirezaMz10/Gini-index-impurity.git
   cd gini_index_impurity
   ```

2. Install the required dependencies (NumPy):
   ```bash
   pip install numpy
   ```

3. Run the script:
   ```bash
   python main.py
   ```

## Example Output
### Dataset:
```python
[[1, 0, 18, 1],
 [1, 1, 15, 1],
 ...]
```

### Example Impurity Calculations:
- Gini Impurity for Feature 1:
  ```python
  calc_impurity(df[:, [0, -1]])
  ```
  Output: `{split_point: impurity}`

- Gini Impurity for Continuous Feature:
  ```python
  calc_impurity(df[:, [2, -1]])
  ```
  Output: `{best_split: lowest_impurity}`

## License
This project is licensed under the MIT License.


   cd gini_index_impurity
   ```

2. Install the required dependencies (NumPy):
   ```bash
   pip install numpy
   ```

3. Run the script:
   ```bash
   python script_name.py
   ```

## Example Output
### Dataset:
```python
[[1, 0, 18, 1],
 [1, 1, 15, 1],
 ...]
```

### Example Impurity Calculations:
- Gini Impurity for Feature 1:
  ```python
  calc_impurity(df[:, [0, -1]])
  ```
  Output: `{split_point: impurity}`

- Gini Impurity for Continuous Feature:
  ```python
  calc_impurity(df[:, [2, -1]])
  ```
  Output: `{best_split: lowest_impurity}`

## License
This project is licensed under the MIT License.

