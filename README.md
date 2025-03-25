
Общая логика

Приложение написано по многослойной архитектуре, где каждый слой выполняет свою роль:

-Handlers – принимают HTTP-запросы, валидируют данные и передают данные дальше в Services. Они не должны содержать сложной логики, так как их задача - передать работу бизнес-логике и репозиториям.

-Services – обрабатывают данные и выполняют бизнес-операции. Являются ядром приложения, где происходит основная работа. Используют репозитории для обработки данных.

-Repositories – взаимодействуют с базой данных, извлекая, добавляя и изменяя данные.

Использован:
- Postman для отправки и получения запросов
- DataGrip для работы и отслеживания БД

Добавлено: 
- удаление пользователя и всех его задач
- проверка на user_id (NOT NULL в запросе SQL добавил)
- получение всех задач по username

** Под каждую ошибку выведено свое уникальное сообщение в LOG 

# practica2otNedeli3
# practica2otNedeli3
