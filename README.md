# Assignment-3
Topsis-for-pretrained-model
# TOPSIS-Based Selection of Pretrained Text Generation Models

This repository contains a Python implementation of the **TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution)** method to evaluate and rank pretrained text generation models. The goal is to identify the best-performing model based on multiple criteria such as **Coherence**, **Fluency**, **Relevance**, and **Perplexity**.

## Table of Contents
- [Introduction](#introduction)
- [Models Evaluated](#models-evaluated)
- [Evaluation Criteria](#evaluation-criteria)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Visualization](#visualization)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Selecting the best pretrained model for text generation can be challenging due to the variety of metrics involved. This project uses the TOPSIS method to simplify the decision-making process by ranking models based on how close they are to an ideal solution.

## Models Evaluated
The following models are evaluated in this project:
- **GPT-2**
- **GPT-2 Medium**
- **GPT-2 Large**
- **GPT-NEO**
- **T5**

## Evaluation Criteria
The models are assessed based on the following criteria:
1. **Coherence**: Logical flow and consistency of the generated text.
2. **Fluency**: Grammatical correctness and readability.
3. **Relevance**: Alignment with the prompt or context.
4. **Perplexity**: A measure of how well the model predicts the next word (lower is better).

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/NishchayJindal/topsis-text-generation.git
    cd topsis-text-generation
    ```

2. Create a virtual environment (optional but recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required libraries:
    ```bash
    pip install numpy pandas matplotlib scikit-learn
    ```

## Usage
Run the script to evaluate and rank the models:
```bash
python topsis_model_selection.py
```

The script performs the following steps:
1. Defines the models and evaluation criteria.
2. Assigns hypothetical evaluation scores.
3. Normalizes the scores using Min-Max scaling.
4. Applies the TOPSIS method to rank the models.
5. Displays the results and generates visualizations.

## Results
The output will display the TOPSIS scores and ranks for each model in a tabular format:

```
        Model  Coherence  Fluency  Relevance  Perplexity  TOPSIS Score  Rank
2   GPT-2 Large          9        9          9          15      1.000000     1
4            T5          7        9          8          16      0.547597     2
1  GPT-2 Medium          9        8          8          18      0.483426     3
0         GPT-2          8        9          7          20      0.427051     4
3       GPT-NEO          8        8          7          17      0.334709     5
```

## Visualization
The script generates the following visualizations:
1. **TOPSIS Scores Bar Chart:** Visualizes the TOPSIS scores of all models.
2. **Model Rankings Bar Chart:** Displays the rank of each model (Rank 1 being the best).

### Example Plots
- **TOPSIS Scores:**
![TOPSIS Scores](./Topsis-Score.png)

- **Model Rankings:**
![Model Rankings](./Model_ranking.png)

## Contributing
Contributions are welcome! If you have suggestions or improvements, feel free to fork the repository and submit a pull request.

## License
This project is licensed under the MIT License.

---

**Author:** Nishchay Jindal 

**Contact:** [njindal_be22@thapar.edu](mailto:njindal_be22@thapar.edu)


---

