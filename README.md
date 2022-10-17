# Avito
Авито — сервис объявлений, который объединяет продавцов и покупателей. На Авито вы можете недорого купить или выгодно продать авто с пробегом или новую машину, квартиру и другую недвижимость, а также новую или б/у одежду и т.д.

Основной функционал авито (MVP):
1. Разсещение объявлений.
2. Поиск объявлений.
3. Просмотр объявлений.
4. Текстовый чат с продавцом.

## 1. Целевая аудитория

| Страна                                            | Кол-во посещений за месяц  |
|---------------------------------------------------|----------------------------|
| Россия                                            | 363.5 млн (95%)            |
| Украина                                           | 8 млн (2.1%)               |
| Казахстан                                         | 0.9 млн (0.2%)             |
| Другие                                            | 7.6 млн (2%)               |
| Всего                                             | 380 млн                    |

Кол-во уникальных пользователей ~ 50 млн человек

Данные взяты за август 2022 г. с сайта https://www.similarweb.com/website/avito.ru/#traffic <br>
Как видно из таблицы и из тематики сервиса, сервис Avito ориентирован только на российский рынок.

## 2. Расчет нагрузки

### 2.1 Продуктовые метрики

Рассчитаем размер хранилища для пользователя. Основное, что расходует память - объявления.
Сейчас на авито размещено 121.898.958 объявлений (https://www.avito.ru/company).
Допустим, у каждого объявления есть:
1. Описание - 500 символов (500 байт).
2. Фотографии - 5 штук. (5 * 1 Мбайт = 5 Мбайт).
3. Чат, связанный с объявлением - 1000 символов (1000 байт).
Размером хранения текста на фоне фотографий можно принебречь. Получаем, что в среднем 1 объявление занимает 5Мбайт. 
На авито 50.000.000 активных пользователей, т.е ~ 3 размщенных объявления в среднем у человека.
К этому добавим место, занимаемое профилем пользователя и получаем, что хранилище пользователя ~ 20 Мбайт


| Метрика                                           | Значение                   |
|---------------------------------------------------|----------------------------|
| Месячная аудитория                                | 380 млн                    |
| Дневная аудитория                                 | 12.3 млн                   |
| Средняя глубина просмотра сайта                   | 10.93 страниц              |
| Средняя длительность посещения                    | 11 минут                   |
| Средний объем данных пользователя                 | 20 Мбайт                   |

| Действие                                          | Кол-во (на одного человека/день) |
|---------------------------------------------------|----------------------------------|
| Размещение объявления                             | 0.008                            |
| Поиск и просмотр объявлений                       | 5                                |


### 2.2 Технические метрики


## N. Источники
1. https://www.similarweb.com/website/avito.ru/#traffic
2. https://www.avito.ru/company
3. https://www.vedomosti.ru/forum/riteil22/columns/2022/04/19/918717-nasha-auditoriya-stala--bolee-vovlechennoi
4. https://tass.ru/ekonomika/12595407
