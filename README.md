# Customer Price Prediction MLOps Project

This project aims to predict customer prices using a machine learning pipeline orchestrated with ZenML, tracked and logged using MLflow, and deployed with a Streamlit app for interactive user interface.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Technologies Used](#technologies-used)
3. [Project Structure](#project-structure)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Contributing](#contributing)
7. [License](#license)

## Project Overview

Customer Price Prediction is a critical component for businesses to strategize their pricing models. This project automates the machine learning workflow, from data ingestion to model deployment, ensuring reproducibility and scalability.

### High Level Overview

![High Level Overview](https://github.com/jayanth119/DeliveryMlops/blob/main/_assets/high_level_overview.png)

### Training and Deployment Pipeline

![Training and Deployment Pipeline](https://github.com/jayanth119/DeliveryMlops/blob/main/_assets/training_and_deployment_pipeline_updated.png)

## Technologies Used

- **ZenML**: For orchestrating the machine learning pipeline.
- **MLflow**: For tracking experiments, logging models, and managing lifecycle.
- **Streamlit**: For creating an interactive web application to showcase model predictions.

## Project Structure

```
customer-price-prediction/
│
├── data/
│   ├── olist_customers_dataset.csv                 # Raw data files
│   
│
│
├── src/
│   ├── data_ingestion.py    # Script for data ingestion
│   ├── preprocessing.py     # Script for data preprocessing
│   ├── training.py          # Script for model training
│   ├── evaluation.py        # Script for model evaluation
│   ├── deployment.py        # Script for model deployment
│
├── streamlit_app.py         # Streamlit app script
│
├── zenml_pipeline.py        # ZenML pipeline definition
│
├── mlflow_experiments/      # MLflow experiment logs
│
├── requirements.txt         # Python dependencies
│
├── README.md                # Project README file
│
└── .gitignore               # Git ignore file
```

## Installation

To get a copy of this project up and running on your local machine, follow these steps:

1. **Clone the repository**
   ```bash
   git clone https://github.com/jayanth119/DeliveryMlops
   cd DeliveryMlops 
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Install ZenML**
   ```bash
   pip install zenml
   zenml init
   ```

5. **Install MLflow**
   ```bash
   pip install mlflow
   ```

6. **Install Streamlit**
   ```bash
   pip install streamlit
   ```

## Usage

1. **Run the ZenML pipeline**
   ```bash
   python zenml_pipeline.py
   ```

2. **Track experiments with MLflow**
   Start the MLflow server:
   ```bash
   mlflow ui
   ```
   Access the MLflow UI at `http://localhost:5000`.

3. **Launch the Streamlit app**
   ```bash
   streamlit run streamlit_app.py
   ```
   Access the Streamlit app at `http://localhost:8501`.

## Contributing

We welcome contributions to enhance the functionalities and features of this project. Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Feature Importance

![Feature Importance](https://github.com/jayanth119/DeliveryMlops/blob/main/_assets/feature_importance_gain.png)

---

Feel free to customize this template to fit your project's specific details and requirements.
