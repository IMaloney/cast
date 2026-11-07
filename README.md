# Snowcast

## Building Files

`make server` --> builds the server

`make client` --> builds the client

`make listener` --> builds the listener

`make build` --> builds the snowcast_control, snowcast_server, and snowcast_listener 

`make clean` --> removes old build files

`make test` --> runs current tests

#### To Start a Server with multiple songs per station:
`./snowcast_server -e [port] [song1],[song2],[song3],... [song4] [song5] `

Example:
`./snowcast_server -e 8888 ./mp3/tinyfile,./mp3/mediumfile,./mp3/VanillaIce-IceIceBaby.mp3 ./mp3/tinyfile ./mp3/mediumfile`

### Server Commands
`print/p` --> prints a list of the stations and all the clients listening to each station

`help/h` --> prints the help menu

`addStation/a [song1] [song2]...` --> adds a new station to server with [songs...] as music

`removeStation/r [stationNumber]` --> removes station [stationNumber] from radio

### Client Commands

`getsongs [station]` --> gets all the songs that are playing on the station

`playlist [station] [num songs]` --> gets the next num songs that will be played on the station


