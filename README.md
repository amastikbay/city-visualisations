# City Network Visualization

This repository contains a Jupyter Notebook (city_viz.ipynb) that downloads, processes, and visualizes the street network of a city using OSMnx, GeoPandas, and Matplotlib. It focuses on simplifying intersections and producing high-quality visual maps of the selected urban area.

# Features

1. Automated City Download: Fetches street network data from OpenStreetMap using OSMnx.

2. Custom CRS: Allows selection of projection (EPSG code).

3. Intersection Simplification: Consolidates close nodes into true intersections for cleaner visualization.

4. Dual Layer Visualization: Shows both the original and simplified network layers with color-coded styling.

5. High-Resolution Export: Saves the final plot as a .png file with customizable styling.

# Installation

pip install osmnx geopandas seaborn matplotlib

# Usage

Open city_viz.ipynb in Jupyter Notebook
Change the cityname variable to your desired location, for example:
cityname = 'Milan, Italy'
crs = 'EPSG:4326'
Run all cells to:
Download the graph
Simplify intersections
Convert to GeoDataFrames
Plot and export the visualization

# Output Example

Running the notebook with cityname = 'Milan, Italy' produces a high-resolution map (milan_graph.png) like:

White lines → original street network
Red points → original nodes
Yellow lines → simplified street network
Blue points → simplified intersections

# Requirements

Python 3.8+

**Packages:** osmnx, geopandas, matplotlib, seaborn

# Notes

Intersection simplification tolerance can be adjusted for different mapping precision.
The script works best for small to medium-sized cities; large metropolitan areas may require additional memory and processing time.
