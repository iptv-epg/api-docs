# Programmes

The `/programmes` endpoint provides access to the list of all programmes available on epg.best.

## List programmes

`GET /api/programmes`


Filters:   
 - `date`: which days
 - `channels[]`: Channel Tvg ID-s
 - `per_page`: Per page number
 - `page`:  Page  

Exmaple: `https://epg.best/api/programmes?date=2020-09-25&channels[]=RTLKlub.hu&channels[]=RTLGold.hu&page=1&per_page=30`

```json
{
  "current_page": 1,
  "data": {
    "AmericanHeroesChannel.us": [
      {
        "start_utc": 1614294000,
        "stop_utc": 1614297600,
        "title": "WWII in the Pacific",
        "sub-title": "No Surrender",
        "desc": "The war drags on in 1945 as the Japanese are determined to fight on, but a secret U.S. weapon could hasten the end of hostilities and save thousands of lives",
        "channel_name": "AmericanHeroesChannel.us",
        "category": "Documentary"
      },
      {
        "start_utc": 1614297600,
        "stop_utc": 1614301200,
        "title": "Hitler's Empire: The Post-War Plan",
        "sub-title": "America",
        "desc": "Support for the National Socialist movement within America is uncovered. Included: revealing outposts of Nazi Germany within the land of the free; and the man thought he believed he was the American Fuhrer",
        "channel_name": "AmericanHeroesChannel.us",
        "category": "Documentary"
      }
    ]
  },
  "first_page_url": "https://epg.best/api/programmes?page=1",
  "from": 1,
  "last_page": 29,
  "last_page_url": "https://epg.best/api/programmes?page=29",
  "next_page_url": "https://epg.best/api/programmes?page=2",
  "path": "https://epg.best/api/programmes",
  "per_page": 20,
  "prev_page_url": null,
  "to": 20,
  "total": 575
}
```
