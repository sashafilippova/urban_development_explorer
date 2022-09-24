# Urban Development Explorer

## Authors: 
- Anthony Hakim
- Marc Loeb
- Sasha Filippova
- Yifu Hou

## Project Descripion:
Our application is an interactive map displaying urban development indicators
along with varios socioeconomic indicators, intended for exploratoty data 
analysis purposes. Intended users are researchers, professionals, 
and students, who are interested in developing an intuition for the various
factors that may affect urban growth and decay.

----------------

### Running the Application Locally:

1. Create & launch a Virtual Environment with Dependencies:

```
bash install.sh
source env/bin/activate
```

2. Run the Apllication:

```
python3 urban_dev_explorer
```

> This executes our dash map with a shell script. A pop-up will direct you to the online Dash map
NOTE: use *ctrl c* to exit the application.

---------

### Testing Geocoding & Data-Wrangling Process:

Geocoding is a highly time-consuming process in the absence of a paid service.
In order to ensure that this project can be run "on the fly" geocoding was 
done in advance. The file **build_dataframes.py** accesses a geoJSON saved in 
our data folder **permits.geojson**, which contains ~44,500 geocoded building 
permits.

1. Run Testing Geocoding:

```
python3 urban_dev_explorer --test_geocode
```

> This version of the code is verbose, with a signifigant number of print 
statements to allow you to see the progress of the geocoding process. A limit of 500 has been added, instead of the full ~44,500 entries. If allowed to run to completion, a file named "perm_new.geojson" will be added to our data directory

2. Run testing of API extraction, Data Cleaning & Merging process:

```
python3 urban_dev_explorer --test_merge
```

> If allowed to run to completion, a file named **new_map_data.csv** will be added to our data directory.

----------------

## Directory:

- **requirements.txt**: list of Python packages required to run the application
- **proj-paper.pdf**: final paper describing the project overview, structure of the software, division of work, etc.
- **proj-diagram.pdf**: visual representation of the application architecture 
- **install.sh**: shell script that creates a virtual envirenment and installs required packages to run the app
- **urban_dev_explorer/**: foder containing the application. See description of the subfolders below.

#### urban_dev_exporer/:


### Data: 



### Final paper: 
https://github.com/sashafilippova/urban_development_explorer/blob/main/proj-paper.pdf
