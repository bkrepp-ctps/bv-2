# bv-2
Repository for major version 2 of the balanced volumes visualization app, supporting multiple routes, and routes with both NB/SB and EB/WB orientation.

It is dervived from the work in the (original Balanced Volumes project repository)[https://github.com/bkrepp-ctps/balancedVolumes ]. 

The original repository was devoted __exclusively__ to the visualizations of balanced traffic volume data for I-93 and Massachusetts SR-3
within the boundary of the Boston Region Metropolitan Planning Organization. The code and data in the original repository were developed
as part of UPWP Project #13291 of the Boston Region Metropolitan Planning Organization for Federal Fiscal Year 2019.

As noted above, this version of the repository is devoted to extending the work done in the original repository to encompass additonal routes,
and to being able to support the generation of visualiations for routes with both NB/SB and EB/WB orientations.

The balanced volume data, and the data used to generate a schematic visualizationof this data, is found in the subdiretory __data/csv__.
 
The balanced volume data for 2018 was produced by Bill Kuttner; the balanced volume data for 2010 and 1999 was produced by Tom Lisco.
The GeoJSON data for the geometry of I-93 and SR-3 within the study area is found in the subdirectory __data/geojson__.

This application relies upon the following libraries:
1. jQuery version 2.2.4 (see https://jquery.com/)
2. d3.js version 4.5.0 (see https://d3js.org/)
3. lodash.js version 3.10.1 (see https://lodash.com/)
4. turf.js version 5.2.0 (see https://turfjs.org/)
5. es6string.js (see https://github.com/jabez128/es6string)
6. syncscroll.js version 0.0.3 (see https://github.com/asvd/syncscroll)
7. jquery.scrollTo.js version 2.1.2 (see http://flesler.blogspot.com/2007/10/jqueryscrollto.html)
8. Google Maps JavaScript API version 3.x (see https://developers.google.com/maps/documentation/javascript/tutorial)
9. ctpsGoogleMapsUtils.js version 2.0 (see https://github.com/bkrepp-ctps/ctpsGoogleMapsUtils)

The current version of the app depends upon version __3__ of the __lodash.js__ library.
Among other functions, the application uses underscore's __\_.pluck()__ function, 
which was removed in version __4__ of the library. 
Migrating the application to version __4__ of lodash - the latest - will entail 
replacing calls to __\_.pluck()__ with calls to __\_.map()__. 
This migration is currently TBD.


