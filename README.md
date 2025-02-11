# Мульти рассылка СМС из 1С для типовых и не типовых конфигураций

[![GitHub release](https://img.shields.io/github/release/Diversus23/multisms.svg)](https://github.com/Diversus23/multisms/releases)

Очень часто в торговых организациях проводятся рассылки своим покупателям об акциях, скидках, новых поступлениях и т.д.
Для этих целей мы создали одну универсальную обработку, которая поможет осуществить смс рассылку в любой конфигурации 1С. Это смс рассылка из 1С.
Для отправки мы используем несколько [сервисов на выбор](https://github.com/Diversus23/multisms#%D1%81-%D0%BA%D0%B0%D0%BA%D0%B8%D0%BC%D0%B8-%D1%81%D0%B5%D1%80%D0%B2%D0%B8%D1%81%D0%B0%D0%BC%D0%B8-%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%B0%D0%B5%D1%82-%D0%BE%D0%B1%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%BA%D0%B0) которые по нашему мнению являются одними из самых функциональных в интернете. Так же есть возможность для юридических лиц заключения договора и оплата безналичным расчетом.
Наша обработка не просто может отправлять СМС, но и позволяет автоматически заполнять сотовые(!) телефонные номера из базы 1С, делать как общие рассылки так и персонализированные, подставляя значения переменных, которые вычисляются для каждого адресата, будь то его долг или фамилия имя, например, узнать баланс и т.д.

![Логотип](https://raw.githubusercontent.com/Diversus23/multisms/master/screen/multismslogo.png "Мульти-рассылка СМС")

## С какими сервисами работает обработка
* [sms.ru](https://sys1c.sms.ru)
* [smsc.ru](http://www.smsc.ru/reg/?ppsoftonit)
* [sms4b.ru](http://sms4b.ru/)
* [smsgorod.ru](http://smsgorod.ru/)
* [terasms.ru](https://terasms.ru/)
* [sms-prosto.ru](https://sms-prosto.ru/)

## Возможности обработки
* Отправка SMS для конфигураций как на обычных формах, так и управляемых;
* Поддержка почти всех типовых конфигураций 1С (УТ 11, УТ 10.3, БП 3.0, ЗУП 3.0, Розница 2.0 и 2.1 и созданные на их базе, УНФ 1.5).
* Из тех конфигураций, которые не поддерживаются есть возможность отправки SMS только не будет заполнения по контактной информации;
* Есть возможность персонализации SMS-сообщений под каждого клиента по формулам;
* Заполнение абонентов как вручную, так и по справочникам конфигурации (Контрагенты, Контактные лица, Сотрудники, Физические лица, Партнеры, Контактные лица партнеров и т.д.);
* Заполнение абонентов по xls-файлу, а так же возможность массового добавления телефонов из буфера обмена
* Выборочная отправка SMS из таблицы;
* Возможность ручной подправки SMS-сообщений перед отправкой;
* Отслеживание статуса доставки SMS-сообщений после их отправки;
* Транслитерация сообщений;
* Информирование о текущем балансе на счету на форме;
* Возможность узнать стоимость отправки смс перед отправкой абонентам;
* Возможность перехода на сайт для пополнения баланса из формы обработки;
* Одна обработка для любой конфигурации на платформе 8.2 или 8.3.

## Итак, для того, чтобы отправлять SMS-сообщения своим клиентам необходимо выполнить следующие шаги:
Шаг 1. Скачиваем обработку на вкладке Скачать она одна для любой конфигурации.

Шаг 2. Распаковываем в папку скачанный архив, в котором инструкция по установке обработки по отправке СМС в Вашу конфигурацию. Устанавливаем по инструкции, либо можем открыть в конфигурации через "Меню > Файл > Открыть".

Шаг 3. В открытой обработке на закладке "Доступ на сайт" выбираем сервис, который будем использовать для рассылки. С тарифами сервиса можно ознакомиться тут же по гиперссылке Тарифы, откроется окно в котором Вы сможете ознакомиться с ценами за рассылку.

Шаг 4. Выбрали сервис из списка на форме, теперь нажимаем кнопку "Регистрация", регистрируемся на сайте. После регистрации на сайте сервиса смс-шлюза вводим логин и пароль от сайта в обработку. Далее можно обновить баланс нажав на кнопку "Обновить баланс" вверху формы. В принципе уже на этом шаге можно попробовать прислать себе тестовую смс. Все сервисы при регистрации дают бесплатные SMS для тестирования функционала.

Шаг 5. Все здорово, но вряд ли Вашему клиенту, которому Вы отправите СМС понравится получать SMS от абонента, например, +79531168017. Можно настроить отправку не от номера, а от буквенного обозначения. Например, SMS будет отправлено не от +79531168017, а от звучного Desheli (к примеру). Давайте согласуем буквенного отправителя.
Нажимаем на кнопку "Согласовать" для согласования буквенного обозначения для отправки SMS.

Вот что у Нас в результате должно получится:

![Что получилось?](https://raw.githubusercontent.com/Diversus23/multisms/master/screen/u0.png "Что получилось?")

Дальше можно заполнить СМС, отправить их и проверить их статусы доставки.

![Заполнение и отправка](https://raw.githubusercontent.com/Diversus23/multisms/master/screen/u6.png "Заполнение и отправка")

Автор: Барилко Виталий Викторович

Сайт публикации: https://softonit.ru/catalog/products/multisms/#detail
