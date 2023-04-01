## Part 1. Установка ОС
- ``Смотрим версию Ubuntu после установки ``<br>
![Alt text](./images/1.jpg "Optional Title")<br>

## Part 2. Создание пользователя
- ``Создаём пользователя и назначаем ему группу adm(новый пользователь в конце).``<br>
![Alt text](./images/2.jpg "Optional Title")<br>
![Alt text](./images/21.jpg "Optional Title")<br>

## Part 3. Настройка сети ОС
- ``Задаtv название машины user-1``<br>
![Alt text](./images/31.jpg "Optional Title")<br>
- ``Установливаем временную зону, соответствующую вашему текущему местоположению.``<br>
![Alt text](./images/32.jpg "Optional Title")<br>
- ``Вывовдим названия сетевых интерфейсов``<br> 
<b>lo (loopback device)</b> -- виртуальный интерфейс, присутствующий по умолчанию в любом Linux. Он используется для отладки сетевых программ и запуска серверных приложений на локальной машине. С этим интерфейсом всегда связан адрес 127.0.0.1. У него есть dns-имя – localhost.
![Alt text](./images/33.jpg "Optional Title")<br>

- ``Узнали внешний IP-адрес``<br>
![Alt text](./images/34.jpg "Optional Title")<br>

- ``Получили ip от dhcp сервера``<br>
<b>DHCP</b> -  Dynamic Host Configuration Protocol
![Alt text](./images/34.png "Optional Title")<br>

- ``Внешний ip-адрес шлюза ``<br>
![Alt text](./images/34.jpg "Optional Title")<br>

- ``внутренний IP-адрес шлюза, он же ip-адрес по умолчанию (gw)``<br>
![Alt text](./images/35.jpg "Optional Title")<br>

- ``Задали статичные настройки ip, gw, dns, изменив файл /etc/netplan/*.yaml``<br>
![Alt text](./images/36.png "Optional Title")<br>

- ``Выполнили команду reboot. Статичные сетевые настройки (ip, gw, dns) соответствуют заданным в предыдущем пункте``<br>
![Alt text](./images/37.jpg "Optional Title")<br>

- ``Пропинговали удаленные хосты 1.1.1.1``<br>
![Alt text](./images/38.jpg "Optional Title")<br>


## Part 4. Обновление ОС
- ``Обновили системные пакеты до последней версии``<br>
![Alt text](./images/41.jpg "Optional Title")<br>
![Alt text](./images/42.jpg "Optional Title")<br>

## Part 5. Использование команды sudo
-<b>sudo</b> - позволяет временно поднимать привилегии и выполнять задачи администрирования системы с максимальными правами<br>
``Добавили пользователя в группу с привилегиями sudo, переключились на этого пользователя и поменяли hostname``<br>
![Alt text](./images/5.jpg "Optional Title")<br>
![Alt text](./images/51.jpg "Optional Title")<br>

## Part 6. Установка и настройка службы времени
- ``Kорректное время и вывод команды``<br>
![Alt text](./images/6.jpg "Optional Title")<br>

## Part 7. Установка и использование текстовых редакторов
- ``Используя каждый из трех выбранных редакторов, создайте файл test_X.txt, где X -- название редактора, в котором создан файл. Напишите в нём свой никнейм, закройте файл с сохранением изменений.``<br>
<b>VIM</b>. Для выхода из режима редактирования: esc, для сохранения: :wq <br>
![Alt text](./images/71.jpg "Optional Title")<br>

<b>NANO</b>.  Для сохранения: ^O + подтвердить, выход: ^X<br>
![Alt text](./images/72.jpg "Optional Title")<br>

<b>JOE</b>. Для сохранения и выхода: ^KX + подтвердить<br>
![Alt text](./images/73.jpg "Optional Title")<br>


- ``Используя каждый из трех выбранных редакторов, откройте файл на редактирование, отредактируйте файл, заменив никнейм на строку "21 School 21", закройте файл без сохранения изменений.``<br>
<b>VIM</b>. Для выхода без сохранения :q! <br>
![Alt text](./images/74.jpg "Optional Title")<br>

<b>NANO</b>.  Для выхода без сохранения: ^X, No<br>
![Alt text](./images/75.jpg "Optional Title")<br>

<b>JOE</b>. Для выхода без сохранения: ^C, yes<br>
![Alt text](./images/76.jpg "Optional Title")<br>











