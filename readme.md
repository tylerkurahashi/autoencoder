## Pre-requisition

Please follow one of the options below to prepare your environment.

1. If you have docker environment in your machine.

- `docker-compose up -d`

- Access `localhost:8888` from your browser.

After it is up, check your token from the container logs to log in to the Notebook server.
- `docker container logs [container name]`
container name is probably `autoencoder_notebook_1`



2. Please enter the command below to create the necessary environment.

`conda env create -f=torch_env.yml`

3. Or prepare the following libraries respectively.
- pytorch=1.10
- torchvision=0.11.1
- scikit-learn=1.0.1
- numpy=1.21.2
- pandas=1.3.4
- matplotlib=3.4.3
- seaborn=0.11.2

## How to Use

Each jupyter notebook is capable of..
#### evaluation.ipynb
- Check Training Process (Loss Curves, Accuracy Curves)
- Check Final Result against Test dataset.

#### infer.ipynb
- Check the input and output of AutoEncoder and compare.
- Perform Classification inference against test dataset images one by one.
(Comparing ground truth and prediction.)