https://backend.com/auth/registration/student POST





**Обрати внимание на [[endpoints/profile/get|get]]. Там дополнительно прописаны visible поля.** Изначально все устанавливается в everyone. Не обязательные поля я собираюсь устанавливать в Null.






```json
{
	"login": "Turbosrulik",
	"password": "some!password",
	"education_email": "example@vuz.education",
	"consent_user_agreement": True,
	"hei": "МАИ (Московский Авиационный Институт)",
	"surname": "Иванов",
	"name": "Иван",
	"patronymic": "Иванов",
	"birthdate": "01.01.2000", // no req
	"contacts": { // no req
		"phone_number": "+7 123 456 78 90",
		"email": "personal@gmail.com",
		"telegram": "@dmitrii_talent",
		"vk": "@dmitrii_talent",
		"whatsapp": "@янезнаюкакввацапезаписываетсятег",
		"steam": "stritten",
		"pinterest": "dmitriitalent",
	},
}
```

в ответе at и rt 
Названия: 
at - accessToken
rt - refreshToken