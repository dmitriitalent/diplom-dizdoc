https://backend.com/auth/registration/other POST





**Обрати внимание на [[endpoints/profile/get|get]]. Там дополнительно прописаны visible поля.** Изначально все устанавливается в everyone. Не обязательные поля я собираюсь устанавливать в Null. 






```json
{
	"login": "Turbosrulik",
	"password": "some!password",
	"key": "guid-guid-guid12-guid",
	"consent_user_agreement": True,
}
```
в ответе at и rt

Названия: 
at - accessToken
rt - refreshToken