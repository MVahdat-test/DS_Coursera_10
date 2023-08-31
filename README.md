# DS_Coursera_10
In this capstone assignment, we will be working
with SpaceX launch data that is gathered from an API, specifically the SpaceX REST API. This API will give us data about launches,
including information about the rocket used, payload delivered, launch specifications,
landing specifications, and landing outcome. Our goal is to use this data to predict whether
SpaceX will attempt to land a rocket or not. The SpaceX REST API endpoints, or URL, starts
with api.spacexdata.com/v4/. We have the different end points, for example: /capsules and /cores We will be working with the endpoint api.spacexdata.com/v4/launches/past. Let’s see how the API works. We will use this URL to target a specific
endpoint of the API to get past launch data. We will perform a get request using the requests
library to obtain the launch data, which we will use to get the data from the API. This result can be viewed by calling the .json()
method. Our response will be in the form of a JSON,
specifically a list of JSON objects. Since we are using an API, you will notice
in the lab that when we get a response it is in the form of a JSON. Specifically, we have a list of JSON objects
which each represent a launch. To convert this JSON to a dataframe, we can
use the json_normalize function. This function will allow us to “normalize”
the structured json data into a flat table. This is what your JSON will look like in a table
form. Another popular data source for obtaining
Falcon 9 Launch data is web scraping related Wiki pages. In this lesson, you will be using the Python
BeautifulSoup package to web scrape some HTML tables that contain valuable Falcon 9 launch
records. Then you need to parse the data from those
tables and convert them into a Pandas data frame for further visualization and analysis. We want to transform this raw data into a
clean dataset which provides meaningful data on the situation we are trying to address: Wrangling Data using an API, Sampling Data, and Dealing with Nulls. You will notice, in some of the columns, like
rocket, we have an identification number, not actual data. This means we will need to use the API again
targeting another endpoint to gather specific data for each ID number. These functions are already created for you,
and will use the following: Booster, Launchpad, payload, and core. The data will be stored in lists and will
be used to create our dataset. Another issue we have is that the launch data
we have includes data for the Falcon 1 booster whereas we only want falcon 9. In this lab, you will need to figure out how
to filter/sample the data to remove Falcon 1 launches. Finally, not all gathered data is perfect. We may end up with data that contains NULL
values. We must sometimes deal with these null values
in order to make the dataset viable for analysis. In this case, we will deal with the NULL values
inside the PayloadMass. In this lab, you must figure out a way to
calculate the mean of the PayloadMass data and then replace the null values in PayloadMass
with the mean. We will leave the column LandingPad with NULL
values, as it is represented when a landing pad is not used. This will be dealt with using one hot encoding
later on.
