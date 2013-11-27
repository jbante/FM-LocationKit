# Location Kit

Location Kit is a collection of functionality for working with location information in FileMaker and FileMaker Go applications.

There are scripts and custom functions in this module, but you do not have to use both. The scripts do not reference any custom functions. Every custom function has an equivalent script, but not every script has an equivalent custom function.

## Installation

1. If you do not already have the [JSON module](http://www.modularfilemaker.org/2013/08/json/) installed in your FileMaker file, import the "Modules" > "JSON" script folder from the module demo file into your file's "Modules" folder.
2. Import the "Modules" > "Location Kit" script folder from the module demo file into your file's "Modules" folder.
3. (optional) Import all the custom functions from the module demo file into your file.

## Scripts

### Calculate Direction Between Locations

The "Calculate Direction Between Locations" script calculates the direction (azimuth and cardinal direction) at the start of a straight line (great circle) path between two points on the surface of the Earth. The LocationAzimuth and LocationCardinalDirection custom functions can be used for the same result.

### Calculate Distance Between Locations

The "Calculate Distance Between Locations" script calculates the distance along a straight line (great circle) path between two points on the surface of the Earth. The LocationDistance custom function can be used for the same result.

### Get Current Location

The "Get Current Location" script parses the result of the LocationValues function into separate variables, and checks whether the result is cached from a previous location fix.

### Start Navigation in Navigon

The "Start Navigation in Navigon" script launches the Navigon app on iOS to start navigation to a location. The location can be specified by address or coordinates (latitude and longitude).

## Custom Functions

### LocationAzimuth ( latitude1 ; longitude1 ; latitude2 ; longitude2 )

The LocationAzimuth custom function calculates the initial azimuth (bearing) along a straight line (great circle) path between two locations on the surface of the Earth. The "Calculate Direction Between Locations" script can be used for the same result.

### LocationCardinalDirection ( azimuth ; precision )

The LocationCardinalDirection custom function converts an azimuth into a cardinal direction. Developers can specify 1, 2, or 3 letters of precision in the cardinal direction. The "Calculate Direction Between Locations" script can be used for the same result.

### LocationDistance ( latitude1 ; longitude1 ; latitude2 ; longitude2 )

The LocationDistance custom function calculates the distance along a straight line (great circle) path between two points on the surface of the Earth. The "Calculate Distance Between Locations" script can be used for the same result.

## License

Anyone may do anything with this software. There is no warranty.