# Urban poverty mapping from satellite imagery

## Project overview
This repository contains the final project for the **Deep Learning for Social Sciences** course (2025). 

It's often hard and expensive to collect poverty data using traditional surveys. This project looks at a faster and cheaper way: using **Convolutional Neural Networks (CNNs)** to find and map poverty levels directly from satellite pictures.

We used poverty data and satellite images from **Nigeria**. The models group different areas into four poverty levels. We also built a model to predict exact poverty scores. To see if the models work in the real world, we tested them on new data from **Kenya**.

---

## About This Project
This was a group project that I took part in. It was a very interesting project because it showed me how we can use computer vision to help solve real-world problems. Working on this project taught me a lot about how helpful AI can be for society, but also how difficult it can be to work with satellite data from different countries.

---

## Models We Used

We tried and compared a few different deep learning models to see which one worked best:

1. **Baseline CNN:** A simple model we built from scratch to use as a starting benchmark.
2. **ResNet50 (Pretrained):** A powerful, ready-made model that already knows how to recognize shapes and features.
3. **ResNet50 (Fine-tuned in 1 Step):** We took the ResNet50 model and trained the whole thing on our satellite pictures.
4. **ResNet50 (Fine-tuned in 2 Steps):** We trained this model in two stages to get better results.
5. **Regression Model:** A model used to predict exact, continuous poverty scores instead of just grouping them into classes.

---

## Repository Structure

The folders in this repository are organized like this:

```text
├── Final Report.pdf            # The full report with our findings
├── Code/                       # All the code and Jupyter notebooks
│   ├── Data/
│   │   ├── Data Collection/
│   │   │   ├── Poverty Data    # Code to get poverty data for Nigeria and Kenya
│   │   │   └── Satellite Images# Code to get satellite images for Nigeria and Kenya
│   │   └── Data Cleaning/      # Code used to clean the data for both countries
│   └── CNN Models/             # Code used to build, train, and test the models
│       ├── Classification.ipynb
│       └── Regression.ipynb
└── Data/                       # The datasets we used
    ├── Poverty Data/           # CSV files with poverty scores
    └── Satellite Images/       # Metadata and ZIP files with the cleaned images


