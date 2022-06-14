# StarMapGenerator

A python script for plotting Star Maps with data from the Skyfield API. This outputs a customisable poster in PNG format.

----
This script takes an input of geographic location, based on a decimal Lat/Long, and a time. 
Using the Skyfield API it generates a projection of star postions relative to this vantage point in XY coordinates, where the origin would be directly above the location.
A circular limit is imposed as the horizon, and the apparent magnitude of stars is also used to limit the data.
From this a scatter graph is created with circular marker size based on star magnitude. This forms a star map.
Star names/Constellation names/Constellation star data are imported so that labels and constellation lines can be added to the final plot.
Planets can also be added to the plot.

To create the poster:
The plot is manipulated to remove standard graph features (such as axes);
the background is changed;
a dial overlay is added;
additional text can be added;
the final image is then output as a PNG.

Independantly customisable features for the poster are:
Star data (location/time);
star data to show (just stars/stars and cons. lines/ stars lines and labels);
the outer background colour;
the inner background colour;
the dial colour;
the additional text colour;
plot feature colour (stars/lines/labels);
additional text content;
additional text location;
whether to include planets;
whether to include planet labels or key.

There is an example PNG available.
