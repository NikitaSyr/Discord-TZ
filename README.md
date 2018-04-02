# Техническое задание Discord

1. Общие положения

«Необходимо создать приложение для разработчика Hammer & Chisel.
Приложение должно быть бесплатным, поддерживать VoIP и видеоконфиренции,
реализованно для Windows, macOS и Linux, а так же иметь мобильные версии для Android и iOS, веб-клиент. »

2. Эксплуатационные назначения

«Привлечение большого числа пользователей, предостовляя им возможность платной подписки»

3. Функциональное назначение

«Приложение должно содержать возможность создания и входа на различные серверы, 
в которых должна быть возможность создавать голосовые и текстовые каналы.

Платные подписки открывают новые функции для пользователя (Gif аватарка, 
возможность использования пользовательских смайлов на всех серверах, увеличение размера загружаемого файла (с 8мб до 50мб))»

4. Требования к хостингу

• JavaScript, Elixir

• Интерфейс HTML

5. Наполнение приложения

«Исполнитель обязуется выполнить минимальное наполнение приложения, которое позволит начать эксплуатацию приложения пользователями.
Испольнитель должен создать интерфейсы описанные в настоящем ТЗ. В обязанности исполнителя не входит создание серверов и каналов»

6. Требования к надёжности 

«Приложение должно обладать защитой от DDoS-атак»

7. Условия сдачи и приемки

Приложение должно корректно отображаться и функционировать в следующих ОС:

• Windows 7 и выше 

• macOS

• Linux

Мобильных платформах:

• Android

• iOS 

браузерах:

• Chrome 13

• FireFox 4

• Safari 5

• Opera 11

8. Страницы и переходы:

Discord-TZ/Карта.png

9. Функциональные характеристики

«При запуске приложения пользователь должен иметь возможность выбрать сервер, на который уже осуществлён вход,
возможность создать собственный сервер и каналы в нём, возможность входа на сервер по приглашению, а так же 
возможность использования личных звонков и сообщений»

10. Анализ сущностей

• Серверы

• Каналы на серверах

• Типы каналов (голосовой, текстовый)

• Платная подписка

• Список друзей

• Личные сообщения и звонки

11. Данные. Пример: Сервер

| Название        | Тип                 | Валидатор  | Описание    |
| ------------- |:------------------:| -----:| -----:|
| Название сервера      | Строка    | Обязательное  |   |
| Каналы      | Канал  |   | Список каналов, находящихся на сервере |
| Порядок следования   | Целое         |    Обязательное |   Число, определяющее порядок следования элементов|
