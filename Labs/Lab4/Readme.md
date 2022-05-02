# IPv6 адресация
### 1. Ручная настройка IPv6-адресов
####  Назначение IPv6-адреса интерфейсам Ethernet на R1
##### После настройки адресов и линк лосал адресов получилась следующая картина.
##### ![1](https://user-images.githubusercontent.com/99610266/166165172-26abb231-5cf9-47fe-972a-2c7d69eef1c6.png)
##### Какие группы многоадресной рассылки назначены интерфейсу G0/0?
##### Все что настроено на интерфейсе это IPv6 адрес и линк локал, коотрый не относится к многорадресной рассылке.
### 2. Активируйте IPv6-маршрутизацию на R1.
##### Назначен ли индивидуальный IPv6-адрес сетевой интерфейсной карте (NIC) на PC-B?
##### ![2](https://user-images.githubusercontent.com/99610266/166166100-e7298870-930f-4527-89cf-968eb2aadc90.png)
##### Включил IPv6 unicast-routing
##### Почему PC-B получил глобальный префикс маршрутизации и идентификатор подсети, которые вы настроили на R1?
##### Изменений со скриншотом не произошло. Т.к на ПК не настаривался адрес, адрес получается из сети FE80::
### 3. Назначение IPv6-адреса интерфейсу управления (SVI) на S1.
##### Результат.
##### ![3](https://user-images.githubusercontent.com/99610266/166166298-e1525800-8e9d-43ef-9135-d4bc66ffb114.png)
### 4. Назначение компьютерам статические IPv6-адреса.
##### Настройки заданы.
### 5. Проверка сквозного подключения
##### С PC-A отправьте эхо-запрос на FE80::1. Это локальный адрес канала, назначенный G0/1 на R1.
##### Отправьте эхо-запрос на интерфейс управления S1 с PC-A.
##### Введите команду tracert на PC-A, чтобы проверить наличие сквозного подключения к PC-B.
##### С PC-B отправьте эхо-запрос на PC-A.
##### С PC-B отправьте эхо-запрос на локальный адрес канала G0/0 на R1.
##### Все подключения осуществлены.
##### ![4](https://user-images.githubusercontent.com/99610266/166166590-d2d31748-3d93-4c83-81a7-7e15419cf486.png)
#### Вопросы для повторения.
##### 1.	Почему обоим интерфейсам Ethernet на R1 можно назначить один и тот же локальный адрес канала — FE80::1?
##### LLA не являются маршрутизируемыми и ограничиваются одним каналом.
##### 2.	Какой идентификатор подсети в индивидуальном IPv6-адресе 2001:db8:acad::aaaa:1234/64?
##### Идентификатор подсети 2001:db8:acad::aaaa