# ARIN-5101-Project
ARIN 5101 Project

# Latest description
The project now loads the CIFAR100 filter a subset of 10 classes base of the config and train the basline CNN model.

The baseline model is a simple CNN with two convolutional layers followed by dense layers for classification.

Then the model and the traing result are saved in the `./models` and `./reports` respectively.

Base on the config, the code might no taring the model and instead, only load the model and report from `./models` and `./reports`


# Basic env setup
To start the project locally:
```bash
conda env create -f environment.yml
```
or to update the env
```bash
conda env update -f environment.yml  --prune
```

Then 
```bash
conda activate Arin5101Proj
```

# How to train
Setting `"force_train": true` in `config.json` will always retrain the model and save the new result.

If a new subset is given and no model for this subset can be found, it would also train a new model.
