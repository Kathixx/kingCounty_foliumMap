
## Data of KingCounty
In this example with folium, we're working with the King County dataset (look in folder: data) as well as the geojson-data of the King County Zipcodes.
The GeoJson Data came from [this page](https://gis-kingcounty.opendata.arcgis.com/datasets/zipcodes-for-king-county-and-surrounding-area-shorelines-zipcode-shore-area/about).
They are already saved as .geojson and .csv in the ```geodata```folder

## Using Folium and Choropleth
We want to create a map with different layers, which I can manually activate (like colorized shapes, makers and so on). We want to show the top ten most expensive zipcodes and then, in those zipcodes, show in different color the houses, depending on the number of bedrooms.


1. Prepare the data: load geojson data
2. Perpare Data: top 10 most expensive, house makers
3. Create a folium map
4. Create different Choropleth-Layers [see also here](https://python-visualization.github.io/folium/latest/user_guide/geojson/choropleth.html)
5. Create a Cluster Marker Object [see also here]()
6. Create different House Makers, depending on bedrooms [see also here](https://python-visualization.github.io/folium/latest/user_guide/vector_layers/circle_and_circle_marker.html)
7. Create a legend to the map [see also here](https://www.geeksforgeeks.org/create-a-legend-on-a-folium-map-a-comprehensive-guide/)
8. Add a minimap [see also here](https://python-visualization.github.io/folium/latest/user_guide/plugins/mini_map.html)
9. Safe the Map to html



## Setup

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

- `Step_2:` Install the virtual environment and the required packages by following commands.

   For `PowerShell` CLI :

    ```PowerShell
    pyenv local 3.11.3
    python -m venv .venv
    .venv\Scripts\Activate.ps1
    pip install --upgrade pip
    pip install -r requirements.txt
    ```

    For `Git-Bash` CLI :
  
    ```BASH
    pyenv local 3.11.3
    python -m venv .venv
    source .venv/Scripts/activate
    pip install --upgrade pip
    pip install -r requirements.txt
    ```
 

 **`Note:`**
    If you encounter an error when trying to run `pip install --upgrade pip`, try using the following command:

   ```Bash
   python.exe -m pip install --upgrade pip
   ```

