# Change a Bit
Small helper funcs for tampering with values' bits and areas of bits.

## Possible usages
Originally I made this for a multiplayer game project. The project (mainly) held the gamestate as uint64_t array
where a single uint64_t element corresponded a single "tile" in the game world. The 64 bits could hold all the
possible different states of the tile including a character/unit, its' action + huge amount of different kinds
stuff.

Some of the tile's bits were used as flags and some as "sub values" with varying bit counts.
This made server side's "game state broadcasting" and many other things quite nice and convinient.

This header has the funcs for dealing with this kind of stuff.
