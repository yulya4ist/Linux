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
- <b>lo (loopback device)</b> -- виртуальный интерфейс, присутствующий по умолчанию в любом Linux. Он используется для отладки сетевых программ и запуска серверных приложений на локальной машине. С этим интерфейсом всегда связан адрес 127.0.0.1. У него есть dns-имя – localhost.
![Alt text](./images/33.jpg "Optional Title")<br>

- ``Узнали внешний IP-адрес``<br>
![Alt text](./images/34.jpg "Optional Title")<br>

- ``Получили ip от dhcp сервера``<br>
- <b>DHCP</b> -  Dynamic Host Configuration Protocol
![Alt text](./images/34.png "Optional Title")<br>

- ``Внешний ip-адрес шлюза ``<br>
![Alt text](./images/34.jpg "Optional Title")<br>

- ``внутренний IP-адрес шлюза, он же ip-адрес по умолчанию (gw)``<br>
![Alt text](./images/35.jpg "Optional Title")<br>

- ``Задали статичные настройки ip, gw, dns, изменив файл /etc/netplan/*.yaml``<br>
![Alt text](./images/36.png "Optional Title")<br>















