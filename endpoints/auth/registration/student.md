https://backend.com/auth/registration/student POST





**Обрати внимание на [[endpoints/profile/get|get]]. Там дополнительно прописаны visible поля.** Изначально все устанавливается в everyone. Не обязательные поля я собираюсь устанавливать в Null.






```json
{
	"login": "Turbosrulik",
	"password": "some!password",
	"passwordConfirm": "some!password",
	"education_email": "example@vuz.education",
	"consent_user_agreement": True,
	"hei": "МАИ (Московский Авиационный Институт)",
	"birthdate": "01.01.2000"
}
```

в ответе at и rt 
Названия: 
at - accessToken
rt - refreshToken