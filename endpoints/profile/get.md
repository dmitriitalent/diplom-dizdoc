https://backend/profile/51 GET

Тут удалено поле password

visible - ADMIN | FRIEND | EVERYONE
```json
{
	"id": 78,
	"login": "Turbosrulik",
	"educationEmail": "example@vuz.education",
	"consentUserAgreement": True,
	"hei": "МАИ (Московский Авиационный Институт)",
	"dormitory": {
		"value": "Икар (ул. Кругоуховая, д. 10)",
		"visibility": "ADMIN",
	},
	"surname": {
		"value": "Иванов",
		"visibility": "EVERYONE",
	},
	"name": {
		"value": "Иван",
		"visibility": "EVERYONE",
	},
	"patronymic": {
		"value": "Иванович",
		"visibility": "FRIEND",
	},
	"birthdate": {
		"value": "165779787663",
		"visibility": "FRIEND",
	},
	"building": {
		"value": "2",
		"visibility": "ADMIN",
	},
	"floor": {
		"value": "4",
		"visibility": "ADMIN",
	},
	"room": {
		"value": "2413",
		"visibility": "ADMIN",
	},
	"contacts": {
		"phoneNumber": {
			"value": "+7 123 456 78 90",
			"visibility": "FRIEND",
		},
		"email": {
			"value": "personal@gmail.com",
			"visibility": "FRIEND",
		},
		"telegram": {
			"value": "@dmitrii_talent",
			"visibility": "EVERYONE",
		},
		"vk": {
			"value": "@dmitrii_talent",
			"visibility": "EVERYONE",
		},
		"whatsapp": {
			"value": "@янезнаюкакввацапезаписываетсятег",
			"visibility": "EVERYONE",
		},
		"steam": {
			"value": "stritten",
			"visibility": "FRIEND",
		},
	},
	
	"friends": {
		"value": [], // array of user data
		"visibility": "FRIEND"
	},	
	
	"ratedNews": [{
		id: 5235,
		like: True,
	}],
	
	"ratedProducts": [{
		id: 215,
		like: False
	},
	{
		id: 216,
		like: True
	}],
	
	"ratedActivities": [{
		id: 882,
		like: False
	}],
	"createdAt": "166989067887"
}
```

если at.role == "ADMIN" то вернуть надо всю доступную информацию вплоть до настроек приватности. (Как будто запрос сделал владелец)

если at.userId != param_id (accessToken), то все unvisible поля для этого пользователя не возвращаются в запросе, исчезает обёртка. Рассмотрен случай для friend
```json
{
	"id": 3456789,
	"login": "Turbosrulik",
	"educationEmail": "example@vuz.education",
	"hei": "МАИ (Московский Авиационный Институт)",
	"surname": "Иванов",
	"name": "Иван",
	"patronymic": "Иванов",
	"birthdate": "01.01.2000",
	"contacts": {
		"phoneNumber": "+7 123 456 78 90",
		"email": "personal@gmail.com",
		"telegram": "@dmitrii_talent",
		"vk": "@dmitrii_talent",
		"whatsapp": "@янезнаюкакввацапезаписываетсятег",
		"steam": "stritten",
		"pinterest": "dmitriitalent",
	},
	
	"friends": [],
}
```

Даже учитывая что я пишу SSR получать с сервера полные данные о пользователе нельзя. Потому что есть шанс что мне придётся использовать запрос не с сервера, а с клиента на бек. Такой запрос можно будет перехватить. 