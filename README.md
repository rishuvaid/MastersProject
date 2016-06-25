## Maritime Trajectory Visualization ##

Vessel trajectories in coastal waters, while still constrained by shipping lanes, can be more diverse than those where traffic moves along defined paths like roads, paths, or tracks. Thus, displaying these trajectories as line segments can lead to visual clutter where it becomes difficult to estimate density or locate patterns. Previous work has shown density to be a meaningful way to visualize vessel traffic, and we investigate the utility of hexagonal binning in order to locate patterns. Instead of binning all self-reported locations, we group all points by voyage and characterize density by the number of voyages passing through a region. While the bins help characterize the use of a particular area, they do not provide any detail about direction. We propose an interactive method where hovering over one of six triangles of a hexagon displays the trajectories in that direction that pass through the regions.

#### Data ####

Data is available from [http://marinecadastre.gov/ais/](MarineCadastre.gov).

#### Techniques ####

We use hexagonal binning (hexbins) to visualize the density of voyages across a region as on overview. In addition, we display individual voyages when the mouse enters a specific hexagon.

#### Example ###

An example of the Boston Harbor will be available.
