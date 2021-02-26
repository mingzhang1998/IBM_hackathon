# IBM_hackathon: Analyzing the Characteristics of Police Shooting Incidents in Economically and Racially Different Areas with Qiskit

# Problem Statement
Police shooting has always been a critical social issue in the U.S. In this Hackathon project, using the police shootings data (victim characteristics) and the city level data (economics, education, race share), we attempt to analyze if there are significant differences in the types of shooting cases based on the socio-economics condition of the areas they happen.  
For example, one question can be, do shooting cases tend to include low threat level victims armed with non-lethal weapons in areas with more poverty and minority rate?

# Methodology

1. Clustering on the city level data. This will generate cluster zones that can be characterized based on their wealth, poverty, education level, and share of race population. Then we would like to profile the clusters or infer on the different variables and features of the shooting cases happening in those location clusters.
   - Proposed methods: Qiskit Max_Cut; K-means implementation using Qiskit; scikit-learn K-means (if Qiskit fails)
2. Run a predictive model that predict which location cluster a shooting case belongs to. The purpose is to infer on the importance of variables involved in a shooting case based on where it happened.
   - Proposed methods: Qiskit QSVM; scikit-learn Random Forest classifier (if Qiskit fails)

# Results
Three location clusters:
- Cluster A: Mostly White, high percentage completed high school
- Cluster B: Mostly Black, high poverty rate, low median income
- Cluster C: Mostly Hispanic and Asian, high median income  

Significant features of shootings in different clusters: Age, Black racial group, Hispanic racial group, Suspect mental illness

# Code files explanation:
Final version: PCA Kmeans + RF-Copy1.ipynb  
Failed attempts: quantum clustering trial 1.ipynb, quantum_clustering_trial 2.ipynb
