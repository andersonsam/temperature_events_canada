# Analysis of the streamflow response to multi-day warm anomaly events across Canada 

This code accompanies the paper:  

Anderson, S. and Chartrand, S. "The streamflow response to multi-day warm anomaly events: Sensitivity to future warming and spatiotemporal variability by event magnitude". Earth's Future. (2024)  

This study identifies the streamflow repsonse to normal, warm, and hot temperature events from 1981 - 2020 across 868 basins in Canada.  Then, we use climate reanalysis data to understand how such streamflow responses are sensitive to warmer annual temperatures.  

_____
## Data

We use the [Caravan](https://www.nature.com/articles/s41597-023-01975-w#Bib1) dataset, which contains streamflow observations (from [HYSETS](https://www.nature.com/articles/s41597-020-00583-2)), basin-averaged meteorological data (from [ERA5-Land](https://essd.copernicus.org/articles/13/4349/2021/)), and basin attributes (from [HydroATLAS](https://www.nature.com/articles/s41597-019-0300-6)).

The [Caravan dataset](https://zenodo.org/records/7944025) can be downloaded and stored locally for the analysis.
_____
## Running the Code  

In terminal, navigate to your desired directory for the code and run:  

>git clone https://github.com/andersonsam/temperature_events_canada

Create virtual environment:  

>conda env create -f environment.yml

Activate the environment:  

>conda activate temperature_events_canada

Open in Jupyter Lab:  

>jupyterlab

### Required libraries  

The following are specified in the environment.yml file:  
  - geopandas = 0.12.1
  - jupyterlab = 3.5.0
  - matplotlib = 3.6.2
  - numpy = 1.23.4
  - pandas = 1.5.1
  - python = 3.10.6
  - scipy = 1.9.3
  - shapely = 1.8.5

### Directory structure  

- environment.yml
- main.ipynb
- Data
  - Caravan
    - attributes
      - hysets
    - timeseries
      - csv
        - hysets    
