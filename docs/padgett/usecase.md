# Integration of QGIS and Python Scripts to Model and Visualize Storm Impacts on Distributed Infrastructure Systems

> **Catalina González-Dueñas and Jamie E. Padgett - Rice University**

> **Miku Fukatsu - Tokyo University of Science**

This use case study shows how to automate the extraction of storm intensity parameters at the structure level to support regional risk assessment studies. This example leverages QGIS and python scripts to obtain the surge elevation and significant wave height from multiple storms at specific building locations. The case study also shows how to visualize the outputs in QGIS and export them as a web map. The followig DesignSafe resources are leveraged in this example: 

[Geospatial data analysis and Visualization on DS - QGIS](https://www.designsafe-ci.org/rw/workspace/#!/qgis-duvd-3.16.3u2)

## Background 

### Citation and Licensing

* Please cite [González-Dueñas and Padgett (2022)](https://doi.org/10.17603/ds2-3zdj-493) to acknowledge the use of any resources from this use case.

* Please cite [Rathje et al. (2017)](https://doi.org/10.1061/(ASCE)NH.1527-6996.0000246) to acknowledge the use of DesignSafe resources.  

* This software is distributed under the GNU General Public License (https://www.gnu.org/licenses/gpl-3.0.html).  

### Description 

This case study aims to support pre-data processing workflows for machine learning applications and regional risk analysis. When developing predictive or surrogate models for the response of distributed infrastructure and structural systems, intensity parameters need to be associated with each component of the system (e.g., buildings, bridges, roads) under varying hazard intensity or different hazard scenarios. To accomplish this and given the different resolutions of the hazard and infrastructure data, geographical tools need to be used to associate the intensity parameters with the distributed infrastructure or portfolio components. In this case study, python codes were developed to automate geospatial analysis and visualization tasks using QGIS, an open-source GIS software. As a proof of concept, 15 storms with varying forward velocity and sea-level rise, are used to extract the surge and significant wave height at specific house locations using the building stock of Galveston Island, TX. The workflow of analysis is as follows:


![caption](img/Fig1_Updated.jpg)

This case study is divided into three basic components:

1. Opening a session in QGIS via DesignSafe
2. Setting the python environment
3. Visualization of the outputs

## Opening a QGIS session in DesignSafe

To access QGIS via DesignSafe go to [Workspace -> Tools & Applications -> Visualization -> QGIS Desktop 3.16](https://www.designsafe-ci.org/rw/workspace/#!/qgis-duvd-3.16.3u2). You will be prompted the following window:

![Fig2](img/Fig2_Updated.jpg)

Change the desktop resolution according to your screen and provide a name for your job. Hit *Launch* when you finish, after a couple of minutes your interactive session will start:

### Header2 Subheading

In aliquam sem fringilla ut morbi. Interdum varius sit amet mattis vulputate enim nulla aliquet. Sit amet mattis vulputate enim nulla.  In egestas erat imperdiet sed euismod nisi porta lorem. Eget nulla facilisi etiam dignissim diam.  Facilisi cras fermentum odio eu feugiat. Velit aliquet sagittis id consectetur. Vel quam elementum pulvinar etiam.  Ut diam quam nulla porttitor massa id neque aliquam. Sodales ut etiam sit amet nisl.  Scelerisque varius morbi enim nunc faucibus a. Sit amet volutpat consequat mauris nunc. Et leo duis ut diam.

*Add images to the folder img and use relative path to specify the location of the image.*   

![caption](img/mkdocs-template.png)
> Use case template design


## Header3

Morbi tristique senectus et netus et. Tristique senectus et netus et malesuada fames.  Eu mi bibendum neque egestas congue quisque. Id consectetur purus ut faucibus pulvinar elementum integer enim. Nunc consequat interdum varius sit amet mattis vulputate enim nulla.  Porta nibh venenatis cras sed felis eget. Dui id ornare arcu odio ut sem nulla pharetra diam. Pellentesque habitant morbi tristique senectus et netus et. Commodo nulla facilisi nullam vehicula ipsum a arcu. Nisi porta lorem mollis aliquam ut porttitor leo.

Numbered list 

1. [numbered linked item](https://maps.google.com)
2. second item
3. third item

### Header3 subheading

Ac feugiat sed lectus vestibulum mattis ullamcorper. Et egestas quis ipsum suspendisse ultrices gravida dictum fusce ut. Scelerisque eu ultrices vitae auctor eu augue ut lectus arcu.  Imperdiet proin fermentum leo vel orci porta non pulvinar. Dictumst quisque sagittis purus sit amet. Aliquam purus sit amet luctus. Aliquet bibendum enim facilisis gravida neque convallis a cras. Orci porta non pulvinar neque laoreet suspendisse. Urna neque viverra justo nec ultrices dui.

**Example Table**

| Column 1 | Column 2 | Column 3 |
|----------|----------|----------|
| Stampede2| CPU      | 2017     |     
| Frontera | CPU & GPU| 2019     |     

Or use markdown table generator: [https://www.tablesgenerator.com/markdown_tables](https://www.tablesgenerator.com/markdown_tables)


### Math

To generate math equations in markdown.

For inline mode formulas: $`a^2+b^2=c^2`$.

For display mode formulas which appear on a separate line
```math
f(x) = \int_{-\infty}^\infty
\hat f(\xi)\,e^{2 \pi i \xi x}
\,d\xi
```

### Code

``` python
import tensorflow as tf
```

Highlight specific lines of the code

``` python hl_lines="3 4"
""" Bubble sort """
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```
