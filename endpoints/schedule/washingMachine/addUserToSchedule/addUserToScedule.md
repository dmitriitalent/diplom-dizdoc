https://backend.com/schedule/washingmachine POST

проживающего получить по at

``` json
{
	"id": 2,
	"from": 515,
	"till": 575,
}
```

return
``` json
{
	"id": 2,
	location: "11** правая",
	"week": [
		{
			// дни ранее ...
			"schedule": [ // вчера
				{ "from": 0, "till": 90, "user": {} },
				{ "from": 91, "till": 120, "user": {} },
				{ "from": 121, "till": 200, "user": {} },
				// ...
			]	
		},
		{ // седгоня
			"schedule": [
				{ "from": 515, "till": 575, "user": {} }
			]	
		},	
	]
}	
```