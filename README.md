# Assignment 2

#  Geospatial data exploration tool using FastAPI


[![PyPI](https://img.shields.io/pypi/pyversions/locust.svg)](https://pypi.org/project/locust/)



# Codelabs link

[Code Labs Link](https://codelabs-preview.appspot.com/?file_id=1y1sR16fZI4Q3GLiPGJNYOEjKz8O3YQqyQOw4OWxb4xc#2)




# Process Outline

1. Data Fetching using FastAPI 
2. Using AWS Logger to keep the track of the API Calls Made
3.Using Streamlit to handle the UI part which enables users for Login and registration to fetch the Metadata
4. Building a Airflow DAGs to automate the process of updating the metadata file on regular interval of time and using great expectation module to ensure data quality
5. Used Docker to containerize the UI and Backend which communicate with each other upn the user request 
6.Deploying the model on AWS fot publically accessible





## How to use  this project:


1. Use Main2 branch to Clone the repo locally `git clone <repo-url>`

2. Setup the local python enviornment.

3. Install all the dependencies from the requirements.txt file
`pip install -r requirements.txt`

4. Install all local dependencies 
`pip install -e .`

5. Create `.env` file.

6. Update the specified key value pair in .env to get detailed logs of the Applications

AWS_ACCESS_KEY_ID 

`AWS_ACCESS_KEY=<value>`

`AWS_ACCESS_KEY_SECRET=<value>`

`AWS_ACCESS_KEY_SECRET=<value>`

`LOG_GROUP_NAME` 

`LOG_STREAMLIT_NAME `

7. Run the streamlit project
`streamlit run ui/main.py`










### Team Member

| NUID | Team Member       |
|:-----:|---------------|
| 002766036       | Anuj Kumar |
| 002794258      |  Hitesh  Pant            |
| 002773080      |  Kunal Bhoyar              |
| 002772221      |  Snehashis Lenka              |
