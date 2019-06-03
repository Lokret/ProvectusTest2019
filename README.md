# Тестовое

- - - - -

### 1. HTML&CSS
Необходимые материалы в папке [Level1_Html&css](https://github.com/DmitryIvanov92/formula-fe-test/tree/master/Level2_Javascript).

Цель - Сверстать [макет](
https://github.com/DmitryIvanov92/formula-fe-test/blob/master/Level1_Html%26css/resources/homepage.psd).    
Любыми средствами, требования два: 
1. работать в последних двух версиях современных браузеров
2. быть адаптивным

- - - - - - - 

### 2. Javascript
Необходимые материалы в папке [Level2_Javascript](https://github.com/DmitryIvanov92/formula-fe-test/tree/master/Level2_Javascript).

Есть массив объектов формата
```
{
  name: 'Name', 
  description: 'Description', 
  expirationDate: '01-30-1999' 
}
```
Необходимо редактировать функцию ```filterByExpiration``` в файле script.js, которая будет получать на вход исходный массив и вернет массив только из тех элементов, у которых ```expirationDate``` больше сегодняшней даты. 
Файл index.html редактировать не нужно.

- - - - - -

### 3. Framework
Необходимые материалы в папке [Level3_Framework](https://github.com/DmitryIvanov92/formula-fe-test/tree/master/Level3_Framework).

Нужно используя верстку, полученную в первом пункте собрать SPA. Использовать React.  
Должно быть две страницы - Home(на макете) и Contact (переход при нажатии на [ссылку 1](https://github.com/DmitryIvanov92/formula-fe-test/blob/master/Level3_Framework/resources/homepage.jpg)).  
На странице Home блоки с описанием и изображением хот-догов ([область 2](https://github.com/DmitryIvanov92/formula-fe-test/blob/master/Level3_Framework/resources/homepage.jpg)) должны загружаться GET-запросом на URL https://formula-test-api.herokuapp.com/menu .

Формат:

```
{
  id: 1,
  name: 'Name', 
  description: 'Description', 
  expirationDate: '01-30-1999',
  backgroundURL: 'https://..../image.jpg'
}
```
Полученный с сервера ответ необходимо отфильтровать по ```expirationDate``` функцией, полученной в **Level2_Javascript**, и отрисовать их на странице Home.

На странице Contact должны быть два ```input``` "Name" и "Email",  ```textarea``` "Comment" и кнопка, при клике на которую данные формы отправляются на сервер. Дизайн на усмотрение разработчика.
Данные отправлять POST-запросом на URL https://formula-test-api.herokuapp.com/contact в json-формате:
```
{
  "name": "name",
  "email": "email",
  "comment": "comment",
}
```
