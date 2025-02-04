# Определение выгодного тарифа для телеком компании


## Данные

- Таблица users — информация о пользователях:
- - user_id — уникальный идентификатор пользователя
- - first_name — имя пользователя
- - last_name — фамилия пользователя
- - age — возраст пользователя (годы)
reg_date — дата подключения тарифа (день, месяц, год)
- - churn_date — дата прекращения пользования тарифом (если значение пропущено, значит, тариф ещё действовал на момент выгрузки данных)
- - city — город проживания пользователя
- - tarif — название тарифного плана
- Таблица calls — информация о звонках:
- - id — уникальный номер звонка
- - call_date — дата звонка
- - duration — длительность звонка в минутах
- - user_id — идентификатор пользователя, сделавшего звонок
- Таблица messages — информация о сообщениях:
- - id — уникальный номер звонка
- - message_date — дата сообщения
- - user_id — идентификатор пользователя, отправившего сообщение
- Таблица internet — информация об интернет-сессиях:
- - id — уникальный номер сессии
- - mb_used — объём потраченного за сессию интернет-трафика (в мегабайтах)
- - session_date — дата интернет-сессии
- - user_id — идентификатор пользователя
- Таблица tariffs — информация о тарифах:
- - tariff_name — название тарифа
- - rub_monthly_fee — ежемесячная абонентская плата в рублях
- - minutes_included — количество минут разговора в месяц, включённых в абонентскую плату
- - messages_included — количество сообщений в месяц, включённых в абонентскую плату
- - mb_per_month_included — объём интернет-трафика, включённого в абонентскую плату (в мегабайтах)
- - rub_per_minute — стоимость минуты разговора сверх тарифного пакета (например, если в тарифе 100 минут разговора в месяц, то со 101 минуты будет взиматься плата)
- - rub_per_message — стоимость отправки сообщения сверх тарифного пакета
- - rub_per_gb — стоимость дополнительного гигабайта интернет-трафика сверх тарифного пакета (1 гигабайт = 1024 мегабайта)

## Задача

На основе данных клиентов оператора сотовой связи проанализировать поведение клиентов и поиск оптимального тарифа  

## Используемые библиотеки

*Matplotlib*, *NumPy*, *SciPy*, *описательная статистика*