# lat-long

https://www.timeanddate.com/time/map/
https://laendercode.net/en/
https://gml.noaa.gov/grad/solcalc/

## todo
- fix the ramp over boundaries, e.g. .75 should transition to 1.1

## coords

https://www.google.com/maps/
({
  frigg_fjord_GRL:      { latitude:  83.1166065, longitude:  -41.9839829 },
  reykjavic_ISL:        { latitude:  64.1334735, longitude:  -21.9224815 },
  columbus_OH_USA:      { latitude:  39.9828671, longitude:  -83.1309138 },
  san_francisco_CA_USA: { latitude:  37.7576793, longitude: -122.5076402 },
  singapore_SGP:        { latitude:   1.3139961, longitude:  103.7041623 },
  panama_city_PAN:      { latitude:   9.0813885, longitude:  -79.5932249 },
  antananarivo_MDG:     { latitude: -18.887626,  longitude:   47.3724268 },
  wellington_NZL:       { latitude: -41.2528753, longitude:  174.614173  },
  punta_arenas_CHL:     { latitude: -53.1417468, longitude:  -70.9763068 },
  mcmurdo_station_ATA:  { latitude: -77.7240158, longitude:  164.7726887 },
})

https://www.latlong.net/
({
  san_francisco_CA_USA: { latitude:  37.774929, longitude: -122.419418 },
  columbus_OH_USA:      { latitude:  39.961178, longitude:  -82.998795 },
  reykjavic_ISL:        { latitude:  64.147210, longitude:  -21.942400 },
  punta_arenas_CHL:     { latitude: -53.161968, longitude:  -70.909561 },
})

## self-serve
https://github.com/mbostock/solar-calculator

`solar.noon(date, longitude)`
Given a date and a longitude in degrees, returns the time of the solar noon. (TODO This description isn’t quite right, because the date is first floored to the UTC day boundary and then adjusted based on the specified longitude.)

`solar.rise(date, latitude, longitude)`
Given a date and a latitude and longitude in degrees, returns the time of sunrise. (TODO Describe more precisely the date of the returned sunrise.)

`solar.set(date, latitude, longitude)`
Given a date and a latitude and longitude in degrees, returns the time of sunset. (TODO Describe more precisely the date of the returned sunset.)


## polar day

```js
results: Object {
  sunrise: "1970-01-01T00:00:01+00:00"
  sunset: "1970-01-01T00:00:01+00:00"
  solar_noon: "2022-08-03T14:54:08+00:00"
  day_length: 0
  civil_twilight_begin: "1970-01-01T00:00:01+00:00"
  civil_twilight_end: "1970-01-01T00:00:01+00:00"
  nautical_twilight_begin: "1970-01-01T00:00:01+00:00"
  nautical_twilight_end: "1970-01-01T00:00:01+00:00"
  astronomical_twilight_begin: "1970-01-01T00:00:01+00:00"
  astronomical_twilight_end: "1970-01-01T00:00:01+00:00"
}
```


## polar night

```js
results: Object {
  sunrise: "1970-01-01T00:00:00+00:00"
  sunset: "1970-01-01T00:00:00+00:00"
  solar_noon: "2022-08-03T01:07:09+00:00"
  day_length: 0
  civil_twilight_begin: "2022-08-02T23:45:38+00:00"
  civil_twilight_end: "2022-08-03T02:28:40+00:00"
  nautical_twilight_begin: "2022-08-02T20:48:22+00:00"
  nautical_twilight_end: "2022-08-03T05:25:55+00:00"
  astronomical_twilight_begin: "2022-08-02T18:50:48+00:00"
  astronomical_twilight_end: "2022-08-03T07:23:30+00:00"
}
```


