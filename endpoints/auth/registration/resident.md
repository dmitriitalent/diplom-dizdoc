https://backend.com/auth/registration/resident POST




**Обрати внимание на [[endpoints/profile/get|get]]. Там дополнительно прописаны visible поля.** Изначально все устанавливается в everyone. Не обязательные поля я собираюсь устанавливать в Null.


```
Пароль
const regex = /^(?=.*\d)(?=.*[!@#$%^&*])[A-Za-z\d!@#$%^&*]{6,}$/;

```
```json
{
	"login": "Turbosrulik", 
	"password": "some!password", 
	"education_email": "example@vuz.education", 
	"consent_user_agreement": True, 
	"hei": "МАИ (Московский Авиационный Институт)", 
	"dormitory": "Икар (ул. Дубосековская, д. 13)",
	"surname": "Иванов", 
	"name": "Иван", 
	"patronymic": "Иванов", 
	"birthdate": "01.01.2000", // no req
	"building": "2", // no req
	"floor": "4", // no req
	"room": "2413", // no req
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
кста вацап вроде должен быть запрещен

предлагаю поле contacts просто как json закинуть в ячейку, я сделаю так что можно будет выбрать среди имеющихся соц. сетей типа телеграм или вк, но если кто то захочет, то сможет вписать свою соц. сеть.

в ответе at и rt
Названия: 
at - accessToken
rt - refreshToken