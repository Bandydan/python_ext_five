# 09. Основы работы WEB

## HTML

Основой страницы типичного сайта является определенным образом отформатированный текст. Текст этот структурирован и может быть снабжен ссылками на части этой же страницы и на другие страницы, как этого сайта, так и любых других сайтов. Этот текст отформатирован и структурирован (или одним словом - размечен) при помощи языка **HTML (HyperText Markup Language) — языка разметки гипертекста.**

**Гипертекстом** называется текст, который может содержать гиперссылки, т.е. обычные ссылки.

**HTML** совсем не обязательно хранится в каком-то файле. Достаточно часто **HTML** полностью или частично генерируется при помощи других языков программирования или каких-то программ. В частности, эта страница в **HTML** преобразована специальной программой из файла формата **.md**.

Важно понимать и помнить, что **HTML** не является языком программирования, это язык разметки текста.

![](https://otvet.imgsmail.ru/download/9783312_d702027446bb40cedf5681913e926517_800.jpg)


## Структура HTML документа

Современного вида HTML документ состоит из нескольких основных элементов, представленных на рисунке ниже:

![HTML document structure](https://www.oreilly.com/library/view/learning-web-design/9781449337513/httpatomoreillycomsourceoreillyimages2257981.png)

На представленном выше рисунке представленна стандартная и очень упрощенная структура HTML документа. По пунктам там:

1. Объявление типа документа. Не является стандартным HTML тэгом, но является важнейшим элементом HTML документа. В приведеном выше случае указывает на то, что формат документа соответсвует стандарту HTML5. [доп. информация](http://htmlbook.ru/html/!doctype)
2. Парный тэг **`<html>`. `<html>`** тэг включает в себя весь документ HTML и является корневым элементом документа.
3. Парный тэг **`<head>`** (заголовок). В этом тэге находится вся общая информация о документе, подключение стилей, скриптов, указываются все мета-данные документа.
4. Одиночный тэг **`<meta>`** содержит мета-данные об текущем HTML документе. В данном случае тэг устанавливает систему кодирования символов в utf8. Есть огромное количество метаданных, которые могут быть установлены этим тегом. Для начала можно ознакомиться с перечнем и примерами на [википедии.](https://ru.wikipedia.org/wiki/%D0%9C%D0%B5%D1%82%D0%B0%D1%82%D0%B5%D0%B3%D0%B8)
5. Обязательный элемент заголовка (head) HTML документа - парный тег **`<title>`**, содержащий внутри себя описание страницы. Содержимое title отображается в названии вкладки страницы в браузере.
6. Тэг **`<body>`** содержит весь контент страницы, который необходимо показывать в окне браузера.

## Тэги HTML

![HTML tag structure](https://www.oreilly.com/library/view/learning-web-design/9781449337513/httpatomoreillycomsourceoreillyimages2257991.png)

Как уже может быть понятно из предидущего раздела, есть теги парные и одиночные(непарные). Парные теги начинаются названием тега, содержимое их находится между тегами открывающим и закрывающим, а закрывается, соответственно, названием тега, предваренным слешом. Одинарные теги содержат всю информацию в открывающей части тега и не имеют внутренней информации.

[Краткая инфа о тегах](https://html5book.ru/html-tags/)

[Таблица тегов](https://html5book.ru/examples/html-tags.html)

## Основы и суть CSS

**CSS - Cascading Style Sheets**, каскадная таблица стилей. **HTML** служит для вывода информации пользователю, тогда как **CSS** служит для оформления и стилизации выведенного при помощи **HTML** текста, картинок и других элементов.

**CSS** состоит из множества селекторов с правилами, как **HTML** состоит из тегов с аттрибутами. Каждое правило устанавливает минимум одно свойство для минимум одного элемента. Каждый селектор выбирает определенный тег или теги на странице и пытается применять к ним свои правила. Успех этого мероприятия зависит от приоритета селектора и порядка его появления.

![css selector](http://www.iraqtimeline.com/maxdesign/basicdesign/images/css_selector_declaration.png)

Для того, чтобы уметь читать CSS, нужно понимать три вещи: селекторы, свойства и порядок их использования. Чтобы уметь верстать, к сожалению, этих знаний недостаточно. Необходимо также накопить немало опыта в изучении взаимодействий различных селекторов, понимать теорию потоков, в которые попадают блоки, осваивать пре и постпроцессоры и многое многое другое. На этом уроке наша задача - уметь читать и слегка изменять существующие селекторы и свойства.

[Селекторы](https://webref.ru/css#selectors)

[Обучение по селекторам](https://learn.javascript.ru/css-selectors)

[CSS свойства](https://puzzleweb.ru/css/all_properties.php)

## Bootstrap

Иногда перед backend программистами все же возникают задачи некоторой минимальной стилизации выводимой информации. На помощь начинающим "верстальщикам" может прийти CSS фреймворк Bootstrap.

![bootstrap](https://pics.me.me/bootstrap-html-css-31715884.png)


### Grid - сетка и прочие радости

Первый важный момент, который следует иметь в виду при принятии решения, использовать ли bootstrap - возможность использовать сетку для размещения элементов.

[grid](https://getbootstrap.com/docs/4.3/layout/grid/)

В обычной ситуации элементы на веб-странице размещаются при помощи CSS несколькими вариантами - абсолютным или относительным позиционированием, в потоке и вне потока, и различными комбинациями этих вариантов. Помимо этих подходов есть подход через flexbox и через сетки. Сетка bootstrap - самая популярная из сеток.

Также рекомендуем рассмотреть все пункты меню и попробовать как можно большее количество элементов и компонентов.

### Client-server, HTTP, REST, Формы

Самый распространенный способ реализации взаимодействия пользователя интернет-сервиса с этим сервисом и его возможностями - архитектура клиент-сервер.

Суть архитектуры довольно проста: пользователь отправляет запросы с клиентского интерфейса на сервер и получает с сервера на клиентский интерфейс ответы на свои запросы.

![](https://www.orosk.com/wp-content/uploads/2016/07/Client-Server-Network-1.jpg)

Запросы (Requests) и ответы (Responses), как правило, отправляются при помощи протокола передачи гипертекста (HTTP). Когда вы кликаете на ссылку на странице, заполняете форму или запускаете поиск, браузер отправляет на сервер HTTP-запрос.

Этот запрос обязательно включает:

- Путь к серверу и/или ресурсу на сервере
- Метод протокола, определяющий необходимое действие (например, получить файл, сохранить или обновить некоторые данные, и т.д.).Самые популярные методы - 
**GET**, для получения ресурса, и **POST** для создания или нового ресурса.
- прочая информация, например:


![](https://www.yuripetrov.ru/edu/python/_images/13_01_10.png)

## IP address, DNS query, HTTP Status Codes


**IP-адрес** (Internet Protocol Address) – это уникальный сетевой идентификатор, присваивающийся каждому участнику локальной или глобальной компьютерной сети.
До недавнего времени человечество использовало один общепринятый формат записи IP-адреса – 32-битный IPv4, например 192.180.0.255. Шестая версия интернет-протокола представляет собой 128-битную запись, состоящую из 8 буквенно-цифровых блоков, разделенных двоеточиями (2001:0db8:85a3:0000:0000:8a2e:0370:7334).

### DNS

Основная концепция преобразования DNS названий достаточно проста. Каждому веб сайту присваивается уникальный IP адрес. Для доступа к веб сайту клиенту необходимо знать этот IP адрес сайта. Для простоты человеческого восприятия в игру вступают домены. Для доступа к запрашиваемому веб сайту браузер (Web browser) должен уметь преобразовывать название домена сайта (domain name) в соответствующий ему IP адрес (IP адрес устанавливается при помощи А записи).

Находим все о доменах и их владельца при помощи комманды **whois domain.com**.

Для того чтоб узнать IP адрес сервера, на котором хостится сайт, используем следующие комманды в терминале:

**host domain.com** 
**dig a domain.com**

Узнаем все хост записи для домена (SOA, TXT, A, CNAME и другие):

**dig any domain.com**

Чтоб проверить живой ли IP адрес, используем коммаду **ping IP**. 

[Подробно о DNS и хост записях](https://eternalhost.net/base/web-hosting/tipy-dns-zapisey)

### HTTP statuses

**HTTP statuses** - часть первой строки ответа сервера при запросах по протоколу HTTP (от 100 до 500). Самые популярные:

**200** - OK («хорошо»)
**302** -  Moved Temporarily («перемещено временно»)
**404** -  Not Found («не найдено»)
**500** -  Internal Server Error («внутренняя ошибка сервера»)

Проверить статус можно командой **wget domain.com +trace**.

![](https://httpstatusdogs.com/img/201.jpg)

[Собаки и HTTP](https://httpstatusdogs.com)


### Практика: создание стандартной формы без bootstrap и с bootstrap с выводом данных на экран.

[REST и споры о нем](https://dou.ua/lenta/articles/rest-conception/)


[Формы на bootstrap](https://getbootstrap.com/docs/4.3/components/forms/)
