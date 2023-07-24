# Background
The goal is to get Louisville restaurant data and louisville inspection data from Open Portal to discover if there's any correlation or relationship.

Sources:
 - Yelp API (returns 1000 businesses)
    - Yelp's API will only allow to return 1000 businesses
 - Louisville Restaurant Inspection Scores: https://data.louisvilleky.gov/datasets/LOJIC::louisville-metro-ky-restaurant-inspection-scores/about
    - Data is only for the last year


# Features Used

1. Read data in
   * Read in excel file
   * Extract data from Yelp API
2. Manipulate and clean data
   * Used pandas to merge two datasets
   * Drop columns, change strings to lowercase
3. Visualize your data
   * Created a choropleth map
   * Created a pairplot
   * Created a scatterplot
4. Interpret your data
   * Please view interpretation of data at the very bottom of [analysis.ipynb](analysis.ipynb) 

# Usage

Follow these steps to run the program on your local machine:
* Clone project:
  * Open desired terminal
  * cd to desired location
  * run `git clone git@github.com:mary-vo/inspection.git`
* Open project in Visual Studio:
  * Open Visual Studio > File > Open Folder... > Navigate to location where project was cloned > click "Select Folder"
* Create and activate a virtual environment
  1. In terminal, type: `python -m venv venv`
  2. Activate the virtual environment, commands vary based on terminal:
     * bash: `source venv/Scripts/activate`
     * powershell: `.\venv\Scripts\activate`
     * command prompt: `venv\Scripts\activate`
* While in the root directory, run `pip install -r requirements.txt`
* Open [analysis.ipynb](analysis.ipynb) by selecting it in the Explorer pane of VSCode
* Select Kernel (top right of notebook) > Python Environments... > venv
* Add API Key in [analysis.ipynb](analysis.ipynb) (see text file provided via Slack). Note: search for *"Authorization": "Bearer "*; insert key after 'Bearer '
* Click on the first cell > select "Run All" button