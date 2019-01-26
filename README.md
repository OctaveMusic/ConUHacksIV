# ConUHacksIV
In support of the fourth edition of ConUHacks, January 26-27 2019; a Major League Hacking event!

## Challenge
### Summary
What if you had access to historical song play information; 180M jukebox song play events, in fact, that occurred across North America in the past 12 months. Knowing each play event contains date, artist, song, genre and geo coordinates, what would you build to help a music product team drive social awareness, analyze trends, discover anomalies, improve music curation, or…?

### API Documentation
https://conuhacks-playback-api.touchtunes.com/docs/

### Secret Authorization Token (*shhhh...!*)
```
9923ac9b-8fd3-421f-b0e5-952f807c6885
```

### Example Usage
#### Getting Plays
```bash
curl -X GET 'https://conuhacks-playback-api.touchtunes.com/plays?startDate=2018-02-19T21:00:00Z&endDate=2018-02-19T22:00:00Z&offset=0' \
     -H 'client-secret: 9923ac9b-8fd3-421f-b0e5-952f807c6885'
```

#### Getting a Song
```bash
curl -X GET https://conuhacks-playback-api.touchtunes.com/song/11088314 \
     -H 'client-secret: 9923ac9b-8fd3-421f-b0e5-952f807c6885'
```

#### Getting an Artist
```bash
curl -X GET https://conuhacks-playback-api.touchtunes.com/artist/1182 \
     -H 'client-secret: 9923ac9b-8fd3-421f-b0e5-952f807c6885'
```
