# User data

To access user data, the client needs to authenticate itself using a valid API key. Please refer to the authentication 
docs for details.

## Accessing user data

Currently, only the EPG URL of the user is readable. The EPG is either a raw XML file  or is compressed using GZIP 
depending on the settings of the user.

`GET https://epg.best/api/user`

```json
{
    	"epg": "http:\/\/epg.best\/fa-abcdef.xml.gz"
}
```