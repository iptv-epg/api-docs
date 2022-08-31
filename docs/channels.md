# Countries and channels

The `/channels` endpoint provides access to the list of all countries and channels available on epg.best. This request does not require any authentication.

## List countries

`GET /api/countries`

```json
{
  "current_page": 1,
  "data": [
    {
      "code": "al",
      "name": "Albania"
    },
    {
      "code": "dz",
      "name": "Algeria"
    }
  ],
  "first_page_url": "/?page=1",
  "from": 1,
  "last_page": 6,
  "last_page_url": "/?page=6",
  "next_page_url": "/?page=2",
  "path": "/",
  "per_page": 20,
  "prev_page_url": null,
  "to": 20,
  "total": 114
}
```

## List all channels

`GET https://epg.best/api/channels`

```json
[
  {
    "country_id": 120,
    "display_name": "TTV One SB",
    "tvg_id": "TTVone.sb",
    "country": "sb"
  },
  {
    "country_id": 120,
    "display_name": "TTV Two SB",
    "tvg_id": "TTVtwo.sb",
    "country": "sb"
  }
]
```

## List channels (V2)

`GET https://epg.best/v2/channels`


Filters:
 - `country_code`: Country code
 - `channels[]`: Channel Tvg ID-s
 - `search`: Search in channel display name
 - `per_page`: Per page number
 - `page`:  Page  

Example: `https://epg.best/api/v2/channels?country_code=hu&channel[]=RTLGold.hu&search=RTL&page=2&per_page=50`

```json
{
  "current_page": 1,
  "data": [
    {
      "display_name": "3 Plus AL",
      "country_id": 48,
      "tvg_id": "3Plus.al",
      "country": "al"
    },
    {
      "display_name": "Alsat AL",
      "country_id": 48,
      "tvg_id": "AlsatM.al",
      "country": "al"
    }
  ],
  "first_page_url": "https://epg.best/api/v2/channels?page=1",
  "from": 1,
  "last_page": 4,
  "last_page_url": "https://epg.best/api/v2/channels?page=4",
  "next_page_url": "https://epg.best/api/v2/channels?page=2",
  "path": "https://epg.best/api/v2/channels",
  "per_page": 20,
  "prev_page_url": null,
  "to": 20,
  "total": 71
}
```
