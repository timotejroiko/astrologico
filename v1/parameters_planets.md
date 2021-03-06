## Planets

An array of IDs specifying the objects to calculate. The ID format consists of a type identifier followed by an object number. Currently a maximum of 100 objects can be requested at a time. If omitted, it defaults to the objects `P0 P1 P2 P3 P4 P5 P6 P7 P8 P9 P11`.

| Example | Descripton |
|---|---|
|P0|Planet number 0 (sun)|
|S1351|Star number 1351 (regulus)|
|A3|Asteroid number 3 (juno)|
|PN5|Planet number 5's Ascending Node (jupiter's north node)|

<br>

### Object Types

| Object Type | Descripton |
|---|---|
| P | Planets and special objects |
| A | Asteroids |
| S | Stars |
| H | Hypothetical Planets |
| C | Comets |
| PA | Planet's Aphelion |
| AA | Asteroid's Aphelion |
| PP | Planet's Perihelion |
| AP | Asteroid's Perihelion |
| PN | Planet's Ascending Node |
| AN | Asteroid's Ascending Node |
| PS | Planet's Descending Node |
| AS | Asteroid's Descending Node |
| PF | Planet's Second Focus |
| AF | Asteroid's Second Focus |
| L | Arabic parts/lots |
| LD | Arabic parts/lots day (no reverse) |
| LN | Arabic parts/lots night (force reverse) |
| [QS:](#integration) | Get an object from the simbad database |

<br>

### Object IDs

Asteroid IDs follow the same numbering as their official designation. Other objects are either numbered alphabetically or follow a special order. You can use the [Search](endpoints_search.md) endpoint to lookup objects by name and get their IDs. Here are the IDs for some of the most used objects:

| ID | Object |
|---|---|
| P0 | Sun |
| P1 | Moon |
| P2 | Mercury |
| P3 | Venus |
| P4 | Mars |
| P5 | Jupiter |
| P6 | Saturn |
| P7 | Uranus |
| P8 | Neptune |
| P9 | Pluto |
| A2060 | Chiron |
| P10 | Mean Ascending Node |
| P11 | True Ascending Node |
| P23 | Mean Descending Node |
| P24 | True Descending Node |
| P14 | Earth |
| P12 | Mean Lilith |
| P13 | True Lilith |
| P21 | Natural Lilith |
| C1 | Comet Halley |
| A1 | Ceres |
| A2 | Pallas |
| A3 | Juno |
| A4 | Vesta |
| H1 | Cupido |
| H2 | Hades |
| H3 | Kronos |
| H4 | Apollon |
| H5 | Admetos |
| H6 | Vulkanus |
| H7 | Poseidon |
| L118 | Part of Fortune |
| L119 | Part of Spirit |
| S3071 | Aldebaran |
| S1351 | Regulus |
| S3099 | Sirius |
| S1224 | Vega |
| S2665 | Spica |

<br>

### Simbad Integration

When working with stars and stellar objects, if our database does not contain the object you're looking for, it is possible to retrieve it directly from the simbad database using any simbad-compatible identifier in the following format:

| Example | Descripton |
|---|---|
|QS:HD 25452| Get Object HD 25452 (Star)|
|QS:NGC 3726| Get Object NGC 3726 (Galaxy)|

<br>