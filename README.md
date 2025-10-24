ChemTwin — Molecular Similarity Analyzer
- A chemoinformatics tool for detecting structural similarity between two compounds, identifying matching atoms, and calculating the Tanimoto similarity score.
Built with RDKit for molecular fingerprinting, substructure matching, and visualization.

* Table of Contents
Overview
Key Features
Requirements
Installation
Usage
Example Code
Understanding the Output
Roadmap
Contributing & License
Contact

>> Overview

ChemTwin is a lightweight and practical chemoinformatics analysis tool that compares two molecules at both structural and quantitative levels.
It can:
1- Detect whether one molecule is a substructure of another (HasSubstructMatch, GetSubstructMatch), and return a tuple of the matching atom indices.
2- Compute molecular similarity using Morgan fingerprints and the Tanimoto coefficient.
3- Classify the similarity level (e.g., nearly identical, highly similar, moderately similar, or different).
4- Generate 2D visualizations of both molecules side-by-side (and optionally highlight the matching atoms).
Note: This tool is rule-based and analytical — it is not a machine learning model ( yet ! ).


>> key Features

1- Substructure matching: Identify if one molecule contains the other and list matching atom indices.
2- Fingerprint similarity: Compute Morgan fingerprints (radius = 2) and Tanimoto similarity.
3- Automatic classification: Label the similarity level based on the Tanimoto score.
4- 2D visualization: Display both compounds side by side using RDKit.
4- (Optional) Generate 3D coordinates and visualize with py3Dmol.

>> Installation

1 - Create a new conda environment and install RDKit.
2 - Clone the repository:
git clone https://github.com/yourusername/chemtwin.git
cd chemtwin
3- Run the script or open the Jupyter notebook for testing.


>>  Usage

You can open and run the project directly on Google Colab:
[![Open In Colab](https://colab.research.google.com/drive/1-SqBM9hNiZPt7qM8O6NISHmeSgRtK9YY?authuser=0#scrollTo=o-YslmOo8eXk)

>> Practical Example: Doxorubicin vs Daunorubicin

You can input the actual SMILES of Doxorubicin and Daunorubicin,
then follow the same steps to check:

Structural submatch
Atom index alignment
Tanimoto similarity percentage and classification

>> Tips
Use Morgan fingerprints (radius=2) for general structural similarity.
For subtle functional group differences, experiment with other fingerprint types.
Remember: Tanimoto similarity is statistical, not necessarily biological similarity.

>> Contributing

Contributions are welcome!
Feel free to open issues or submit pull requests.
Please include clear descriptions and runnable examples.

>> License

MIT License — You’re free to use, modify, and distribute the code with proper attribution.

>> Contact

Author: Mohamed Zaghloul
Email : zaghloulmohamed741@gmail.com
