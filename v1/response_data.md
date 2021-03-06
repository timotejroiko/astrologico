## Data

This object contains all the calculated data. These fields can be enabled by using [Display Options](parameters_display.md).

All fields (except `name`, `formula` and `error`) are arrays when using the [Ephemeris](endpoints_ephemeris.md) endpoint.

| Value | Type | Descripton |
|---|---|---|
| name | String | Object name |
| names | Array | Array of names for objects with multiple names (returned instead of `name` for stars and arabic parts only) |
| designations | Array | Array of official designations (returned for stars only) |
| formula | String | Object's formula (arabic parts only) |
| reversed | String | Whether the formula was reversed (arabic parts only) |
| longitude | Float | The object's ecliptic longitude in decimal degrees |
| latitude | Float | The object's ecliptic latitude in decimal degrees |
| distance | Float | The object's distance in AU |
| distanceLY | Float | The object's distance in Light Years (returned for stars only) |
| longitudeSpeed | Float | The object's longitude speed in decimal degrees per day |
| latitudeSpeed | Float | The object's latitude speed in decimal degrees per day |
| distanceSpeed | Float | The object's distance changes in AU per day |
| hds | String | The object's gate, line, color, tone and base position for the Human Design System |
| stationary | Boolean | Whether the object is considered "stationary" |
| declination | Float | The object's celestial declination in decimal degrees |
| rightAscension | Float | The object's right ascension in decimal degrees |
| declinationSpeed | Float | The object's declination speed in decimal degrees per day |
| rightAscensionSpeed | Float | The object's right ascension speed in decimal degrees per day |
| magnitude | Float | The object's magnitude |
| angularDiameter | Float | The object's angular diameter in decimal degrees |
| azimuth | Float | The object's azimuth decimal degrees |
| altitude | Float | The object's altitude in decimal degrees |
| error | String | error message (if an error occurs) |

Not all objects support all display options, some are exclusive to certain objects while others might not be available to certain objects. In case a field is not available, it will return `"not available"` instead.

<br>