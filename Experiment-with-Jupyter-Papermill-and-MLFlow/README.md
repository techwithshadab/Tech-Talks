# Experiment-with-Jupyter-Papermill-and-MLFlow
Simple data science experimentation with `jupyter`, `papermill`, and `mlflow`

Machine Learning and AI are changing or would say have changed the way how businesses used to behave. However, the Data Science community is still lacking good practices for organizing their projects and effectively collaborating and experimenting quickly to reduce “time to market”.

During this session, we will learn about such open-source tools like “papermill” and “mlflow” which can help you in helping ML models shareable and reproducible. It is designed to handle large files, data sets, machine learning models, metrics as well as code

### Slides- [Experiment with Jupyter, Papermill, and MLFlow](https://speakerdeck.com/shadab96/experimentation-with-jupyter-papermill-and-mlflow)

---

# Quick-start

- Clone this repo

```
git clone git@github.com:shadab-entrepreneur/Tech-Talks.git
```
- Set up virtualenv

```
cd Tech-Talks/Experiment-with-Jupyter-Papermill-and-MLFlow

# Create virtualenv based on requirements.txt
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

# Install kernelspec for Jupyter notebooks (the name argument must be identical)
python -m ipykernel install --user --name=papermill-mlflow
```

- Start Jupyter notebook

```
cd notebooks
jupyter notebook
```

- Run the cells in `papermill.ipynb`

![image of runner notebook](https://github.com/shadab-entrepreneur/Tech-Talks/blob/master/Experiment-with-Jupyter-Papermill-and-MLFlow/assets/papermill.png)

- Start MLflow (in another terminal)

```
# Open another terminal

# Activate the virtualenv
cd papermill-mlflow
source venv/bin/activate

# Start the mlflow server
cd notebooks
mlflow server
```

- Access the MLflow UI opening this in a browser: [http://127.0.0.1:5000](http://127.0.0.1:5000/#/experiments/1)
    - Navigate to "stock_up_down" in the experiment tab if necessary

![image of mlflow](https://github.com/shadab-entrepreneur/Tech-Talks/blob/master/Experiment-with-Jupyter-Papermill-and-MLFlow/assets/mlflow.png)
