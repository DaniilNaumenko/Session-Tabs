## Введение

Содержание данного документа описывает план тестирования разрабатываемого приложения. Более подробную информацию о приложении можно найти в документе [SRS.md](https://github.com/pobozhnaya18/Session-Tabs/blob/master/Documents/Требования%20к%20проекту.md#system_requirements)
Тестировщику необходимо уметь пользоваться персональным компьютером.
Цель тестирования: проверить работоспособность функционала, заявленного в требованиях, и всего приложения.

## Объекты тестирования

В качестве объектов тестирования можно выделить атрибуты качества платформы по ISO 25010:

1) функциональность
   + функциональная полнота: приложение должно выполнять все заявленные функции
   + функциональная корректность: приложение должно выполнять все заявленные функции корректно
   + функциональная целесообразность: отсутствуют не заявленные функции, которые бы мешали приложению выполнять первоначально поставленные задачи
2) удобство использования
   + эстетика пользовательского интерфейса: элементы управления объектами должны быть всегда доступны пользователю
   + защищённость от ошибки пользователя
   
Данные атрибуты были взяты с учётом специфики приложения.

## Риски

При подключенном интернете осуществляется возможность отображения сессии всех открытых вкладок. Соответсятвенно, работа приложения напрямую зависит от доступа к интернету.

## Аспекты тестирования

В ходе тестирования планируется проверить реализацию основных функций приложения, провести позитивные и негативные тесты, а также проверить нефункциональные требования.
Дымное тестирование будет проводиться по тестам, без доступа к исходному коду по типу "чёрного ящика". Данное тестирование будет проверять всю самую важную функциональность.
К основным функциям можно отнести следующие пункты:
* возможность отображать сессии всех открытых вкладок;
* возможность поиска в окрытых вкладках;
* возможность сохранять вкладки в сессию;
* возможность удалять вкладки из сессии сохраненных;
* возможность восстановления одной или всех сохраненных вкладок из сессии.

### Возможность отображать сессии всех открытых вкладок
Этот вариант использования небходимо протестировать на:
* Корректность вывода всех открытых вкладок;

### Возможность поиска в окрытых вкладках
Этот вариант использования небходимо протестировать на:
* Поиск вкладки, которая существует в сессии;
* Поиск вкладки, которая не существует в сессии;

### Возможность сохранять вкладки в сессию
Этот вариант использования небходимо протестировать на:
* Правильность сохранения вкладок в сессию;

### Возможность удалять вкладки из сессии сохраненных
Этот вариант использования небходимо протестировать на:
* Удаление существующей вкладки;

### Возможность восстановления одной или всех сохраненных вкладок из сессии
Этот вариант использования небходимо протестировать на:
* Восстановление одной/всех вкладок после изменения сессии;
* Восстановление одной/всех вкладок когда небыло сделано изменений в сессии;

### Нефункциональные требования:
* Надежность системы при перезагрузке и сбоям в браузере;
* Приложение должно соответствовать заданному размеру;
* Способность запуска на любом устройстве, при наличии Google Chrome.

##  Подходы к тестированию

Для тестирования приложения необходимо вручную проверить каждый вариант использования.

## Представление результатов

Результаты тестирования представлены в документе ["Представление результатов"](https://github.com/DaniilNaumenko/Session-Tabs/blob/patch-1/Testing/TestResults.md)

## Вывод

Данный тестовый план позволяет протестировать основной функционал приложения. Успешное прохождение всех тестов позволяет полагать, что данное приложение работает корректно.