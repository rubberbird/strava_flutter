# strava_flutter

Dart/flutter package to use Strava API v3

Follow the "new" Authentication process

https://developers.strava.com/docs/authentication/



## API currently supported:

- authorize
- deauthorize


### Athlete related APIs
- getLoggedInAthlete
- updateLoggedInAthlete (scope profile:write)
- getLoggedInAthleteZones
- getGearById
- getStats
### Club related APIs
- getClubById
- getClubActivitiesById (need to be member of the club)
- getClubMembersById (no need to be member of the club)
### Race related APIs
- getRunningRaces
- getRunningRaceById
### Activity related APIs
- createActivity
- uploadActivity (including getUploadById
### Segments related APIs
- getSegmentById
- getLoggedInAthleteStarredSegments
- getLeaderboardBySegmentId




## How to use it

1 - Create a file secret.dart to put the secret shown on  Strava settings related to your app
https://www.strava.com/settings/api

2 - In constants.dart put your appID in clientID

3 - To see debug info in Strava API, set isInDebug to true in globals.dart

4 - Please check examples.dart for the moment

https://github.com/BirdyF/strava_flutter/blob/master/example/lib/main.dart

https://github.com/BirdyF/strava_flutter/blob/master/example/lib/examples.dart


If you have any problem or need an API not yet implemented please post an new issue


## Tested on:
- Android 4.4.2 , 4.4.23
- iOS 12.1, 12.1.2, 12.1.4


## Thanks 

Thanks to Joe Birch, I used his code to better understand Oauth process
https://github.com/hitherejoe/FlutterOAuth

And Javier for https://javiercbk.github.io/json_to_dart/


## License:
strava_flutter is provided under a MIT License. Copyright (c) 2019 Patrick FINK
