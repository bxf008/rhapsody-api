rhapsody-api
===

NodeJS API wrapper for Rhapsody/Napster.  Honestly, I have a fancy TV and I want to build a Rhapsody integrated app for it.  Hopefully, others will find this useful as well.  This library implements promises.  Head on over to https://developer.rhapsody.com/ and sign up for developer account.


## Installation
```
npm install rhapsody-api
```

## Usage
```javascript
var Rhapsody = require("rhapsody-api")("YOUR-ACCESS-TOKEN");

Rhapsody.topArtists().then(function(resp){
  console.log(resp);
});
```

## API Reference
Metadata APIs
```javascript
.topArtists([params])
.artistDetails(artist)
.artistBio(artist)
.artistNewReleases(artist [, params])
.artistTopAlbums(artist [. params])
.artistDiscography(artist [. params])
.artistTopTracks(artist [. params])
.artistImages(artist)
.similarArtists(artist)
.artistEditorialPost(artist)
.newAlbums([params])
.staffPickAlbums([params])
.topAlbums([params])
.albumDetails(album)
.albumTracks(album)
.albumImages(album)
.similarAlbums(album)
.albumReviews(album)
.getTopTracks([params])
.getTrackDetails(track)
```
Member APIs
```javascript
.myFavorites(access_token)
.getMyLibraryArtists(access_token)
.getMyPlaylists(access_token)
.getPlaylistDetails(access_token)
.getPlaylistTracks(access_token)
.getRecentArtists(access_token)
.getRecentGenres(access_token)
.getRecentListens(access_token)

```


