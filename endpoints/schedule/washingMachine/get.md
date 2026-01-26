https://backend.com/schedule/washingmachine GET
получать общежитие по at

schedule содержит массив последних 7 дней. Временные метки в минутах. Всего 24 * 60 = 1440

``` json
[
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
	
	{
		"id": 2,
		location: "11** правая",
		"week": [
			{
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
	}	
]
```