"https://backend.com/activity?id=133" GET


``` json 
{
	"id": 133,
	"owner": {}, // user data
	"name": "Турнир по шашкам",
	"description": "Туринр по шашкам будет проводиться с 18:00 до 24:00",
	"images": ["guid-guid-guid-guid.jpg"],
	"isPrivate": True,
	"inviteCode": "H2tre7v116hH9h",
	"visiters": [
		{
			"user": {}, // user data
			"signUpAt": "00:00:00T01.01.0001" // время регистрации 
		}
	],
	"publishedAt": "166989067887",
	"updatedAt": "166989067887",
}
```
если owner.id != at.userId то inviteCode = null

``` json 
{
	"id": 133,
	"owner": {}, // user data
	"name": "Турнир по шашкам",
	"description": "Туринр по шашкам будет проводиться с 18:00 до 24:00",
	"images": ["guid-guid-guid-guid.jpg"],
	"isPrivate": True,
	"inviteCode": Null,
	"visiters": [
		{
			"user": {}, // user data
			"signUpAt": "00:00:00T01.01.0001" // время регистрации 
		}
	],
	"publishedAt": "166989067887",
	"updatedAt": "166989067887",
}
```