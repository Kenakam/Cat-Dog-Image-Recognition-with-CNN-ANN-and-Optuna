# Cat & Dog Image Recognition with CNN, ANN, and Optuna

## 📌 Project Overview

This repository contains a comprehensive Jupyter Notebook (`Cat_&_Dog_recognition_CNN_+_ANN.ipynb`) engineered to perform binary image classification to distinguish between cats and dogs. Built entirely inside the **Google Colab** cloud ecosystem, the notebook implements deep learning architectures using **Artificial Neural Networks (ANN)** and **Convolutional Neural Networks (CNN)** via TensorFlow and Keras.

To optimize model performance, the project integrates **Optuna**, an automated hyperparameter optimization library, to seek out optimal architectural settings, dynamic layer choices, and optimizer configurations for the networks.

---

## 🛠️ Project Workflow

The analysis follows a production-ready computer vision pipeline optimized for Google Colab:

1. **Environment Setup & Google Drive Integration**:
* Installing external optimization libraries directly inside the runtime using `!pip install optuna`.
* Mounting Google Drive (`/content/drive/My Drive`) to access, stream, and store structured image dataset directories without exhausting local runtime memory spaces.


2. **Image Pre-processing & Augmentation**:
* Standardizing raw unstructured image directories into uniform geometric pixel dimensions fit for deep networks.
* Applying scaling operations, normalizing pixel variance boundaries, and configuring training/validation splits using dynamic directory parsers.


3. **Hyperparameter Optimization Suite (Optuna)**:
* Constructing automated search trials aiming to maximize model performance metrics over target validation sets.
* Testing variations in foundational image layers, multi-layer depth expansions, network widths, continuous dropout regularizations, learning rates, and core optimization functions.


4. **Model Finalization & Performance Evaluation**:
* Rebuilding and training the optimized computer vision network configurations utilizing the top parameter bounds recommended by Optuna.
* Plotting optimization convergence records and exporting final tabular prediction grids using Pandas and IPython HTML display rendering engines to observe live prediction outputs alongside test images.



---

## ⚙️ Model Limitations & Operational Constraints

* **Task-Related Thresholds**: Specific training thresholds used in this project—such as target image canvas sizes, validation split parameters, network layer depths, learning rates, or early-stopping patience counters—are **task-related thresholds**. Rather than acting as general-purpose out-of-the-box machine learning defaults, they were chosen to accommodate the exact distributions and resolution variances found in this specific cat and dog image dataset.
* **Hardware & Cloud Limitations**: While this project utilized **Google Colab's cloud environment**, training computer vision models, dense convolutional filters, and intensive iterative Optuna study loops relies heavily on volatile cloud runtime allocations. Because resource availability was tied to standard shared cloud tiers rather than dedicated hardware arrays, model performance benchmarks, learning convergence paths, and total trial capacities may reflect "not ideal" profiles. Resource constraints limited the ability to execute an exhaustive grid search or run massive cross-validation epochs across larger, more complex network architectures.

---

## 💻 Technologies Used

* **Python 3.x**
* **Cloud Platform**: Google Colab
* **Data Manipulation & Visualization**: Pandas, NumPy, Matplotlib, Seaborn, IPython Display
* **Deep Learning Frameworks**: TensorFlow, Keras (`Sequential`, Convolutional Layers, Dense Layers)
* **Hyperparameter Optimization Suite**: Optuna
* **System Integration**: Google Drive PyDrive Mount Modules

---

## 🚀 How to Use

1. **Dataset Positioning**: Upload your target training and testing animal image directories into your personal Google Drive profile (`My Drive`) under a dedicated folder structure.
2. **Environment & Execution**: Open the `Cat_&_Dog_recognition_CNN_+_ANN.ipynb` file inside your Google Colab workspace.
3. **Step-by-Step Run**:
* Execute the introductory cell to install `optuna` and complete the interactive OAuth prompt to mount your Google Drive.
* Run the rest of the notebook cells sequentially to process the image paths, kick off the automated trial loops, and display the final performance tables.


## NOTE: Because file sizes are too large, I'm providing links for them:
* training set: https://drive.google.com/file/d/1y5R514fgg2_0CQ3CZhpaW13Tn5TnUWPP/view?usp=drive_link 
* test set: https://drive.google.com/file/d/13PvSLJIvdvXQdMcGqFJMCaPOW1MQioRR/view?usp=drive_link
* single prediction: https://drive.google.com/file/d/1QWes_cjinmmz7pY3uEl6v_0DODR5_uKy/view?usp=drive_link
