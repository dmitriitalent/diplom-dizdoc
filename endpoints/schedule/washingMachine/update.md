https://backend.com/schedule/washingmachine PUT

``` json
{
	"id": 1,
	location: "11** левая",
},
```

return 
``` json
{
	"id": 1,
	location: "11** левая",
	"week": [
		{ // вчера
			"schedule": [
				{ "from": 0, "till": 90, "user": {} },
				{ "from": 91, "till": 120, "user": {} },
				{ "from": 121, "till": 200, "user": {} }
				// ...
			]	
		},
		{ // седгоня
			"schedule": []	
		},
	]
},
```