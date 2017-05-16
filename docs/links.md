# User links

Business users who have a user based subscription have a number of custom links that can be given to own users. 

## List all user links

`GET https://www.iptv-epg.com/api/links`

```json
[
	{
		"id": 101,
		"url": "http:\/\/iptv-epg.com\/r65-example.xml"
	},
	{
		"id": 102,
		"url": "http:\/\/iptv-epg.com\/r66-example.xml"
	},
    (...)
]
```

## Reset a links

You can reset a link using its ID by sending the following `POST` request. It will return the newly reset link.

`POST https://www.iptv-epg.com/api/links/reset/{id}`

```json
{
    "id": 101,
    "url": "http:\/\/iptv-epg.com\/r65-example.xml"
}
```
