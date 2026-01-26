https://backend.com/news POST 

**pinned_service возможно стоит переименовать**

image-guid я буду генерировать сам на фронте. файл также сам переименовывать буду. После запроса отсылаю картинки через [[addImages]]

```json
{
	"authorId": 52, // user data
	"name": "Крутое название для новости",
	"description": "Какое то овердлинное описание которое мне лень писать длинным",
	"images": ["guid-guid-guid-guid.jpg"],
	viewTemplate: 1,
	"pinned_activities": [ 
		132, // activity id 
		133 
	],
	"pinned_services": [ 
		232, // service id 
		233 
	],
} 
```

```json
{
	"id": 23,
	"author": {}, // user data
	"name": "Крутое название для новости",
	"description": "Какое то овердлинное описание которое мне лень писать длинным",
	"images": ["guid-guid-guid-guid.jpg"],
	viewTemplate: 1,
	"pinned_activities": [ 
		132, // activity id 
		133
	],
	"pinned_services": [ 
		232, // service id 
		233 
	],
	"publishedAt": "166989067887",
	"updatedAt": "166989067887",
} 
```