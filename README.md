# Flight Route Visualizer

## Overview
This project provides an interactive web map visualizing flight routes using MapLibre GL JS. It fetches route data from a JSON file and displays the flight paths as arcs using `turf.greatCircle`. Each airport is marked on the map, showing its name and code. The map also includes an attribution to GCMap for data sourcing.

## Features
- Interactive map with zoom and pan functionalities.
- Flight routes are represented as arcs for a realistic globe projection.
- Airports are marked with clickable icons, displaying airport codes and names.
- Custom attribution for data source.

## Usage

### Generate route json
Run the get_flight_data.ipynb notebook to generate the json file, set the `flight_str` from your own flight data.

### View map
To view the map, open the `index.html` file in a web browser. Ensure an active internet connection for MapLibre GL JS and the data source (at `fetch('/flight.json')`).

You can change the map style by changing the `style` property of the `map` object in `index.html` and the url in `raster-tiles`. See MapLibre GL JS documentation for more information.

## Credits
Data sourced from [GCMap](http://www.gcmap.com/).

