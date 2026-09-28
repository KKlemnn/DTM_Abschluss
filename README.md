## EP 01 | Dasymetric Maps
### Definition, advantages and disadvantages
Dasymetric maps are an alternative to regular choropleth maps that aim to represent the spatial distribution of a phenomenon more realistically. While a regular choropleth map assigns a value to an entire area, regardless of the presence of the phenomenon in all parts of said area, a dasymetric map uses additional information, to show where the phenomenon is actually concentrated.
The main advantage of dasymetric maps is therefore that they can provide a more accurate and detailed representation of spatial patterns and reduce the misleading impression that a phenomenon is evenly spread across an area. They are particularly useful when large areas contain significant amounts of land that are empty of any phenomena. For example, a dasymetric population by area map would leave out uninhabited space to better represent population distribution. Through this, dasymetric maps try to lessen the area size bias, cognitive illusion in cartography where people perceive larger geographic regions on a map as more dominant or important than smaller regions, even when both share the same data value or colour.

However, dasymetric maps also have disadvantages: they require additional data and are therefore more complex to create. While less so than regular choropleth maps, they still rely on assumptions about how the phenomenon is distributed within an areas. Therefore, they can appear more precise than choropleth maps but may not necessarily be more accurate. Additionally, the generally smaller sizes of coloured areas may be harder to read and interpret.

Overall, regular choropleth maps are simpler, easier to produce and interpret, whereas dasymetric maps can provide a more realistic spatial representation but require more data and methodological assumptions.

### Method and Application: Berlin Populatiuon Map
In the example below the polygons of the LOR (Lifeworld-oriented spaces) of Berlin were coloured according to their population. Unmodified, this produced the first map, showing absolute numbers per LOR.
For the next map, these were computed against the areas of the LOR itself and coloured accordingly, thus creating a (regular choropleth) population density map.

The last map then has the LORs cut down to just the areas that are actual residential areas. This resulted in a dasymetric population density map.
 <img width="auto" height="auto" alt="image" src="https://raw.githubusercontent.com/KKlemnn/DTM_Abschluss/refs/heads/main/Klemann_Berlin_Bev%C3%B6lkerung_Versch_Karten-1.png" />

## EP 02 | Grid Choropleth Maps
### Definition, advantages and disadvantages
Grid Choropleth maps are a variation of the regular Choropleth map in which the study area is divided into a regular grid of equal-sized cells, such as squares or hexagons, instead of administrative areas or other statistical units. This makes the map less dependent on administrative boundaries and allows spatial patterns to be represented more consistently across an area. Analogous to a Choropleth map, each cell is assigned a colour according to the value of the variable being mapped. With every grid cell being the same size, comparisons between locations is easier and the visual influence of large administrative areas reduced. Grid maps can therefore reveal local spatial patterns and concentrations that may be hidden in a regular choropleth. They are also useful for analysing phenomena continuously distributed across space and can make comparisons between different regions easier because the same spatial framework is used everywhere.

One disadvantage of Grid Choropleth maps stems from the different data format required for their creation: A more detailed data source and more spatial processing is generally necessary for their creation. The choice of grid size can also influence the patterns that appear: very large cells may hide local variation, while very small cells can produce a noisy or overly detailed map.

Grid Choropleth maps offer a more spatially consistent alternative to regular Choropleths, but their usefulness depends strongly on the quality and resolution of the underlying data and on the chosen grid size.

### Method and Application: Cherry Blossom in Berlin I
For this example, the location of all cherry tries in Berlin was first mapped and the entirety of the Berlin area divided into 500m squares. Next, the amount of cherry trees per square was counted and the squares coloured accordingly.
 <img width="auto" height="auto" alt="image" src="https://raw.githubusercontent.com/KKlemnn/DTM_Abschluss/refs/heads/main/Kirschbl%C3%BCten%20500m.png"/>

## EP 03 | Dot Maps
### Definition, advantages and disadvantages
Dot maps are a type of thematic map that represent the location and distribution of a phenomenon using individual dots, with each dot representing a fixed quantity of the mapped variable. Unlike a regular choropleth map, which assigns a single colour and value to an entire administrative area, a dot map can show the spatial concentration and dispersion of the phenomena within that area.
This is a major advantage because it provides a more intuitive impression of where something is concentrated rather than simply showing an average value for a whole region. Thus, they can also reveal clusters, gaps and density patterns that may be hidden by the boundaries of regular choropleth maps. In addition, because the dots represent quantities, the reader can often get a direct visual impression of the magnitude of the phenomenon.

The major disadvantage of dot maps is that they can become difficult to read when there are very large numbers of dots, creating visual clutter. The size of dots can produce additional confusion: if each dot represents too large a quantity, smaller concentrations may disappear, whereas too small a value can produce an overcrowded map. Furthermore, dots do not necessarily represent the exact location of individual phenomena, but may just be aaproximation. 

In comparison, regular choropleth maps are generally easier to interpret for comparing overall values between clearly defined administrative units, whereas dot maps are better at communicating spatial distribution, concentration and dispersion within those units.

### Method and Application: Cherry Blossom in Berlin II
For this map the above described method was used, but instead of differently coloured shapes representing areas, differently scaled and coloured cherryblossoms represent how many trees are in a given area.

Thus, this is not a Dot Map in the traditional sense, as the dots don't represent individual phenomena, but rather aggregation of these.
 <img width="auto" height="auto" alt="image" src="https://raw.githubusercontent.com/KKlemnn/DTM_Abschluss/refs/heads/main/Kirschbl%C3%BCte.png" />

## EP 04 | Value by Alpha Maps
### Definition, advantages and disadvantages
In Value by Alpha Map is a Choropleth Map in which the representation of a value is done not merely by colour variation, but by also modifying the transparency of that colour along the spectrum. Thus multiple colours can be used for signifying the variation of one value, usually a nominal value, while the transparency of that colour is used to represent a metric value.

It is thus possible to represent two different values on the same map, which is the big advantage of the Value by Alpha Map. Depending on the minimum transparency used, it is also possible to retain significant amounts of information not exclusive to the Choropleth map itself

Especially on higher transparency values Value by Alpha Maps can become difficult to read as it becomes hard to tell colours apart that are barely visible in the first place. Even when these differences are sufficient however, the simple creation of an actual leged becomes difficult, as two different axis need to be represented.

Overall, Value by Alpha Maps offer unique advantages in presenting much more information than regular Choropleth maps, but become rather hard to read because of this.

### Method and Application: 2026 Hungarian Parliamentarian Election
In this example, the election results for the two biggest parties, Fidesz and Tisza were mapped onto the electoral constituencies. The areas were than coloured according to what parties carried more votes, with the intensity of the colour representing a higher share of the votes.

Arranging the map in this way also mitigates one of the large disadvantages of the Value by Alpha Map: Where it becomes hard to tell which party won, the difference in votes was much smaller than in those with clearer colouring.
 <img width="auto" height="auto" alt="image" src="https://raw.githubusercontent.com/KKlemnn/DTM_Abschluss/refs/heads/main/Layout%201.png/>

## EP 05 | Origin Destination Maps
Origin-destination maps are a type of thematic map used to show movement or flows between two or more locations. Therefore, they graphically connect an origin, where a movement begins, to a destination, where it ends. The connection can than further be used to represent both the direction (for example by an arrowhead) or volume or intensity of the connection by variation in thickness and colour of the line.

Its main advantage is that it makes spatial connections, direction and movement patterns visible, allowing the reader to identify major flows, hubs and important connections that a Choropleth cannot show.

However, origin-destination maps can become difficult to read when there are many flows, as overlapping lines and arrows can create significant visual clutter. Small or low-volume flows may also be difficult to see, while very large flows can dominate the map. Another disadvantage is that the map can require more explanation because the reader must understand the meaning of line direction, thickness and possibly colour.

Unlike a regular Choropleth Map, which allows relatively straightforward comparison of values between areas, an origin-destination map is therefore better suited to understanding connections and movement between areas.

### Method and Application: Volunteers for the International Brigades in the Spanish Civil War
This map attempted to visualise the origin of the volunteers for the International Brigades in the Spanish Civil War. First, the volunteers were mapped to points in the capitals of their country of origin. The size of the three-pointed Star in that location is an additional indicator for the amount of volunteers Next lines were drawn to Madrid, with thickness and colour representing the amount of volunteers.

This map should be regarded as a failure, but with valuable lessons learned. First, the amount of volunteers is distributed extremely unevenly: The Most volunteers, almost 9000, came from France. The second place is already only a mere 2000, while the smaller contingents number in the low hundreds. This required a logarithmic scale, which is already counterintuitive. Furthermore, the geographic location of the capitals makes it almost inevitable, that the French connection blocks out all others.
 <img width="auto" height="auto" alt="image" src="https://raw.githubusercontent.com/KKlemnn/DTM_Abschluss/refs/heads/main/IntBrig.png" />

## EP 06 | Tile Maps for Raster Data
Tile Maps can be used to make more fine-grain raster data easier to visualise. In this, they work quite similar to Grid Choropleth Maps and have the same advantage and disadvantages.

Additional, the simplification can be an advantage, by eliminating clutter and making general trends more visible. It can also work to their disadvantage however, by eliminating much of the detail of the initial datset.

### Method and Application: Germany as building bricks
Using a raster data height map as the data source, Germany has been divided into equally sized squared. The data from the height map was then aggregated into these squared, using a mean, and is now represented in different colours, following the conventional display of altitude on maps. Additional detail was then added to make the squares appear as if they were plastic building bricks.
 <img width="auto" height="auto" alt="image" src="https://raw.githubusercontent.com/KKlemnn/DTM_Abschluss/refs/heads/main/deutschland_lego_v2.png" />

## EP 07 | Animated Maps
The most straightforward way of showing a temporal axis on a map is generally to have it be animated. This basically means that multiple versions of the map are strung one after another to visualise changes in phenomena.

The advantage is obvious: Simply displaying the different states in sequence allows for a quick identification of trends.

On the other hand, the fact that the animation will only go one way, makes it almost impossible to compare temporal states directly with one another. 

### Method and Application: Comet Shower
For this animation, the visualised Dataset contained the start and endpoint of visible comets at given points in time. These points were connected and coloured mimicking a shooting star. Then, the shooting stars were aggregated by hour and are displayed in sequence.
 <img width="auto" height="auto" alt="image" src="https://raw.githubusercontent.com/KKlemnn/DTM_Abschluss/refs/heads/main/full.gif" />

## EP 08 | Mesh Data
Mesh data divides an area into a regular grid of small cells, with each cell containing a value for a particular variable. Whereas in the previous examples of Grid and Tile Maps, where non-uniform data was represented on a uniform map, now the challenge is to find ways in which to display this uniform data in non-uniform ways. Additionally, as recognisable geographic features may be absent in the data, an additional challenge is to use ways of making these visible, without interfering with the mesh data.

### Method and Application: Van-Gogh-Style Wind Map
The mesh data displayed here is for wind speed, specifically during the winter storm of 1953, the heaviest to hit the Netherlands in the last century. The lines themselves present wind direction and more lines converging presents particularly intense winds.
Through various blending methods, the streamlines themselves show a (distorted) elevation map of Western-Central Europe, do better localise the map.
 <img width="auto" height="auto" alt="image" src="https://raw.githubusercontent.com/KKlemnn/DTM_Abschluss/refs/heads/main/1953_storm_big.gif" />

## EP 09 | Beyond the Second Dimension
Some data is best visualised in not two, but three dimensions. To achieve this, two different methods can be used in QGIS: 2.5D and (True) 3D.
2.5D merely approximates a three-dimensional view by shofting existing areas up accordning to a set 'height' value and drawing additional areas 'below' them to fake them being solid. While fairly easily visible and renderable on a two dimensional map, this is no true 3D and may not be able to show details on all sides of the object.

3D View on the other hand can display these details, but requires a 3 dimensional space to be properly displayed, where it can be looked at from multiple angles.

### Method and Application: A Village in 2.5 and 3D
These pictures show a small village in 2.5D and 3D (the later only in a screenshot). For the 2.5D view, the objects merely needed a height (in this case already contained in the dataset) to render the 2.5D view: The 'top' of the polygons was then coloured red, while the 'sides' where coloured light gray.
 <img width="auto" height="auto" alt="image" src="https://raw.githubusercontent.com/KKlemnn/DTM_Abschluss/refs/heads/main/Bordenau.png" />

The 3D view however required more complex models, which for example distinguished between roof and wall polygons. These were then coloured as in the 2.5D view.
 <img width="auto" height="auto" alt="image" src="https://raw.githubusercontent.com/KKlemnn/DTM_Abschluss/refs/heads/main/Bordenau3d.png" />
