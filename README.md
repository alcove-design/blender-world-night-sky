# blender-world-night-sky

World configuration for Blender 3D, featuring:

* Map of the actual stars of our sky, based on NASA imagery.
* Optionally, constellation lines

HDRI files is not included, c.f. [these instructions](https://github.com/alcove-design/viewing-the-world/blob/master/hdri.md#night-sky-star-map-using-nasa-data) to get them.

### Approach

## Pros

* Display of a realistic universe
* Strength parameter to limit the number of visible stars
* Configurable rotation.

## Cons

* HDRI files are heavy: 28MB for the 4K version, 418 MB for the 16k version. A more suitable approach might be to programatically encode each star's display (location, luminosity, color) - provided input data exists. Thoughts?

### Contributing

Fixes and suggestions welcome.


## License

Public domain, c.f. License .md

Please credit the imagery creators when using the HDRIs:

> NASA/Goddard Space Flight Center Scientific Visualization Studio. Constellation figures based on those developed for the IAU by Alan MacRobert of Sky and Telescope magazine (Roger Sinnott and Rick Fienberg). 
