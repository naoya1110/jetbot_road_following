# AIでロボットを走らせよう


## Setup
1. Log in to your JetBot from a web browser.
1. Open a terminal and log in via SSH
    ```
    ssh jetbot@0.0.0.0
    ```
1. Then navigate to `workspace/jetbot/notebooks` directory.
    ```
    cd jetbot/notebooks
    ```
1. Clone this repository.
    ```
    git clone https://github.com/naoya1110/jetbot_road_following.git
    ```

## Data Collection
1. Navigate to `workspace/jetbot/notebooks/jetbot_road_following` directory in the file browser.
1. Open `01_data_collection.ipynb`
1. Perform data collection by following instructions in the notebook.
1. Download `dataset.zip` to your local PC.

## Model Training
1. Open `02_train_model_resnet18.ipynb` in Google Colab from [here](https://colab.research.google.com/github/naoya1110/jetbot_road_following/blob/main/02_train_model_resnet18.ipynb)
1. Upload `dataset.zip` by using the file browser in Google Colab.
1. Train a model with Google Colab by following instructions in the notebook.
1. Download `best_model_resnet18.pth` to your local PC

## Live Demo
1. Upload `best_model_resnet18.pth` to `workspace/jetbot/notebooks/jetbot_road_following` directory in your JetBot
1. Open `03_live_demo_resnet18_trt.ipynb`
1. Run your JetBot with the trained model by following the instructions in the notebook.
