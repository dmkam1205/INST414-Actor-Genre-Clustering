# Actor Genre Clustering Analysis

This repository contains the code and data for my INST414 clustering assignment.

## Project Question

Can actors be grouped into meaningful career archetypes based on the distribution of genres in which they have appeared?

## Data

The actor-by-genre dataset was constructed from raw IMDb movie records covering movies from 2000 through 2022.

Each row represents an actor and each column represents a genre. The values represent how many times an actor appeared in movies associated with each genre.

## Method

The analysis:

- Constructs an actor-by-genre matrix from raw IMDb JSON data
- Applies row-level L1 normalization
- Uses the elbow method to select a value for k
- Applies K-Means clustering with k = 8
- Examines cluster centroids and representative actors
- Validates cluster assignments and cluster sizes

## Files

- `actor_genre_clustering.ipynb` - full analysis
- `constructed_actor_genre_matrix.csv` - constructed actor-by-genre dataset
- `actor_cluster_assignments.csv` - actor cluster assignments
- `cluster_summary.csv` - cluster summary results
- `actor_cluster_elbow.png` - elbow-method visualization
- `actor_cluster_sizes.png` - cluster-size visualization
