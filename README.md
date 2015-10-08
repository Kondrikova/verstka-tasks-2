# Задача к лекции «HTML, II часть» – «Бабуленькин сервант»

:sos: [Как создать Pull Request](https://github.com/urfu-2015/guides/blob/master/how-to-pull-request.md)  
:warning: При создании PullRequest'а не забудьте указать ваши имя и фамилию.

### Общие требования

Мы очень хотим, чтобы код вы написали сами, а не пользовались внешними библиотеками.

Прежде чем отправлять решение проверьте его на соответствие [общим требованиям](https://github.com/urfu-2015/guides/blob/master/html-codestyle.md).

Когда вы создадите или обновите пулл-реквест – он частично будет проверен
автоматически. Результаты вы увидите внизу:

Если всё плохо:  
<img width="308" alt="2015-10-08_1845" src="https://cloud.githubusercontent.com/assets/4534405/10368030/ccc43228-6dec-11e5-925e-47793862d13e.png">

Если всё хорошо:  
<img width="218" alt="2015-10-08_1841" src="https://cloud.githubusercontent.com/assets/4534405/10367916/60487fc8-6dec-11e5-9e1d-2a1b15da2220.png">


Проверить HTML можно и вручную на соответствие вручную требованиям можно так:
```sh
# Устанавливаем проверяльщик
npm install

# Проверяем
npm test

# В результате выведутся ошибки, если они есть.
# Если какие-либо ошибки будут не понятны – смело спрашиваем у ментора.
```

В помощь вам, мы разместили файл `.editorconfig`. Этот файл содержит базовые
правила оформления кода (codestyle), понятные для большинства редакторов.
Прочитайте [о нём подробнее](https://github.com/urfu-2015/guides/blob/master/editorconfig.md).

### Задача

У моей бабуленьки есть старый сервант, где она хранит старые книги и видеокасеты
с фильмами. Она бы хотела разместить информацию о них в «этих ваших интернетах»,
чтобы обмениваться с бабуленьками других внучков.

Итак, у нас есть информация в виде текста о текущих книгах и фильмах. Вам необходимо:
- разметить его **без использования CSS**;
- дополнить книгу красивой обложкой, а автора – фотографией;
- фильмы дополнить трейлерами;
- внизу обязательно разместить удобную форму для добавления новых книг и фильмов;
- * возможно, к книгам вы захотите разместить аудио-версию, а к фильмам субтитры.
- * по некоторым книгам могут быть сняты фильмы ;)

Собственно, текст (тщательно записанный со слов бабуленьки):

```text

- Война и мир.

    Тип: Книга
    Издательство: АСТ, Астрель
    ISBN: 5-17-006400-4,978-5-17-006400-7
    Год: 1867 г
    Тип издания: Авторский сборник
    Язык: Русский
    Страниц: 704 стр.
    Формат: ePub
    Переплет: Твердый переплет
    Дата размещения: 8 котобря 2015
    Жанр: Русская классика, Литература 19 века
    URL: http://babulenkin-servant.com/books/war_and_peace.epub
    Описание: Великий роман-эпопея Льва Толстого чудесным образом, как огромная
    мозаика, сложен из тысяч картин - батальных, бальных, любовных, бытовых,
    политических, философских, портретных, пейзажных, психологических...

        Автор: Лев Николаевич Толстой
        Дата рождения: 16 августа 1828
        Дата смерти: 7 ноября 1910
        Место рождения:	Ясная Поляна, Тульская губерния, Российская империя
        Род деятельности: прозаик, публицист, философ

- Harry Potter and the Sorcerer's Stone

    Тип: Книга
    Издательство: АСТ, Астрель
    ISBN: 978-0439708180
    Год: 1998 г
    Язык: English
    Страниц: 309 стр.
    Формат: pdf
    Переплет: Мягкий переплет
    Дата размещения: 4 котобря 2015
    Жанр: Fantasy, Adventure, Kids & Family
    URL: http://babulenkin-servant.com/books/potter.pdf
    Описание: Harry Potter has no idea how famous he is. That's because he's
    being raised by his miserable aunt and uncle who are terrified Harry will
    learn that he's really a wizard, just as his parents were.

        Автор: J. K. Rowling
        Дата рождения: 31 июля 1965
        Дата смерти: –
        Место рождения:	Глостершир, Англия
        Род деятельности: прозаик
        URL: jkrowling.com
        Адрес: 50 Bedford Square, London
        Email: info@jkrowlingpr.com

- Titanic

    Тип: Фильм
    Год: 1997
    Страна: США
    Слоган: «Ничто на Земле не сможет разлучить их»
    Режиссер: Джеймс Кэмерон
    Сценарий: Джеймс Кэмерон
    Продюсер: Джеймс Кэмерон, Джон Ландау, Памела Исли
    Оператор: Рассел Карпентер
    Композитор: Джеймс Хорнер
    Художник: Питер Ламонт, Мартин Лэйн, Чарльз Дуайт Ли
    Монтаж: Конрад Бафф IV, Джеймс Кэмерон, Ричард А. Харрис
    Жанр: драма, мелодрама
    Дата размещения: 1 котобря 2015
    URL: http://babulenkin-servant.com/films/titanic.mp4
    Описание: Молодые влюбленные Джек и Роза находят друг друга в первом и
    последнем плавании «непотопляемого» Титаника. Они не могли знать, что
    шикарный лайнер столкнется с айсбергом в холодных водах Северной Атлантики,
    и их страстная любовь превратится в схватку со смертью.

        Автор: Джеймс Кэмерон
        Дата рождения: 16 августа 1954
        Дата смерти: –
        Место рождения: Капускасинг, Онтарио, Канада
        Род деятельности: продюсер, режиссер, сценарист, актер


А ЗДЕСЬ ФОРМА ДОБАВЛЕНИЯ НОВЫХ КНИГ И ФИЛЬМОВ
```
