Отчет по 4 работе «Уязвимости OWSAP»

1.1Повторить тестирование по материалу

![](file:///C:/Users/Future/AppData/Local/Temp/msohtmlclip1/01/clip_image001.png)

![](file:///C:/Users/Future/AppData/Local/Temp/msohtmlclip1/01/clip_image003.png)

Данные успешно получены

1.2 Проверить наличие уязвимости Хранимая HTML инъекция в своем приложении![](file:///C:/Users/Future/AppData/Local/Temp/msohtmlclip1/01/clip_image004.png)

HTML – инъекция не прошла, так как защиту дает шаблонизатор jinja

1.3 Основные методы защиты

               1 -Экранирование (кодирование) вывода на стороне сервера. Автоматическое преобразование управляющих символов HTML в безопасные HTML-сущности.

               2. Валидация входящих данных и контекстное кодирование. Проверка всех поступающих от пользователя данных на соответствие строгому типу и применение специфического экранирования при передаче данных внутрь JavaScript.

1.4 Исправление сайта

Исправление сайта не требуется, так как защиту уже дает jinja

2.1 Самостоятельно протестировать HTML Reflected (Get) уровень Low (в приложении bWapp):

Инструкция для поверки Уязвимость HTMl Injection — Reflected (GET) уровень (Medium).

![](file:///C:/Users/Future/AppData/Local/Temp/msohtmlclip1/01/clip_image006.png)

![](file:///C:/Users/Future/AppData/Local/Temp/msohtmlclip1/01/clip_image008.png)

![](file:///C:/Users/Future/AppData/Local/Temp/msohtmlclip1/01/clip_image010.jpg)

Следуя инструкции мы отобразили ссылку на сайте.

Инструкция для проверки уязвимости HTML Injection — Reflected (POST) уровень (Low).

![](file:///C:/Users/Future/AppData/Local/Temp/msohtmlclip1/01/clip_image011.png)

Данные полученные перехватом запроса POST

![](file:///C:/Users/Future/AppData/Local/Temp/msohtmlclip1/01/clip_image013.png)

В итоге мы успешно проэксплуатировали данную уязвимость и вывели кликабельную ссылку, с использованием тега «**a**», и масштабирования текста, тега «**h1**» и «**h2**».