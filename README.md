# SC4000: PetFinder.my Pawpularity Contest

## Project Overview

This repository contains the work of my group for SC4000 Machine Learning for the [PetFinder.my Pawpularity Contest](https://www.kaggle.com/c/petfinder-pawpularity-score) on Kaggle.

PetFinder.my is Malaysia’s leading animal welfare platform. The goal of this competition was to develop a machine learning model that analyzes raw images and metadata to accurately predict the “Pawpularity” score of pet photos, helping to improve animal adoption rates.

## Team Members
- Shao Wen
- Jun Kai
- Shermaine
- Jefferson
- Amy (me)

## My Contribution 
I focused on the model optimization phase of the project. I implemented hyperparameter tuning using Scikit-Learn's GridSearchCV and RandomizedSearchCV to systematically explore the parameter space of our models. This process was a significant learning experience because I was unfamiliar with Github and Python at the time. It took a lot of researching to understand what I was supposed to tackle. While the resulting performance gains on our specific models were marginal, it provided important hands-on experience in a key aspect of the machine learning workflow and helped the team rule out certain configurations.

## Repository Structure & Development Workflow

Our team adopted a feature-branch workflow to explore a wide range of approaches to this complex problem. The `main` branch is kept clean as a starting point.

**To explore our work, please navigate to the respective branches using the branch dropdown menu on GitHub.**

*   **`branch-1: preprocessing-augmentation`**
    *   Contents: The preprocessing of provided CSV metadata and performing image augmentation techniques to expand and enhance the training dataset.

*   **`branch-2: model-implementation`**
    *   Contents: Implementation of several core model architectures (e.g. CNNs) to establish baseline performance metrics for the project.

*   **`branch-3: hyperparameter-tuning`**
    *   Contents: Experiments with hyperparameter tuning on existing models. This branch also served as a collaborative hub for sharing model files and architectures. *(Note: This branch contains experimental code and is reflective of an iterative development process.)* 

## Key Findings & Results

Our team investigated multiple approaches, including data augmentation, various model architectures, and hyperparameter tuning.

*   **Result:** The performance, measured by Root Mean Squared Error (RMSE), across our different models was ultimately very similar.
*   **Conclusion:** Our experiments suggested that the marginal gains from hyperparameter tuning on our chosen architectures were limited. The challenge likely resided in the "Pawpularity" target itself.
*   **Performance:** Our final model scores placed us below the 50th percentile on the Kaggle leaderboard, indicating that while we built a functional pipeline, more sophisticated approaches were required for optimized performance.

## Lessons Learned

This project was an invaluable learning experience in the end-to-end process of a machine learning competition:

1.  **Importance of a Solid Baseline:** We learned that establishing a strong baseline model is crucial before investing significant time in hyperparameter tuning.
2.  **Collaboration with Git:** This project served as my introduction to using Git and GitHub for collaboration. It was challenging to figure out how to merge work and maintaining a clean structure.
3.  **Facing Reality:** Documenting and understanding why an approach didn't work is just as important as documenting success. I think we got to the point of overfitting our parameters and not focusing on other problems within our methodology that resulted in a low score.
4.  **Problem Analysis:** I gained insight into how the nature of the target variable (a subjective and abstract "Pawpularity" score) can be a major limiting factor in model performance.
