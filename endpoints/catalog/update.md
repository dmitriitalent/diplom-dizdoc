https://backend.com/catalog PUT

``` json 
{
	"id": 66,
	"name": "Крутая футболка",
	"description": "Принт отличный даже после стирки. 100% хлопок",
	"price": 700,
	"category": "Одежда",
	"viewTemplate": 3,
	"images": ["guid-guid-guid-guid.jpg"],
}
```
return
``` json 
{
	"id": 66,
	"owner": {}, // user data
	"name": "Крутая футболка",
	"description": "Принт отличный даже после стирки. 100% хлопок",
	"price": 700,
	"category": "Одежда",
	"viewTemplate": 3,
	"images": ["guid-guid-guid-guid.jpg"],
	"publishedAt": "166989067887",
	"updatedAt": "166999999987",
}
```