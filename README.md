# blender-world-night-sky

World configuration for Blender 3D, featuring:

* Map of the actual stars of our sky, based on NASA imagery.
* Optionally, constellation lines

HDRI files is not included, c.f. [these instructions](https://github.com/alcove-design/viewing-the-world/blob/master/hdri.md#night-sky-star-map-using-nasa-data) to get them.

## Usage

Use at your own risks, consider this a beta version.

Process is currently the following, I am looking forward to simplify it.

1. Get the HDRI file(s) as described in the link above.
2. Append the `World` object from this repository's blend to your blend file.
3. In the World settings tab. delete the default world, and use the newly appended world
4. Edit the image texture nodes in order to link to your HDRI files locations
5. Adapt strength, constellations factor and rotation parameters as suitable.

If using the blend file directly, before rendering, you might want to adjust the number of threads under `Performance\Threads` cycles menu, as it is currently hard-coded to 6.

## Demo

World strength 1:

![demo 1](img/world-strength-1.png?raw=true)

World strength .2:

![demo 2](img/world-strength-0-2.png?raw=true)


Constellations display (wide angle shot):

![demo 3](img/with-constellations.png?raw=true)


N.B.: All demo images above contain a sun light in addition to the sky HDRI. The sky itself is much darker.

## Approach

### Pros

* Display of a realistic universe
* Strength parameter to limit the number of visible stars
* Configurable rotation.

### Cons

* HDRI files are heavy: 28MB for the 4K version, 418 MB for the 16k version. A more suitable approach might be to programatically encode each star's display (location, luminosity, color) - provided input data exists. Thoughts?

## Contributing

Fixes and suggestions welcome.


## License

Public domain, c.f. License .md

Please credit the imagery creators when using the HDRIs:

> NASA/Goddard Space Flight Center Scientific Visualization Studio. Constellation figures based on those developed for the IAU by Alan MacRobert of Sky and Telescope magazine (Roger Sinnott and Rick Fienberg). 
