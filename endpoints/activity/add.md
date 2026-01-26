https://backend.com/activity POST

image-guid я буду генерировать сам на фронте. файл также сам переименовывать буду. После запроса отсылаю картинки через [[addImages]]

На беке надо генерировать InviteCode. Пользователи смогут вписать его и присоединиться к закрытому мероприятию.  

visible - ADMIN | FRIEND | EVERYONE

``` json
{
	"owner": {}, // user data
	"name": "Турнир по шашкам",
	"description": "Туринр по шашкам будет проводиться с 18:00 до 24:00",
	"images": ["guid-guid-guid-guid.jpg"],
	"viewTemplate": 2, // цифра которая нужна чисто мне, по ней не планируется фильтрации. 1 байта хватит.
	"isPrivate": False,
}
```

return
``` json 
{
	"id": 133,
	"name": "Турнир по шашкам",
	"description": "Туринр по шашкам будет проводиться с 18:00 до 24:00",
	"images": ["guid-guid-guid-guid.jpg"],
	"viewTemplate": 2,
	"score": 0,
	"isPrivate": False,
	"inviteCode": "H2tre7v116hH9h",
	"visiters": [],
	"publishedAt": "166989067887",
	"updatedAt": "166989067887",
}
```