https://backend.com/news PUT 

image-guid я буду генерировать сам на фронте. файл также сам переименовывать буду. Затем следующим запросом сразу буду отсылать addImage

```json
{
	"name": "Крутое название для новости",
	"description": "Какое то овердлинное описание которое мне лень писать длинным",
	"images": ["guid-guid-guid-guid.jpg"],
	viewTemplate: 4,
	"pinned_activities": [ 
		132, // activity id 
		134
	],
	"pinned_services": [ 
		232, // service id 
		234 
	],
} 
```

return
```json
{
	"id": 23,
	"author": {}, // user data
	"name": "Крутое название для новости",
	"description": "Какое то овердлинное описание которое мне лень писать длинным",
	"images": ["guid-guid-guid-guid.jpg"],
	viewTemplate: 4,
	"pinned_activities": [ 
		132, // activity id 
		134
	],
	"pinned_services": [ 
		232, // service id 
		234 
	],
	"publishedAt": "166989067887",
	"updatedAt": "166999999987",
} 
```
```