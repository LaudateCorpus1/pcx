# pcx
Read pcx bitmap image files in R.

## About

The PCX (Picture Exchange) format is an old bitmap image format that is compressed using runlength encoding and typically indexed, i.e. used with a fixed palette. It was used together with the WAL format for parts of the assets (skybox textures, model skins) in the early Quake series games (id tech1 and tech2 engines).

## Package API

Not ready yet, this is WIP. Here is the current idea:

    # read an indexed PCX image with a 256 colors palette from file at filepath:
    pcx = read.pcx(filepath);

    # show the image
    image(pcx$colors);

    # show the palette:
    # plot(1:256, col=rgb(pcx$palette, maxColorValue = 255))


## References

* The [PCX spec](http://bespin.org/~qz/pc-gpe/pcx.txt)
* A general [PCX format description at Wikipedia](https://en.wikipedia.org/wiki/PCX)
* More details and assembly reading code at the [Shikadi Modding Wiki](http://www.shikadi.net/moddingwiki/PCX_Format). Also checkout the references section.
