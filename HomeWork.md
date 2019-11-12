# 1. Выбор темы
Сервис знакомство (Тиндер)

# 2. Определение возможного диапазона нагрузок подобного проекта

# 3. Выбор планируемой нагрузки 

# 4. Логическая схема базы данных (без выбора СУБД)

- Users
	- ID
	- name 
	- birthday
	- bio
	- university
	- city
	- description
	- accountId
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

- Session
	- ID
	- userId
	- session

- Messages 
	- ID
	- userFromID
	- userToId
	- message


# 5. Физическая системы хранения (конкретные СУБД, шардинг, расчет нагрузки, обоснование реализуемости на основе результатов нагрузочного тестирования)



