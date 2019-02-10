---
layout: page
title: Parameters - Display
navigation: 5
---

<style>
	.inner a {
		color: royalblue;
		font-weight: bold;
	}
	.inner code {
		font-size: 100%;
	}
	.sidebar {
		width: 30%
	}
	.navigation li {
		padding: 5px;
	}
</style>

<script>
	window.onload = function(){
		if (location.hash) {
			let target = location.hash;
			document.querySelector(".content").scroll({top:document.querySelector(target).offsetTop,behavior:"smooth"})
		}
	}
</script>

<br>

## Parameters - Display

An array of planetary values that should be returned. If none is specified, it defaults to `LONGITUDE` and `LONGITUDE_SPEED`.

| option | Descripton |
|---|---|
| LONGITUDE | Longitude (ecliptic coordinates) |
| LATITUDE | Latitude (ecliptic coordinates) |
| ASCENSION | Right Ascension (equatorial coordinates) |
| DECLINATION | Declination (equatorial coordinates) |
| ALTITUDE | Altitude (horizontal coordinates) |
| AZIMUTH | Azimuth (horizontal coordinates) |
| DISTANCE | Distance in AU |
| MAGNITUDE | Magnitude |
| DIAMETER | Angular diameter |
| HDS | Human Design System positions (gate,line,color,tone,base) |
| STATIONS | Whether or not the object is considered "stationary" |
| LONGITUDE_SPEED | Longitude speed (degrees per day) |
| LATITUDE_SPEED | Latitude speed (degrees per day) |
| ASCENSION_SPEED | Right Ascension speed (degrees per day) |
| DECLINATION_SPEED | Declination speed (degrees per day) |
| DISTANCE_SPEED | Distance speed (AU per day) |

<br>

### Parameters - Display Examples

Example for retrieving `Longitude`, `Latitude` and `Declination` values:

| GET | POST |
|---|---|
|`display=LONGITUDE|LATITUDE|DECLINATION`|`display:["LONGITUDE","LATITUDE","DECLINATION"]`|

<br><br><br>