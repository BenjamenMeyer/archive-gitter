# download gitter archives

uses the gitter REST API to download archives of public gitter rooms.

Create a config file using JSON:
```
{
    "token": "<gitter token goes here">",
	"all": false,
	"rooms": [
	]
}
```

The above config file will return a list of all the rooms that archive-gitter sees.
If you want to download archives of all the rooms, set "all" to true.
If you only want a subset of rooms, then put their reported names into the "rooms" listing.

Archives are stored in `archive/room/name.json`.

Subsequent runs check for new messages since last run.

License: CC-0, Public Domain
