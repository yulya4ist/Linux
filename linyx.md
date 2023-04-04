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
- <b>sudo</b> - позволяет временно поднимать привилегии и выполнять задачи администрирования системы с максимальными правами<br>
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

<b>NANO</b>.  Для выхода без сохранения: ^X, N<br>
![Alt text](./images/75.jpg "Optional Title")<br>

<b>JOE</b>. Для выхода без сохранения: ^C, y<br>
![Alt text](./images/76.jpg "Optional Title")<br>


- ``Используя каждый из трех выбранных редакторов, отредактируйте файл ещё раз, а затем освойте функции поиска по содержимому файла (слово) и замены слова на любое другое.``<br>

<b>VIM</b>. Для поиска: /"cлово для поиска" <br>
![Alt text](./images/731.jpg "Optional Title")<br>
 Для замены: :s/"cлово для замены"/"замена" <br>
![Alt text](./images/732.jpg "Optional Title")<br>
 
 
<b>NANO</b>. Для поиска: ^W <br>
![Alt text](./images/733.jpg "Optional Title")<br>
 Для замены: ^R <br>
![Alt text](./images/734.jpg "Optional Title")<br>

<b>JOE</b>. Для поиска: ^K F <br>
![Alt text](./images/735.jpg "Optional Title")<br>
 Для замены: ^K F, затем R, Y <br>
![Alt text](./images/736.jpg "Optional Title")<br>


## Part 8. Установка и базовая настройка сервиса SSHD
- ``Установить службу SSHd.``<br>
![Alt text](./images/81.png "Optional Title")<br>
- ``Добавили автостарт.``<br>
![Alt text](./images/82.png "Optional Title")<br>
- ``Поменяли порт на 2022.``<br>
![Alt text](./images/8_0.png "Optional Title")<br>
- ``Установили net-tools.``<br>
![Alt text](./images/83.png "Optional Title")<br>
- ``Используя команду ps, показали наличие процесса sshd.``<br>
![Alt text](./images/8_00.png "Optional Title")<br>
<b>ps</b> - выводит сведения о процессах в статическом виде.<br>
<b>-e</b> - позволяет выбрать все процессы.<br>
<b>| grep sshd </b>- поиск по выводу через пайп.<br>
- ``Вывод команды  <b>netstat -tan</b>.``<br>
![Alt text](./images/84.png "Optional Title")<br>
- ``Значение ключей -tan:``<br>
<b>-a</b> - Показывать состояние всех сокетов; обычно сокеты, используемые серверными процессами, не показываются.<br>
<b>-n</b> - Показывать сетевые адреса как числа. netstat обычно показывает адреса как символы.<br>
<b>-t</b> - Отображать TCP подключения<br>
<b>Proto</b> - Содержит тип протокола<br>
<b>Recv-Q</b> - Счётчик байтов не скопированных программой пользователя из этого сокета.<br>
<b>Send-Q</b> - Счётчик байтов, не подтверждённых удалённым узлом.<br>
<b>Local Address</b> - Адрес и номер порта локального конца сокета.<br>
<b>Foreign Address</b> - Адрес и номер порта удалённого конца сокета.<br>
<b>State </b>- Состояние сокета.<br>
<b>LISTEN</b> Сокет ожидает входящих подключений.<br>
<b>SYN_SENT</b> Сокет, находящийся в режиме активной попытки установки подключения.<br>
<b>0.0.0.0</b> - это немаршрутизируемый адрес IPv4, который используется в качестве адреса по умолчанию или адреса-заполнителя. <br>


## Part 9. Установка и использование утилит top, htop
-htop
 - отсортированному по PID
   ![Alt text](./images/91.png "Optional Title")
 - отсортированному по PERCENT_CPU
   ![Alt text](./images/92.png "Optional Title")
 - отсортированному по PERCENT_MEM
   ![Alt text](./images/93.png "Optional Title")
 - отсортированному по TIME
   ![Alt text](./images/94.png "Optional Title")

















