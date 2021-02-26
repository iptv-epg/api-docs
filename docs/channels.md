# Countries and channels

The `/channels` endpoint provides access to the list of all countries and channels available on epg.best.
This request does not require any authentication.

## List countries

`GET /api/countries`

`GET /api/countries?page={integer}&per_page={integer}`

## List all channels

`GET https://epg.best/api/channels`

```json
[
    {
        "country": "at",
        "display_name": "3sat", 
        "tvg_id": "3sat.at"
    },
    {
        "country": "at",
        "display_name": "Arte AT",
        "tvg_id": "ARTE.at"
    }
]
```