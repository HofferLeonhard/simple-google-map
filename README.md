# simple-google-map
Simple Project for using the Google Map API with a free key

## How to use
All the essentials here are done in javascript, through the block script.
First, decal an array of coordinate points to display on the map. For example :

	var cords = [
		{title: "Douala", icon: "marker.png", sizes: {width: 100, height: 120}, lat: 9.737100489464419, length: 4.05229331768824},
		{title: "Yaounde", icon: "marker.png", sizes: {width: 100, height: 120}, lat: 4.737100489464419, length: 4.05229331768824},
		{title: "Nkongsamba", icon: "marker.png", sizes: {width: 100, height: 120}, lat: 14.737100489464419, length: 4.05229331768824},
		{title: "Edea", icon: "marker.png", sizes: {width: 100, height: 120}, lat: 4.0511, length: 9.7679}
	];

This Javascript table contains objects that represent the different points to display on the map, with properties to exploit, such as the title, the icon to display on the map, the latitude, ...

#### NB: 
This structure is mainly used for the test, this will depend on the use that will be made later, for example, to recover the latitude and longitude from the address, we will need more to specify, to share the title that will be important.

#### Presentation

We have two essential functions: mapCords () and mapCordsAddress ()

###### mapCords (id, cords)
It is a recursive function used to display a set of points given on the map

It takes an identifier from which we will begin the chart and the table to browse.

###### mapCordsAddress (id, cords)
It is a recursive function used to retrieve information from a set of points from google map, such as latitude and longitude.

It takes an identifier from which we will begin the chart and the table to browse.

To exploit its results, use its internal object map_coords, which contains the coordinates of a desired address

### How to test
Just open the index.html file in your browser and see the results

Enjoy it !