### Тестовое задание "Компонент сборок проекта"

Нужно сделать страницу для отображения списка проектов и списка его сборок.
Компонент состоит из 2 "экранов"

![Prototype](https://user-images.githubusercontent.com/3533939/67852217-1109f780-fb1d-11e9-9abd-455077cb46e2.png)

Первый - выводит уникальный список проектов
по клику на строчку списка, открывается второй экран 

Переход между экранами и анимация а-ля настройки в ios (https://experience.sap.com/fiori-design-ios/wp-content/uploads/sites/23/2017/07/push.gif)

Второй - список сборок по выбранному проекту
В шапке выводит название выбранного проекта и контрол для возврата к списку проектов.
В элементе стиска отображается `id` сборки, статус и имя инициатора (цветовое кодирование статуса произвольное)

Дизайн и верстка (цвета, шрифты, отступы, сетки) произвольно, достаточно сходства с прототипом.

Входящие данные имеют вид: 

```
[
  {
    "id": 455329,
    "project": "Quintity",
    "status": "error",
    "initiator": "Gail Barron"
  },
  {
    "id": 603571,
    "project": "Futurize",
    "status": "error",
    "initiator": "Gretchen Guy"
  },
  {
    "id": 119844,
    "project": "Futurize",
    "status": "success",
    "initiator": "Mcconnell Phillips"
  },
  {
    "id": 101638,
    "project": "Quintity",
    "status": "success",
    "initiator": "Jordan Hamilton"
  },
  {
    "id": 73782,
    "project": "Myopium",
    "status": "success",
    "initiator": "Mae Holden"
  },
  {
    "id": 614340,
    "project": "Myopium",
    "status": "success",
    "initiator": "Reynolds Chen"
  },
  {
    "id": 566761,
    "project": "Myopium",
    "status": "pending",
    "initiator": "Caldwell Peterson"
  },
  {
    "id": 498651,
    "project": "Myopium",
    "status": "success",
    "initiator": "Wolfe Barnett"
  },
  {
    "id": 62377,
    "project": "Sultraxin",
    "status": "pending",
    "initiator": "Hannah Strickland"
  },
  {
    "id": 255727,
    "project": "Virva",
    "status": "pending",
    "initiator": "Chasity David"
  },
  {
    "id": 365782,
    "project": "Cubix",
    "status": "error",
    "initiator": "Lara Henderson"
  },
  {
    "id": 409981,
    "project": "Cubix",
    "status": "success",
    "initiator": "Freda Hardy"
  },
  {
    "id": 498118,
    "project": "Eternis",
    "status": "error",
    "initiator": "Violet Pope"
  },
  {
    "id": 641329,
    "project": "Eternis",
    "status": "success",
    "initiator": "Allyson Winters"
  },
  {
    "id": 451203,
    "project": "Eternis",
    "status": "error",
    "initiator": "Brenda Joyner"
  },
  {
    "id": 377864,
    "project": "Anivet",
    "status": "success",
    "initiator": "Jeannette Olson"
  },
  {
    "id": 200836,
    "project": "Anivet",
    "status": "pending",
    "initiator": "Kane Fulton"
  },
  {
    "id": 487570,
    "project": "Anivet",
    "status": "pending",
    "initiator": "Letitia Farmer"
  },
  {
    "id": 555975,
    "project": "Amtas",
    "status": "success",
    "initiator": "Lewis Holmes"
  },
  {
    "id": 540501,
    "project": "Amtas",
    "status": "error",
    "initiator": "Dunlap Stanton"
  }
]
```

### Уловия и тех требования к реализации

 - стек React/ Redux / thunk
 - api ручку можно за mock'ать
 - css препроцессор на выбор
 - сборщик webpack
 - размещение на гитхаб
 - в качестве сервера допускается использование webpack-dev-server
 - НЕ использовать JS для анимации переходов
 - НЕ использовать ui библиотеки (Material UI, bootstrap и пр)
 - НЕ использовать роутинг библиотеки
 - НЕ использовать React Create App - нужно написать минимально необходимый билд конфиг 