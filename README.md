# nztm-geo-conversion-js
JavaScript function to convert NZTM coordinates to universal Latitude Longitude

This function was implemented in July 2019 on request of Holly Horwood to be used in her [NZ Holiday Helper project](https://github.com/Holly-Horwood/holiday_helper/).  See her [published version of this script](https://github.com/Holly-Horwood/holiday_helper/blob/master/assets/js/geo.js) with attribution, or the script in use on her [project's live site](https://holly-horwood.github.io/holiday_helper/).

Problem: The NZ Department of Conservation API uses the NZTM coordinate projection, while the Google Maps API uses Lat/Long.  Land Information New Zealand (LINZ) publishes the [transformation formulae](https://www.linz.govt.nz/data/geodetic-services/coordinate-conversion/projection-conversions/transverse-mercator-transformation-formulae) and [NZTM2000 parameters](https://www.linz.govt.nz/data/geodetic-system/datums-projections-and-heights/projections/new-zealand-transverse-mercator-2000), which together provide the information necessary to perform the conversions programmatically.

This JavaScript version of the algorithm was adapted from [this C# implementation on the GIS Stack Exchange](https://gis.stackexchange.com/questions/225065/converting-nztm-new-zealand-transverse-mercator-to-lat-long/277227#277227).  (Note that [a different JavaScript solution](https://gis.stackexchange.com/questions/225065/converting-nztm-new-zealand-transverse-mercator-to-lat-long/336426#336426 ) was later posted to the same S/E question in September 2019.)
