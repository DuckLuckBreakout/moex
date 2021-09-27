# Московская биржа

## 1. Тема и целевая аудитория

### 1.1 Тема

[Московская биржа](https://www.moex.com/)
является организатором торгов акциями, облигациями, производными инструментами, валютой, инструментами денежного рынка, драгоценными металлами, зерном и сахаром.
### 1.2 MVP
- Размещение запросов на покупку/продажу акций;
- Просмотр истории изменения курса;
- Просмотр текущего курса;
- Просмотр истории сделок;
- Просмотр портфеля;
- Просмотр биржевого стакана.


### 1.3 Целевая аудитория


#### 1.3.1 Общие данные



По [данным на август 2021 года](https://www.moex.com/s719) Московская биржа имеет следующее число зарегистрированных клиентов в Системе торгов:

Тип клиента | Число|
------------- | -------------:
Физические лица	|22 591 697|	
Юридические лица	|28 709|		
Иностранные лица		|27 297|	
Иностранные физические лица 	|21 434|		
Иностранные юридические лица 		|5 863|	
Клиенты, передавшие свои средства в ДУ	|195 761|		
Всего		|22 843 464|	


По [данным на август 2021 года](https://www.moex.com/s719) Московская биржа имеет следующее число уникальных клиентов в Системе торгов:

Тип клиента | Число|
------------- | -------------:
Физические лица	|13 773 190|	
Юридические лица	|19 995|		
Иностранные лица		|20 283|	
Иностранные физические лица 	|17 471|		
Иностранные юридические лица 		|2 812|	
Клиенты, передавшие свои средства в ДУ	|122 307|		
Всего		|13 935 775|	


По [данным на август 2021 года](https://www.moex.com/s719) Московская биржа имеет следующее число активных клиентов в Системе торгов (совершивших в течение месяца хотя бы одну сделку):

Тип клиента | Число|
------------- | -------------:
Физические лица	|2 094 638|	
Юридические лица	|1 456|		
Иностранные лица		|3 097|	
Иностранные физические лица 	|2 876|		
Иностранные юридические лица 		|221|	
Клиенты, передавшие свои средства в ДУ	|40 871|		
Всего		|2 140 062|	

__98% клиентов в Системе торгов - физические лица__


#### 1.3.2 Возрастные группы

Исходя из  [исследования](https://www.tinkoff.ru/about/news/04032021-tinkoff-investments-russsian-investors-portrait-2020/) Тинькофф Инвестиций за 2020 год:

Возрастная группа | Процент |
------------- | -------------:
18-28 лет	|27%|	
28-38 лет	|43%|		
38-48 лет	|21%|		
48+ лет	|9%|		

__70% клиентов-физических лиц в Системе торгов находятся в возрасте от 18 до 38 лет__

## 2. Расчёт нагрузки

### 2.1 Продуктовые метрики


#### 2.1.1 Дневная аудитория

На [август 2021 года](https://www.moex.com/ru/spot/members-rating.aspx?rid=111) АО "Тинькофф Банк" занимает первое место по числу клиентов Московской биржи с числом клиентов равным `6 535 540` человек. Это  `6 535 540 / 22 591 697 = 29%` от числа зарегистрированных физических лиц из России.

На момент [регистрации 1млн счетов](https://www.tinkoff.ru/about/news/24092019-tinkoff-investments-opened-1-million-accounts/), ежедневно Тинькофф Инвестициями пользовались до `80 000` человек.

Предположим, что на данный момент число ежедневных пользователей "Тинькофф Инвестиции" увеличилось пропорционально увеличению общего числа зарегистрированных клиентов. Тогда на данный момент ежедневно "Тинькофф Инвестиции" используют `6.535540 * 80 000 = 522 843` пользователя. Тинькофф предоставляет интерфейс для взаимодействия с биржей `29%` всех клиентов Московской биржи, тогда можно предположить, что `522 843` это `29%` от ежедневного числа клиентов Московской биржи. Тогда ежедневное число пользователей Московской биржи: `522 843 / 0.29 = 1 802 906` человек.


#### 2.1.2 Месячная аудитория

По [данным на август 2021 года](https://www.moex.com/s719)  Московской биржей за месяц пользовалось `13 790 661` уникальных физических лица.


#### 2.1.3 Среднее количество действий пользователя по типам в день

Для примерного подсчета средней продолжительности сессии воспользуемся [данными](https://www.similarweb.com/ru/website/binance.com/#overview) о средней сессии на бирже Binance.
Средняя продолжительность сессии: `00:09:17`

Действие | Количество |
------------- | -------------:
Размещение запросов на покупку/продажу акций	| [0.64](https://www.tinkoff.ru/about/news/04032021-tinkoff-investments-russsian-investors-portrait-2020/)|	
Просмотр текущего курса	|1080|		
Просмотр истории изменения курса	|25|		
Просмотр истории сделок |25|
Просмотр портфеля |2|
Просмотр биржевого стакана |25|

### 2.2 Технические метрики

### 2.2.1 Хранение данных

Основные типы данных - временные ряды
По данным на апрель 2020 год число компаний, акции которых торгуются на Московской бирже равно 630.

История курса акций на Московской бирже хранится от 2004 года. Предположим что данные о курсе хранятся с интервалом в 0.5 секунды, и что все компании присутствовали на бирже с самого начала. Тогда для каждой компании необходимо хранить `60 * 60 * 2 * 9 * 365 * 17 = 402 084 000` данных о курсе на каждый период времени.

Допустим, хранится только время и курс относительно какой-то условной валюты, тогда для каждой секунды хранится:

- Время - int - 4 байта;
- Курс - double - 8 байт.

Итого 12 байт на каждую запись.

Всего на историю курса одной акции: `402 084 000 * 12 = 4 825 008 000 Байт = 4.49Гб`

Всего на историю курса всех акций: `402 084 000 * 12 * 630 = 2835 Гб = 2.77 Тб`

### 2.2.2 Сетевой трафик

Основной тип трафика - запрос текущего курса.

Ответ на запрос курса на бирже Yobit занимает примерно 208 Байт.
![img](https://user-images.githubusercontent.com/49189299/134879239-f81bbaa0-aaba-417f-9c92-0d89207ef834.png)


Тогда один пользователь в день получает ответов с текущим курсом на
`208 * 1080 = 224 640 Байт`

В день биржей пользуется около `1 802 906` человек, следовательно суммарно на запрос курса отправляется около `405 004 803 840 Байт = 377.19 Гб`

Торговая сессия длится `9 часов = 32 400 сек`, следовательно в секунду трафик запросов на текущий курс: `377.19 Гб / 32 400 сек = 0.011 Гб/сек = 11.9 Мб/сек`


### 2.2.3 RPS в разбивке по типам запросов (запросов в секунду) 
Один пользователь в день совершает в среднем `1 157.64` действий.

Следовательно в день суммарно `1 157.64 * 1 802 906 = 2 087 116 101.84` действий.

Торговая сессия длится `32 400` секунд, следовательно `RPS = 2 087 116 101.84 / 32 400 = 64417.16`

Действие | RPS | Тип |
------------- | -------------:| -------------:
Размещение запросов на покупку/продажу акций	| 35.61 |	запись
Просмотр текущего курса	|60 253 |	чтение
Просмотр истории изменения курса	|1 288.34| чтение		
Просмотр истории сделок |1 288.34| чтение
Просмотр портфеля |103.07| чтение
Просмотр биржевого стакана |1 288.34| чтение

