# Julia Kerpel
<img src="./65496248_c7ktf1fhxa.heic.PNG" style="width:50%; margin:auto; display:block">
## Hello! My name is Julia Kerpel. I am a first year at UC Berkeley, pursuing an engineering degree. I am also part of the fourth cohort of the [SEED Scholars Honors Program](https://seedscholars.berkeley.edu/home).
<hr>

### I am from Highland Park, IL. That is over 2,000 miles from Berkeley!
from datascience import *
import numpy as np
import plotly.express as px
import plotly
print(plotly.offline.plot(fig, include_plotlyjs=False, output_type='div'))
fig.show()
cities = make_array('Highland Park','Berkeley')
lats = make_array(42.1817,37.8715)
lons = make_array(-87.8003,-122.2730)
towns()
towns.with_columns('city',cities,'latitude',lats,'longitude',lons)
px.scatter_geo(towns, 
               lat = 'latitude', 
               lon = 'longitude',
               title = "Where is Julia?"
              )
