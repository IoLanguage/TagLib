# TagLib 
Used to set meta data tags on the following audio formats:

```
ape
flac
mp3
mpc
mpeg
ogg
```

Supports reading and writing the following attributes:

```
title
artist
album
year
track
genre 
```

And reading the attributes:
```
bitRate
sampleRate
channels
length
```

Example use (load and modify a track genre):

```Io
t := TagLib clone setPath("foo.mp3") load
writeln("genre = ", t genre)
t setGenre("ambient")
t save
```

# Installation
`taglib` should be installed and foundable in your system. Then:
```
eerie install https://github.com/IoLanguage/TagLib.git
```
