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
	"passwordConfirm": "some!password",
	"education_email": "example@vuz.education", 
	"consent_user_agreement": True, 
	"hei": "МАИ (Московский Авиационный Институт)", 
	"birthdate": "01.01.2000",
	"dormitory": "Икар (ул. Дубосековская, д. 13)",
	"building": "2",
	"floor": "4",
	"room": "2413",
	"surname": "Иванов", 
	"name": "Иван", 
	"patronymic": "Иванов", 
}
```
кста вацап вроде должен быть запрещен

предлагаю поле contacts просто как json закинуть в ячейку, я сделаю так что можно будет выбрать среди имеющихся соц. сетей типа телеграм или вк, но если кто то захочет, то сможет вписать свою соц. сеть.

в ответе at и rt
Названия: 
at - accessToken
rt - refreshToken