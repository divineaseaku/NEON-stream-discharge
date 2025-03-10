NEON Stage-Discharge Rating Curve & Continuous Discharge Shiny App
================

<!-- README.md is generated from README.Rmd. Please edit that file -->

<!-- ****** Description ****** -->

This interactive shiny app plots NEON stage-discharge rating curve and
continuous discharge data using language R. In the left panel, users can
input a domain ID, site ID and date range for which they want data
plotted. Users can include quality flags in the continuous discharge
plot before or after clicking submit. Graphs are render in the right
panel after user click the submit button. The first tab from the left
displays a continuous discharge plot for the selected time range, and
the second tab plots the rating curves used in predicting continuous
discharge.

Note: All data plotted on this app is sourced from the [NEON Data
Portal](https://data.neonscience.org/home) using the
[neonUtilities](https://github.com/NEONScience/NEON-utilities) R
package.

<!-- ****** Usage ****** -->

## User Inputs

**NEON Domain & Site Selection**

User makes a selection from 19 domains, then chooses a site id from the
sites available in the domain.

**Date Range**

Ability to specify date ranges for which data is to be visualized.

**Quality Flag Viewer**

Functionality for toggling between Final Review quality flags, Science
Review quality flags before or after clicking the submit button. When
activated, the quality flags will be rendered as a shaded backround on
the continuous discharge plot spanning the flagged time range.

“Include Final Quality Flag” = Discharge final quality flag indicating
whether a data product has passed or failed an overall assessment of its
quality; detailed in ATBD.

“Include Science Review Quality Flag” = Discharge final quality flag
indicating whether a data product has failed a science review of its
quality detailed in NEON.DOC.001113.

## App Outpus

**Site Description**

Contains a hyperlink of user selected site description hosted on [The
NEON
Website](https://www.neonscience.org/field-sites/explore-field-sites)

**Metadata Table**

The metaData table Contains some key variables associated with the
selected Site ID.

  - Upstream watershed area (km^2): The area (km2) of land that drains
    water into the aquatic site.

  - Reach slope (m): The gradient (m) of the stream bed from the
    upstream to downstream reach boundary of the aquatic site. Slope is
    measured using a total station during topographic site surveys.

  - Mean bankfull width (m): The mean bankfull width (m) of the channel
    measured with total station instruments at transects located
    throughout the monitoring reach. At bankfull stage water is just
    beginning to spill out of the channel and into the floodplain.
    Bankfull flows typically occur at 1.5-year recurrence intervals.

  - D50 particle size(mm): The diameter (mm) of bed substrate
    corresponding to 50% finer in the particle-size distribution.
    Substrate is measured throughout the monitoring reach using
    200-point pebble count methods.

**Continuous Discharge Plot**

The continuous Discharge graph represents the predicted continuous
discharge from sensor-based surface water pressure and stage-discharge.

The plot includes:

  - Continuous discharge (black line)

  - Discharge uncertainty (red and pink ribbons)

  - Empirical discharge (purple points)

  - Continuous stage (blue line)

  - Stage uncertainty (light blue ribbon)

  - Empirical stage (orange points)

User can perform the following on this graph:

  - Zoom in an out of graphs by right-click the section they what to
    view and dragging the mouse to a any stop

  - Toggle legend attributes on the graph ON and OFF by clicking their
    on their representation in the legend

  - Change discharge scales between linear and log by clicking either
    buttons

  - Switch tabs to view the rating curve plot

**Stage-Discharge Rating Curve(s) Plot**

The rating curve graph plots the relationship between stage and
discharge.

The plot includes:

  - Posterior rating curve (black line)

  - Empirical stage-discharge pairs (black points)

  - Rating curve uncertainty (red and pink ribbons)

User can perform the following on this graph:

  - Zoom in an out of graphs by right-click the section they what to
    view and dragging the mouse to a any stop

  - Toggle legend attributes on the graph ON and OFF by clicking their
    on their representation in the legend

  - Change discharge scales between linear and log by clicking either
    buttons

  - Switch tabs to view the continuous discharge plot

<!-- ****** Acknowledgements ****** -->

## Credits & Acknowledgements

Authors:

Divine Aseaku - email: <divineaseaku@gmail.com>

Zachary L. Nickerson - email: <nickerson@battelleecology.org>

<!-- HTML tags to produce image, resize, add hyperlink. -->

<!-- ONLY WORKS WITH HTML or GITHUB documents -->

<a href="http://www.neonscience.org/">
<img src="logo.png" width="300px" /> </a>

<!-- Acknowledgements text -->

The National Ecological Observatory Network is a project solely funded
by the National Science Foundation and managed under cooperative
agreement by Battelle. Any opinions, findings, and conclusions or
recommendations expressed in this material are those of the author(s)
and do not necessarily reflect the views of the National Science
Foundation.

<!-- ****** License ****** -->

## License

GNU AFFERO GENERAL PUBLIC LICENSE Version 3, 19 November 2007

<!-- ****** Disclaimer ****** -->

## Disclaimer

*Information and documents contained within this package are available
as-is. Codes or documents, or their use, may not be supported or
maintained under any program or service and may not be compatible with
data currently available from the NEON Data Portal.*
