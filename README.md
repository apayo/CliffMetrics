# CliffMetrics
Version 1.0 
Date 26 March 2024

<p align="left">
  <img src="https://gmd.copernicus.org/articles/11/4317/2018/gmd-11-4317-2018-avatar-web.png" alt="CliffMetrics summary figure" width="250">
</p>

## Table of contents

- [About](#about)
- [Quick Start](#quick-start)
- [References](#references)
- [Contacts](#contacts)

## About
CliffMetrics (Automatic Cliff Metrics delineation) delineates the location of the coastline, coastline normals, and cliff top and toe location along these normals.


## Quick Start

CliffMetrics builds easily using Linux. If you wish to run CliffMetrics on Windows, then we currently recommend using the Windows Subsystem Linux (WSL) software to do this.

Create a local copy of the github repository, for example by downloading a zipfile, then unpacking it or cloning. We suggest unpacking it to something like "/home/YOUR NAME/Projects/CiffMetrics/", this is your CliffMetrics folder.

```
git clone https://github.com/apayo/CliffMetrics
```

In a terminal window (i.e. at a command-line prompt) move to the CliffMetrics folder. Check that you can see a folder structure like this:

in
out
src
cliffmetrics.ini 

Then move to the the src folder Then run run_cmake.sh. 
```
cd CliffMetrics/src
./run_cmake.sh
```
If you get the Permission denied message `-bash: ./run_cmake.sh: Permission denied` you will have to grant permission using `chmod 777 run_cmake.sh` and then `./run_cmake.sh`

If you see error messages re. missing software (for example, telling you that CMake cannot be found or is too old, or GDAL cannot be found or is too old) then you need to install or update the software that is causing the problem.

Run make install `make install`. This will create an executable file called cliff in the CliffMetrics folder.

Edit cliffmetrics.ini to tell CliffMetrics which input file to read (for example, in/simple_fast/simple_fast.dat)

Run cliff `./cliff`. Output will appear in the out/ folder.

Enjoy!

## References
  See <a href="https://doi.org/10.5281/zenodo.1412486"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.1412486.svg" alt="DOI"></a> for the first release of the source code.
  
  See <a href="https://github.com/apayo/CliffMetrics" target="_blank">https://github.com/apayo/CliffMetrics</a> for the latest version of the source code.

  See https://saga-gis.sourceforge.io/saga_tool_doc/8.1.0/ta_cliffmetrics_0.html for the integration in SAGA GIS.

  See https://earthwise.bgs.ac.uk/index.php/Category:CliffMetrics for dedicated Wiki site.

  Payo, A., Jigena Antelo, B., Hurst, M., Palaseanu-Lovejoy, M., Williams, C., Jenkins, G., Lee, K., Favis-Mortlock, D., Barkwith, A., and Ellis, M. A.: Development of an automatic delineation of cliff top and toe on very irregular planform coastlines (CliffMetrics v1.0), Geosci. Model Dev., 11, 4317–4337, https://doi.org/10.5194/gmd-11-4317-2018, 2018.
	


## Contacts
- Andres Payo (agarcia) - <https://www.bgs.ac.uk/people/payo-garcia-andres/>
- BGS Enquiries (enquiries) - <https://www.bgs.ac.uk/about-bgs/contact-us/>
 


