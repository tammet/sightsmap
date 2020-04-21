# sightsmap

A selection of sightsmap data is under the data folder:
* topspots_15K.js contains ca 15.000 top spots in the decreasing order of popularity. Some info fields are understandable, some are not explained.
* topspots_15K_extended.js contains ca 15.000 top spots in the decreasing order of popularity, corresponding exactly to the top spots in the previous file.

Fields in each sublist of topspots_15K_extended.js: 

* country code
* type from wiki abstracts
* comma-separated list of tag candidate words
* geonames ID
* geonames type
* geonames type name

Example:

["IT", "capital", "square,tues,basilica,fountain,saint,mary,villa,peter,church,bridge,people,paul,john,san,way,building,port,hole,view,angel,plaza,museum,mountains,pedro,night,arc,hotel,spa,avenue,steps,monument,republic,national,santa,temple,island,course,station,park,novel,interior,old,stage,city", 3169069, "A.ADM2", "second-order administrative division"],

Fields in topspots_15K.js:

* title
* heatmap image file name in sightsmap, append to http://sightsmap.com/wpng/ like http://sightsmap.com/wpng/w2_1.png
* latitude
* longitude
* wiki name (1) or not (0)
* wikitravel (wikivoyage) page exists (1) or not (0)
* if not 0, then google places id (only if neither wikipedia nor foursquare data found)
* 0 or foursquare id (only present if foursquare found and either no wiki found or foursquare name matches wiki)
* foursquare top obj pop (usercount*coeff)
* foursquare usercount
* foursquare type
* foursquare category shorthand
* nr of foursquare places nearby (few km radius, lat+-0.02,lng+-0.04)
* calculated popularity
* population from geonames or 0 or missing if not found 

Example:

["Rome", "w2_1.png", 41.9, 12.48, 1, 1, 0, 0, 160240.0, 16024, "Historic Site", "s", 1054, 2643736]


