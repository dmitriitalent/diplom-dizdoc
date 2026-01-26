https://backend.com/catalog POST

image-guid я буду генерировать сам на фронте. файл также сам переименовывать буду. После запроса отсылаю картинки через [[addImages]]

``` json
{
	"ownerId": 41, // user 
	"name": "Нефорская футболка",
	"description": "Принт начал трескаться после стирки. 100% хлопок",
	"price": 500,
	"category": "select",
	"viewTemplate": 2, // цифра которая нужна чисто мне, по ней не планируется фильтрации. 1 байта хватит.
	"images": ["guid-guid-guid-guid.jpg"],
}
```
return
``` json 
{
	"id": 66,
	"owner": {}, // user data
	"name": "Нефорская футболка",
	"description": "Принт начал трескаться после стирки. 100% хлопок",
	"price": 500,
	"category": "select",
	"viewTemplate": 2,
	"images": ["guid-guid-guid-guid.jpg"],
	"publishedAt": "166989067887",
	"updatedAt": "166989067887",
}
```