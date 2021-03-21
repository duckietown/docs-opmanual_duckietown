# Duckietowns and Duckiebots {#dt-ops-city-definitions status=ready}

<div class='requirements' markdown="1">

Requires: Knowledge of the [Duckietown appearance specifications](#dt-ops-appearance-specifications).

Results: Knowledge of the relation between Duckietown and Duckiebots, or, what can Duckiebots do in different Duckietowns.

Next Steps: [Duckietown assembly](#dt-ops-assembly).

</div>

Not all functionalities of the Duckiebots require all Duckietown city elements to work. If you are wondering what learning experiences you can explore with what Duckietown, you are in the right place. We define Duckietown configurations of increasing complexity depending on what Duckiebot functionalities they support.

## Only traffic signs (no city) {#dt-ops-no-city-def status=ready}

Without a Duckietown, it will not be possible for Duckiebots to showcase most of their behaviors. Nonetheless, traffic signs have AprilTags, which allow to play with the AprilTag detection and relative pose estimation pipeline, and in turn with the camera calibration and system identification procedures.

## City loops {#dt-ops-loops-def status=ready}

The fundamental Duckiebot behaviors can be explored with a very simple Duckietown. We call these simple cities: _loops_.

City loops are closed road patterns, without intersections, that meet the appearance specifications. They can be made only of floor layer elements, with no signals.

City loops enable to play with the:

* _perception pipeline_: what happens when data is obtained in form of measurements (i.e., images in the `DB17` and `DB18` configurations), and how it is used to extract information, leading the Duckiebots to generate a belief of their position and orientation in the lanes.

* _lane control_: the process that Duckiebots apply to transform beliefs provided by the perception pipeline in decisions on how to steer in order to stay inside the lane.  

* _traffic management_: the functionality for which Duckiebots stay at a safety distance from other Duckiebots driving in front of them.

When city loops are augmented with traffic signs, e.g., road names, it is then possible to explore the functionality of:

* _AprilTag detection and relative pose estimation_: how Duckiebots detect AprilTags, and determine their position and orientation relative to them. This information can be used to localize in the map.

If you acquired a Duckietown Starter Pack, you have a city loop with traffic signs.

## Navigable cities {#dt-ops-nav-def status=ready}

The more complex Duckiebot behaviors require intersections and other city elements such as traffic lights to work. We define cities that include intersections as _navigable_ cities.

Navigable cities are city loops connected by intersections, meeting the appearance specification. Navigable cities require traffic signs.

Navigable cities enable testing of Duckiebot behaviors. A complete list (for one or more Duckiebots) of behaviors can be found in the [demo section](https://github.com/duckietown/docs-robotarium/blob/master/book/robotarium/00_book_robotarium.md) of the Duckiebot operation manual.

## Robotarium {#dt-ops-robotarium-def status=ready}

Robotariums (Robotic aquariums) are experimental Duckietowns designed for continuous operations. Robotariums require a maintenance area in addition to a Duckietown, providing essential functions like automatic charging. More information on Robotariums can be found in the [Robotarium book](https://github.com/duckietown/docs-robotarium).


TODO: switch last two links with proper inter-book references
