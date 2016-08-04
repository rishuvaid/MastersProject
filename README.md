## Maritime Trajectory Visualization ##

Vessel trajectories in coastal waters, while still constrained by shipping lanes, can be more diverse than those where traffic moves along defined paths like roads, paths, or tracks. Thus, displaying these trajectories as line segments can lead to visual clutter where it becomes difficult to estimate density or locate patterns. Previous work has shown density to be a meaningful way to visualize vessel traffic, and we investigate the utility of hexagonal binning in order to locate patterns. Instead of binning all self-reported locations, we group all points by voyage and characterize density by the number of voyages passing through a region. While the bins help characterize the use of a particular area, they do not provide any detail about direction. We propose an interactive method where hovering over one of six triangles of a hexagon displays the trajectories in that direction that pass through the regions.

#### Data ####

Data is available from [MarineCadastre.gov](http://marinecadastre.gov/ais/).

#### Techniques ####

We use hexagonal binning (hexbins) to visualize the density of voyages across a region as on overview. In addition, we allow a user to interactively highlight individual voyages by hovering over a specific hexagon. As this does not provide information about direction, we also present a technique to subdivide each hexagon into six triangles, and upon hover over a triangle, highlight voyages that locally have the same direction as the triangle. Since the triangles are equilateral, we add an arrow to make clear the direction being shown.

#### Example ####

An [example](https://rishuvaid.github.io/maritime-vis/ais-tri-map.html) of voyages that pass near Boston in January 2011. When the mouse is dragged over one of the six triangles that the hexagon is divided into, the voyages crossing the corresponding edge into the hexagon are shown. Thus, moving across the edge shows voyages in the opposite direction. This can be compared with an [example](https://rishuvaid.github.io/maritime-vis/ais-hex-map.html) where all voayges passing through a hexagon are highlighted, regardless of direction.

 * [Hexagons](https://rishuvaid.github.io/maritime-vis/ais-hex-map.html)
 * [Directional Triangles](https://rishuvaid.github.io/maritime-vis/ais-tri-map.html)

#### Video ####

A short [video](https://rishuvaid.github.io/maritime-vis/video.mp4) is available.
