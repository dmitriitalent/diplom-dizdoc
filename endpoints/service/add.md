image-guid я буду генерировать сам на фронте. файл также сам переименовывать буду. После запроса отсылаю картинки через [[addImages]]
paymentMode : ONCE | HOURLY | CONTRACT



``` json
{
	"name": "Репетиторство по физике",
	"description": "Помогу вам разобраться в физике. Каждый день с 18:00 до 24:00",
	"viewTemplate": 1,
	"price": 500,
	"images": ["guid-guid-guid-guid.jpg"],
}
```

return
``` json 
{
	"id": 133,
	owner: {},
	"name": "Репетиторство по физике",
	"description": "Помогу вам разобраться в физике. Каждый день с 18:00 до 24:00",
	"viewTemplate": 1,
	"price": 500,
	"paymentMode": "once",
	"images": ["guid-guid-guid-guid.jpg"],
	"comments": [{}],
	"publishedAt": "166989067887",
	"updatedAt": "166989067887",
}
```