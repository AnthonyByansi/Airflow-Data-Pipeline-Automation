# Airflow Data Pipeline Automation

This project provides a workflow using Apache Airflow to automate the data pipeline for a specific use case. The purpose of this project is to demonstrate how Airflow can be used to automate the process of extracting, transforming, and loading data from various sources into a data warehouse or data lake.

## Getting Started

To get started with this project, you will need to have Apache Airflow installed on your system. You can follow the installation instructions provided by the official Airflow documentation [here](https://airflow.apache.org/docs/apache-airflow/stable/start/index.html).

Once you have Airflow installed, you can clone this repository to your local machine and create a new virtual environment using the requirements.txt file provided:
```bash
$ git clone https://github.com/AnthonyByansi/airflow-data-pipeline-automation.git
$ cd airflow-data-pipeline-automation
$ python -m venv venv
$ source venv/bin/activate
$ pip install -r requirements.txt
```

Next, you can initialize the Airflow database and start the Airflow web server: 
```bash
$ airflow db init
$ airflow webserver --port 8080
```

Finally, you can trigger the DAG by navigating to the Airflow web interface at `http://localhost:8080` and clicking on the "Trigger DAG" button. This will start the process of extracting, transforming, and loading data according to the specific use case defined in the DAG.


## Contributing

If you are interested in contributing to this project, please feel free to submit a pull request. We welcome contributions of all kinds, including bug fixes, new features, and documentation improvements.

Before submitting a pull request, please make sure to run the tests and format your code using `flake8` and `black`:
```bash
$ pytest
$ flake8
$ black .
```
## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/AnthonyByansi/Airflow-Data-Pipeline-Automation/blob/main/README.md) file for details.
