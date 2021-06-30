# Meteolakes Transects

This is an example for how to process transects from the Meteolakes API.

http://meteolakes.ch/api/transect/file/:lake/:variable/:location/:year/:week

| Parameter | Description | Acceptable Inputs |
| --- | --- | --- |
| lake | Name of the lake | geneva, zurich, biel, greifensee |
| variable | Variable to return | temperature, velocity |
| location | Location of transect | xz, yz |
| year | Year of data | |
| week | Week of the year | 1 - 52 |

Transect locations:

| Lake | xz | yz |
| --- | --- | --- |
| geneva | Geneva - Villeneuve | Evian - Lausanne |
| zurich | Zurich - Schmerikon | Oberrieden - Herrliberg |
| biel | Saint Johannsen - Biel | Tauffelen - Twann |
| greifensee | South - North | West - East |

The returned csv object has quite a complex structure. It returns a grid of values; x (CH1903), y (CH1903), depth (m), values (xNo timesteps).