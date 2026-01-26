https://backend.com/activity PUT


``` json 
{
	"id": 133,
	"name": "Турнир по шахматам",
	"description": "Туринр по шахматам будет проводиться с 18:00 до 24:00",
	"images": ["guid-guid-guid-guid.jpg"],
	"viewTemplate": 3,
	"isPrivate": True,
}
```

return 

``` json 
{
	"id": 133,
	"owner": {}, // user data
	"name": "Турнир по шахматам",
	"description": "Туринр по шахматам будет проводиться с 18:00 до 24:00",
	"images": ["guid-guid-guid-guid.jpg"],
	"viewTemplate": 3,
	"isPrivate": True,
	"inviteCode": "H2tre7v116hH9h",
	"visiters": [
		{
			"user": {}, // user data
			"signUpAt": "00:00:00T01.01.0001" // время регистрации 
		}
	],
	"publishedAt": "166989067887",
	"updatedAt": "166999999987",
}
```