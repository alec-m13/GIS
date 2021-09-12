This repository is for practice learning how GIS systems work.

My plan is to follow the CDC tutorial [here](https://www.cdc.gov/dhdsp/maps/gisx/training/index.html) but using [QGIS](https://www.qgis.org/en/site/) instead of ArcGIS. Hopefully it turns out ok, here we go.

It looks like the CDC tutorial is very specifically designed for ArcGIS, so it won't be the easiest starting point for learning GIS through QGIS. Alternatively the makers of QGIS have put together a [user manual](https://docs.qgis.org/3.10/en/docs/user_manual/index.html) with tutorials specifically made for QGIS, so I plan to use that primarily. But it is not my goal to do the QGIS tutorial or even to learn QGIS for its own sake (no offense to the makers of QGIS) -- my goal is to follow the CDC tutorial using QGIS. It looks like I will learn new material from the QGIS manual and then exercise my skills by adapting the CDC tutorial as best I can.

I will not be including the actual GIS data in this repository, both because that would be an unnecessary use of GitHub's storage and beacuse these data can be licensed in ways which I don't want to deal with. Instead in each folder which contains GIS data which I use, I will add a text file with a link to the source of the data while suppressing the data from inclusion in git.

I will use this repository's wiki as a progress blog for the various tutorials and this readme for overarching structural decisions throughout the learning process.

Initially I had one project file `project_headquarters.qgz` which I intended to use for every module. After a little practice it looks like QGIS isn't really designed for such centrality, it seems better to have a different project file for each module. So I am adding a `Layer_Defs` folder to each submodule. Any map files made to be consumed by QGIS (whole project and any individual layers or other components) will go in these folders and any pdf/svg/etc made to be consumed by human eyes will go in the `rendered` folder.
