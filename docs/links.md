# User links

Business users who have a user based subscription have a number of custom links that can be given to own users. 

## List all user links

`GET https://epg.best/api/links`

```json
[
	{
		"id": 101,
		"m3u_user": "example",
		"m3u_password": "example",
        "expiration_date": "2021-01-01 00:00:00",
		"url": "http:\/\/epg.best\/r65-example.xml",
		"m3u_url": "http:\/\/epg.best\/r65-example.m3u",
		"enigma2_url": "http:\/\/epg.best\/enigma2\/r65-example.zip",
        "tv_app_code": "20 00 00 00 00 00"
	},
	{
		"id": 102,
		"m3u_user": "example",
		"m3u_password": "example",
		"url": "http:\/\/epg.best\/r66-example.xml",
		"m3u_url": "http:\/\/epg.best\/r66-example.m3u",
		"enigma2_url": "http:\/\/epg.best\/enigma2\/r66-example.zip",
		"tv_app_code": "20 00 00 00 00 00"
	}
]
```

## Reset a link

You can reset a link using its ID by sending the following `POST` request. It will return the newly reset link.

`POST https://epg.best/api/links/reset/{id}`

```json
{
    "id": 101,
    "url": "http:\/\/epg.best\/r65-example.xml"
}
```
