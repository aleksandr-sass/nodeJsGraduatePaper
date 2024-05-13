# Node JS Graduate Paper
## JS by MDA
### 2024Q2

### Задачи
1. Определиться со структурой будущей базы данных+
2. Найти самую простую в освоении СУБД, которую можно будет "подружить" с NodeJS-сервером (beta)
3. Освоиться с PostgreSQL
4. Попробовать написать свой простой сервер на NodeJS
5.
6.
7.
8.
9.
10.

### Решение
1. **Cтруктура БД**
Я ожидаю, что мне понадобится база данных со следующими полями: поле (ожидаемый формат данных)
  * id (int/number)
  * datetime (datetime: YYYY/MM/DD @HH:MM)
  * courseName (string) // I will get it from that page, that user will see
  * tel (string: +37529 XXX XX XX)
  * Comment (string with length about 500 chars)
  * Processed (обработан): Boolean
2. **Выбор СУБД**
Пока что есть два реальных варианта:
  * Sqlite (через модуль Sqlite3)
  * PostgreSQL.
Sqlite прост, но, всё-таки он работает по принципу: многие читают - один пишет.
В моём проекте же всё в точности наоборот: многие (клиенты) пишут, а только один (админ) - читает.

Да, PostgreSQL будет сложнее в освоении. Но также важно понимать тот факт, что знание PostgreSQL куда проще "монетизировать".

Также есть как минимум один пример использования PostgreSQL в связке с NodeJS:

https://medium.com/devschacht/node-hero-chapter-5-dd79607858f2#:~:text=%C2%ABNode.,%D0%BF%D0%BE%D0%BF%D1%83%D0%BB%D1%8F%D1%80%D0%BD%D0%B0%D1%8F%20NoSQL%20%D0%B1%D0%B0%D0%B7%D0%B0%20%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)%C2%BB.

Таким образом, в качестве промежуточного варианта СУБД я выбираю PostgreSQL.


3.
4.
5.
6.
7.
8.
9.
10.

### Ожидаемый конечный результат
* Front-end -> Back-end <- Admin's page
* Database & easy access to it
* Admin can add service info to user's comment

### Minimum Viable Product
* Есть сайт, на котором можно оставить свой номер телефона - и на следующий день тебя запишут на курсы.