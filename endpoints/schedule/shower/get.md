https://backend.com/schedule/shower?id=1 GET
получать общежитие по at

gender = MAN | WOMAN

schedule содержит массив дней недели. Временные метки в минутах. Всего 24 * 60 = 1440
Если не работает в этот день то пустой массив. 

``` json
[
	{
		"id": 1,
		location: "11**",
		"schedule": [
			[
				{ "from": 0, "till": 410, "gender": "MAN" },
				{ "from": 440, "till": 1130, "gender": "MAN" },
				{ "from": 1160, "till": 1440, "gender": "MAN" }
			],
			[],
			[
				{ "from": 0, "till": 410, "gender": "MAN" },
				{ "from": 440, "till": 1130, "gender": "MAN" },
				{ "from": 1160, "till": 1440, "gender": "MAN" }
			],
			[
				{ "from": 0, "till": 410, "gender": "MAN" },
				{ "from": 440, "till": 1130, "gender": "MAN" },
				{ "from": 1160, "till": 1440, "gender": "MAN" }
			],
			[
				{ "from": 0, "till": 410, "gender": "MAN" },
				{ "from": 440, "till": 1130, "gender": "MAN" },
				{ "from": 1160, "till": 1440, "gender": "MAN" }
			],
			[
				{ "from": 0, "till": 410, "gender": "MAN" },
				{ "from": 440, "till": 1130, "gender": "MAN" },
				{ "from": 1160, "till": 1440, "gender": "MAN" }
			],
			[
				{ "from": 0, "till": 410, "gender": "MAN" },
				{ "from": 440, "till": 1130, "gender": "MAN" },
				{ "from": 1160, "till": 1440, "gender": "MAN" }
			],
		]
	},
	
	{
		"id": 2,
		location: "11**",
		"schedule": [
			[
				{ "from": 0, "till": 410, "gender": "WOMAN" },
				{ "from": 440, "till": 1130, "gender": "WOMAN" },
				{ "from": 1160, "till": 1440, "gender": "WOMAN" }
			],
			[
				{ "from": 0, "till": 60, "gender": "WOMAN" },
				{ "from": 61, "till": 120, "gender": "MAN" },
				{ "from": 121, "till": 180, "gender": "WOMAN" },
				{ "from": 181, "till": 240, "gender": "MAN" },
				{ "from": 241, "till": 300, "gender": "WOMAN" },
				{ "from": 301, "till": 360, "gender": "MAN" },
				// ... каждый час меняется так как у мужчин в этот день ремонт 
			],
			[
				{ "from": 0, "till": 410, "gender": "WOMAN" },
				{ "from": 440, "till": 1130, "gender": "WOMAN" },
				{ "from": 1160, "till": 1440, "gender": "WOMAN" }
			],
			[
				{ "from": 0, "till": 410, "gender": "WOMAN" },
				{ "from": 440, "till": 1130, "gender": "WOMAN" },
				{ "from": 1160, "till": 1440, "gender": "WOMAN" }
			],
			[
				{ "from": 0, "till": 410, "gender": "WOMAN" },
				{ "from": 440, "till": 1130, "gender": "WOMAN" },
				{ "from": 1160, "till": 1440, "gender": "WOMAN" }
			],
			[
				{ "from": 0, "till": 410, "gender": "WOMAN" },
				{ "from": 440, "till": 1130, "gender": "WOMAN" },
				{ "from": 1160, "till": 1440, "gender": "WOMAN" }
			],
			[
				{ "from": 0, "till": 410, "gender": "WOMAN" },
				{ "from": 440, "till": 1130, "gender": "WOMAN" },
				{ "from": 1160, "till": 1440, "gender": "WOMAN" }
			],
		]
	}	
]
```