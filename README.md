# GTD

Читаем 

https://developers.google.com/calendar/quickstart/python?hl=ru

получаем credentials.json, кладем в папку src. 

Уснановить:

`pip install --upgrade google-api-python-client google-auth-httplib2 google-auth-oauthlib`

Новая задача попадает в Input.md. 
Разбирая корзину, для каждого эвента последовательно отвечая на вопросы:
1. С этим нужно что-то делать?
2. Делать мне?
3. Сейчас делать?
4. Одношаговое или проект?

Евенты попатают в те или иные списки, которые в конечном итоге должны все попасть в Done.md

Скрипты add заполняют лист To_do.md и Shopping_list.md с проектов где есть пункты без дат:

- [ ] ...
- [ ] Купить ...

Если у аункта есть дата `01.01.2021`, то создается событие в гугл календаре.

Скрипт delete удаляет из списокв и календаря выполненные события 
- [x] ...

и помещает их в Done.md  