# Hierarchical Clustering of Keystroke Data: Profiling Students in Programming Courses

This repo contains all the code used for the final project, "Hierarchical Clustering of Keystroke Data: Profiling Students in Programming Courses."

## Project summary: 

Understanding student engagement and performance can enhance learning outcomes. Traditional assessment methods often fall short in providing insights into students' behaviors and struggles. This research aims to explore how hierarchical clustering can be applied to keystroke data of a programming course to uncover insights into student engagement, coding behaviors, and learning patterns.

## Dataset:

The data used in this study was collected from a cohort of students enrolled in an introductory programming course CS1. The dataset have a rich metadata consist of submission, compilation, edit, and keystroke events (Edwards, J. (2022). 2021 CS1 Keystroke Data. Harvard Dataverse. Version V6. Available at: https://doi.org/10.7910/DVN/BVOF7S).

## Files:

- `dataset/`: Directory containing the programming keystroke dataset from the CS1 course.
- `features_results/`: Directory containing the features extracted from the keystrokes data. I choose 12 features for clustering: error count, number of compilation, mean time difference be-
tween two consecutive compilations, number of short, medium, and long pauses during, number of semicolon, number of ”print”, ”while”, ”for”, and ”space” keys, and total number of keystrokes frequency for each student per assignment.
- `hierarchical_clustering.ipynb`: Script for extracting the features and implementing clustering methiods.

## Clustering Results:

I used four different methods for clustering: Hierarchical (Agglomerative) Clustering with PCA, Hierarchical (Agglomerative) Clustering with t-SNE, K-Means Clustering with PCA, and K-Means Clustering with t-SNE.
The results are as follow:

#### 1. Hierarchical (Agglomerative) Clustering with PCA
<img src="https://github.com/user-attachments/assets/79c2a936-0d6d-4902-b345-d6b09419eae3" alt="dendrogram_ac_pca" width=50% height=50%/>
<img src="https://github.com/user-attachments/assets/7055e851-6721-4287-aa2e-e6df50d80cb3" alt="clusters_ac_pca" width=50% height=50%/>

#### 2. Hierarchical (Agglomerative) Clustering with t-SNE
<img src="https://github.com/user-attachments/assets/7c50a55f-72c3-4802-be4e-25e099eefb59" alt="dendrogram_ac_tsne" width=50% height=50%/>
<img src="https://github.com/user-attachments/assets/f53eef16-e2c5-431a-adc0-1ed29da30e53" alt="clusters_ac_tsne" width=50% height=50%/>

#### 3. K-Means Clustering with PCA
<img src="https://github.com/user-attachments/assets/d0d6e103-2b82-4f87-a424-26b795b66049" alt="clusters_kmeans_pca" width=50% height=50%/>

#### 4. K-Means Clustering with t-SNE
<img src="https://github.com/user-attachments/assets/0b1ccd8c-85ac-44be-b4f3-8a971c70da0b" alt="clusters_kmeans_tsne" width=50% height=50%/>









