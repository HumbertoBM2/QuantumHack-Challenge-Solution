<div align="center">

# Solution to IBM's 2023 QuantumHack Challenge

##### Jupyter Notebook where team 8 applied basic quantum computing and Python to solve an optimization problem.

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Qiskit](https://img.shields.io/badge/Qiskit-%236929C4.svg?style=for-the-badge&logo=Qiskit&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)

</div>

## Team 8 

- Humberto Barrera Martínez
- Miguel Ángel González Gutierrez
- Pedro Antonio González Soto
- Alejandro Emilio Novales Treviño

## Overview 

The challenge involves creating a program that, utilizing Quantum Computing, determines the optimal route passing through a given set of points. The provided Jupyter Notebook offers a solution to this challenge, employing the TSP Solver with VQA to address each cluster and utilizing KMeans for cluster generation and solving.

The primary code to tackle the challenge is found in the first cell, while the subsequent cells feature test codes used during the development process. For the purpose of understanding and addressing the problem at hand, these test codes can be disregarded.

Our approach to solving this problem involved dividing the entire system of points into n clusters, each containing 4 points. We opted for this approach because when converting the nodes into a matrix, the numpy library struggles to handle matrices with dimensions equal to or larger than 6x6. This limitation influenced our decision, along with the constraint of limited resources for testing, preventing us from applying the TSP solver algorithm to clusters with 5 points due to insufficient RAM.

However, the use of a quantum computer presented a potential solution. Quantum computing allows for more flexible modifications to the cluster sizes through the Kmeans algorithm, leveraging the enhanced processing power to achieve a more efficient classification and solution for each subsystem of points.
