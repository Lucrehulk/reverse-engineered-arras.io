# reverse-engineered-arras.io
The most in depth and advanced arras.io reverse engineering work that is valid post-2022 (after WASM additions to arras.io), including full packet hooking, decoding, multiple parsers for sending and recieving packets, & more.

I am now publicly releasing this specialized client of mine from which I did my reverse engineering work on arras given the poor state this game has found itself in.
I never fully completed everything and this client is missing some stuff, but it has almost everything of importance. It is a great base to work with, and really does have a ton of useful stuff. Seeing as I have virtually quit this game, I didn't want this code to go to waste.

I spent some time writing up a "reverse_engineering" folder, which contains a ton of explanations and data on the special code I've created for this game. My hope is that, by releasing this and providing info, skilled coders who want to work on Arras still can use this as a resource.

Important note: I am not actively updating this anymore. But, PULL REQUESTS ARE WELCOME AND ENCOURAGED. There are some things missing, and some potential things that can be improved. Most notably, the current entity deletion detection in the "u" packet is based on a heuristic as the complete entity deletion system is unsolved. I will accept and allow any improvements to be merged--I am just not actively working on this myself. 

Some notable things that could be improved on or added (again, any improvements to these will be accepted with pull requests):

```
Previously mentioned, improving the "u" packet entity death detection heuristic or solving the "canon" way to detect entity death.

"C"ontrol packet direction of movement flags for QOL instead of key pressing (only handled facing).

"F" packet (death packet) parser.

Mockup parser additions and improvements.

More rigorous handling of all packets/parsers (especially Room and potentially the MapManager that utilizes Room) to ensure error mitigation.

And there's loads more that can be done, these are just a few examples that I would say are the more interesting and if anyone wants to tackle their own work stemming from this, I'd start with these.
```

Old readme stuff below.

A custom arras.io client of mine with a ton of neat features--included fully decoded packets and parsing for them.

Client contains functionality for -
```
Parsing critical incoming packets (full access to things like room, entities, broadcast, mockup data, & more).
Logging and modifying incoming and outgoing packets.
Writing/constructing custom outgoing packets.
& more.
```
