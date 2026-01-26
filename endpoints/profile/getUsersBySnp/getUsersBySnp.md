https://backend.com/profile/getUsersBySnp GET
поиск пользователей по ФИО в своём вузе

ограничения: 

| STUDENT    | получаем профиль через access token |
| ---------- | ----------------------------------- |
| RESIDENT   | получаем профиль через access token |
| COMMANDANT | получаем профиль через access token |
| ADMIN      | получаем профиль через access token |
| MODERATOR  | не ограничено                       |
| DEVELOPER  | не ограничено                       |

```json
[
	{
		"surname": "Гришков",
		"name": "Дмитрий",
		"patronimyc": "Александрович"
	},
	{
		"surname": "Дерихов",
		"name": "Алексей",
		"patronimyc": "Александрович"
	}
]
```

return
``` json
[
	{}, // user data
	{} // user data
]
```