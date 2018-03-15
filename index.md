---
layout: post
title: HEC-RAS and Open Source Software
---
##HEC-RAS and Open Source Software##


What does open source geospatial have to do with the US Army Corps of Engineer’s latest hydraulic modeling software HEC-RAS 5 (with 2D goodness!)?  Well it turns out that the popular open source geospatial library known as GDAL is a critical part of the expanding functionality in [HEC-RAS 5](http://www.hec.usace.army.mil/software/hec-ras/ "HEC RAS 5").  Every install of HEC-RAS 5.0 comes packaged with a version of GDAL inside.  As an engineer who solves spatial problems, it’s exciting to see the US Army Corps marry the standard tool for open channel hydraulics with one of my favorite swiss army geospatial libraries. 

<img src="https://farm5.staticflickr.com/4772/39838354915_b0846fe831_o.png" width="1489" height="745" alt="RAS">

If you don't know what GDAL is (pronounced "G-DAHL")… You are in good company, as few civil engineers have heard of this library. 

[GDAL](http://www.gdal.org/ "GDAL") is an open source geospatial project that read/writes a [ton](http://www.gdal.org/formats_list.html "ton") of different geospatial formats and provides additional processing tools for all of these formats in a nicely written library package.  Technically it's GDAL/OGR with GDAL dealing with raster data (imagery, DEMs, etc) and OGR solving problems on the vector side (points, lines polygons). It’s widely used (it’s even found in ESRI’s ArcGIS software), but not as well known among most daily users of GIS software.  

GDAL has a host of handy [utilities](http://www.gdal.org/gdal_utilities.html "utilities") for working with geospatial data including conversion of raster data to vector data, vector data to raster data, a raster calculator, contour generation, merging of multiple rasters and much more.  It makes the process of converting data between different projections a breeze, and is an essential piece of software for anyone who wants to work with geospatial data using open source software.

So why should a civil engineer care that the US Army Corps is using GDAL as a foundational library for its latest version of HEC-RAS? HEC-RAS solves fundamentally spatial problems, but until version 5 of HEC-RAS, it relied on outside software to define the geospatial inputs (GeoRAS and its ilk). With GDAL under the hood, HEC-RAS can now provide all of the geospatial goodness that your HEC-RAS was missing. The capabilities to add shapefiles, aerial imagery and even online aerial imagery in RAS Mapper are built on top of the GDAL library. With the next version of HEC-RAS [promising](http://hecrasmodel.blogspot.sg/2017/06/new-geospatial-editing-tools-coming-in.html "promising") full capabilities to create and edit all of your cross section data within HEC-RAS, those days of depending on GeoRAS (and consequently needing lots of $$ for expensive proprietary 3D analysis software to get work done) should be going the way of the... 

<img src="https://farm5.staticflickr.com/4796/40023209044_b65697c94b_o.png" width="600" height="669" alt="dodo-bird-Alice-in-Wonderland-1">

Investing in open standards and open source software needs to be highlighted in the civil engineering community. It provides value to all of us in two forms... lower operational costs for those using the software, which gets passed on to our local, state and federal governments in the form of lower fees and project costs, and open source software gives the community more control over how to use and shape the pieces of software they depends on to get things done.   

And for those of you worried about what those guys in Redmond are going to do with fewer 3D Analyst licenses from civil engineers... don't worry, I hear they are doing [okay](http://businessworld.in/article/-Esri-s-Annual-Revenues-Exceed-1-1-Billion-/24-04-2017-116907/ "okay")... 

<img src="https://farm5.staticflickr.com/4784/38922891410_04ac03e813_o.jpg" width="500" height="281" alt="scrooge-500x281">