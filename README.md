# King County Housing EDA
This repo is about the exploratory data analysis (EDA) of a dataset of houses whcih were sold in King county between may 2014 and may 2015. For an assignment in my data science bootcamp, I have to find houses for my client, Amy Williams, who is a Mafioso and wants to sell Top 10% central houses over time and she needs average outskirt houses over time to hide from the FBI.
# Contents of this Repo

* A [Jupyter Lab Notebook](EDA-LJB.ipynb) containing fetching cleaning and analyzing the data
* A presentation of the EDA: [King-County-Housing.pdf](King-County-Housing.pdf)
* A file explaining the column names: [column_names.md](column_names.md)
* A geoJSON File of King County Zip Codes which is required for the maps:[KingCo-Zip.geojson](KingCo-Zip.geojson)
* A [requirements.txt](requirements.txt) for the library installation which will be explained in the setup below
* A [.env](.env) File in which you need to add the username and password for the database connection.



# Setup
## Venv
In order to run the Jupyter Notebook, you will have to set up a virtual environment and install the libraries in the [requirements.txt](requirements.txt).

For this you will need to: 
* set the python version locally to 3.11.3
* create a virtual environment using the `venv` module
* activate your newly created environment 
* upgrade `pip`(optional)
* install the required packages via `pip`

For plotly to run in Jupyter Lab you have to install node.js

- Check **Node version**  by run the following commands:
    ```sh
    node -v
    ```
    If you haven't installed it yet, begin at `step_1`. Otherwise, proceed to `step_2`.


### **`macOS`** type the following commands : 


- `Step_1:` Update Homebrew and install Node by following commands:
    ```sh
    brew update
    brew install node
    ```

- `Step_2:` Install the virtual environment and the required packages by following commands:

    ```BASH
    pyenv local 3.11.3
    python -m venv .venv
    source .venv/bin/activate
    pip install --upgrade pip
    pip install -r requirements.txt
    ```
### **`WindowsOS`** type the following commands :


- `Step_1:` Update Chocolatey and install Node by following commands:
    ```sh
    choco upgrade chocolatey
    choco install nodejs
    ```

- `Step_2:` Install the virtual environment and the required packages by following commands:

    ```BASH
    pyenv local 3.11.3
    python -m venv .venv
    source .venv/bin/activate
    pip install --upgrade pip
    pip install -r requirements.txt
    ```
 **`Note:`**
    If you encounter an error when trying to run `pip install --upgrade pip`, try using the following command:

   ```Bash
   python.exe -m pip install --upgrade pip
   ```

# Database connection
## .env
To be able to connect to the database and fetch the data, you will have to enter username and password into the [.env](.env) file. 

