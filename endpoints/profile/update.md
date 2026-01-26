https://backend/profile PUT

Сводка: Нельзя изменить login, password, hei. Это делается отдельно в [[updateLogin]] и [[updatePassword]]. Hei вуз менять тоже надо отдельно, потому что чел может перевестись в питер и соответственно надо будет удалять его вещи из каталога и услуги (предлагаю не думать об этом пока). Хотя такой инструмент нужно будет создать для удалений людей отчисленных из вуза.

visible - ADMIN | FRIEND | EVERYONE

```json
{
	"id": 3456789,
	"educationEmail": "example@vuz.education",
	"consentUserAgreement": True,
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
	"contacts": [
		{
			"key": "phoneNumber",
			"value": "+7 123 456 78 90",
			"visibility": "FRIEND",
		},
		{ 
			"key": "email",
			"value": "personal@gmail.com",
			"visibility": "FRIEND",
		},
		{
			"key": "telegram",
			"value": "@dmitrii_talent",
			"visibility": "EVERYONE",
		},
		{
			"key": "vk",
			"value": "@dmitrii_talent",
			"visibility": "EVERYONE",
		},
		{
			"key": "whatsapp",
			"value": "@янезнаюкакввацапезаписываетсятег",
			"visibility": "EVERYONE",
		},
		{
			"key": "steam",
			"value": "stritten",
			"visibility": "FRIEND",
		},
	],
}
```