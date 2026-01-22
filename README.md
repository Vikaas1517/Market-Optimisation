🛒 Market Basket Analysis using ECLAT & FP-Growth
📌 Overview

This repository implements Market Basket Analysis using two efficient frequent pattern mining algorithms:
ECLAT (Equivalence Class Transformation) and FP-Growth (Frequent Pattern Growth).

The project focuses on discovering frequent itemsets from transactional datasets to support market optimisation, including product placement, cross-selling, promotions, and inventory management.

🎯 Objectives

Discover frequently co-purchased items

Compare performance of ECLAT vs FP-Growth

Improve market optimisation strategies

Reduce computational cost compared to Apriori

Extract actionable insights from large transaction datasets

🧠 Algorithms Used
🔹 ECLAT (Equivalence Class Transformation)

Uses vertical data representation (TID sets)

Support calculated via set intersection

Depth-first search traversal

Efficient for dense datasets

🔹 FP-Growth (Frequent Pattern Growth)

Uses a compact FP-Tree structure

Avoids candidate generation

Faster than Apriori for large datasets

Efficient for sparse and large-scale data

📊 Algorithm Comparison
Feature	ECLAT	FP-Growth
Data Format	Vertical	Tree-based
Candidate Gen	Yes (implicit)	No
Memory Usage	Moderate	Efficient
Best For	Dense data	Large datasets
Speed	High	Very High

🛠️ Technologies Used

Python

Pandas

NumPy

itertools

mlxtend (for FP-Growth, optional)

⚙️ Installation
git clone https://github.com/your-username/Market-Basket-Analysis.git
cd Market-Basket-Analysis
pip install -r requirements.txt

▶️ Usage
Run ECLAT
python src/eclat.py

Run FP-Growth
python src/fp_growth.py


You can configure:

Minimum support threshold

Input dataset

Output file format

📈 Output

Frequent itemsets with support values

Comparative insights from both algorithms

Useful for:

Product bundling

Shelf layout optimisation

Targeted promotions

Recommendation systems

🚀 Applications

Retail & E-commerce analytics

Recommendation engines

Customer behaviour analysis

Inventory and demand optimisation

Business intelligence systems

📌 Future Enhancements

Association rule mining (confidence, lift, conviction)

Visualisation dashboards

Real-time transaction streaming

Performance benchmarking on large datasets

Integration with ML-based recommenders

🤝 Contributing

Contributions are welcome!
Feel free to fork the repository, improve the algorithms, and submit a pull request.
