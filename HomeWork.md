## 1. Выбор темы
Tinder - location-based social search

## 2. Определение возможного диапазона нагрузок подобного проекта

- 57 миллион пользователей
- 4.1 миллион Tinder Plus and Tinder Gold
- 30+ миллиард матчей c момента начало проекта (2012)
- 2 миллион просмотров каждый день 
- 1.6 миллион матчей каждый день
- 34 минут - средное время который пользователи тратят в день
- 7,5 млн. Свайпов в день в Индии (2016), где Tinder открыл свой первый международный офис

## 3. Выбор планируемой нагрузки 

## 4. Логическая схема базы данных (без выбора СУБД)

- Users
	- ID
	- name 
	- birthday
	- bio
	- university
	- city
	- description
	- accountID
	- interestedOn 
		- men
		- women
	- ageRange
	- maxDistance
	- isActive

- Account 
	- ID 
	- email
	- phone 
	- password
	- lastSignIn

- Likes 
	- ID
	- userFromID
	- userToID
	- like 
		- like (1)
		- dislike (-1) 

- Session
	- ID
	- userId
	- session

- Messages 
	- ID
	- userFromID
	- userToID
	- message


## 5. Физическая системы хранения 
### (конкретные СУБД, шардинг, расчет нагрузки, обоснование реализуемости на основе результатов нагрузочного тестирования)

- Для хранения общей информации PostgreSQL
- Для хранения информации о геоданных пользователей PostgreSQL с PostGis
- Для сессий Redis

### Links

[50 Interesting tinder Statistics and Facts (December 2018)](https://expandedramblings.com/index.php/tinder-statistics/amp/)


