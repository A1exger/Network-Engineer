# Доступ к сетевым устройствам по протоколу SSH
### 1. Настройка основных параметров устройств
##### Настройка основных параметров устройств произведена.
#### Топология
##### ![1](https://user-images.githubusercontent.com/99610266/166168318-4ea40758-1930-4597-a653-826eb0de7c88.png)
### 2. Настройка маршрутизатора для доступа по протоколу SSH
##### Step 1 Настройка аутентификации устройств.
##### В самом начале желательно установить врмя и дату на устройстве. Используется команда clock set 22:33:55 7 May 2022
##### Создание домена для устройства - ip domain name domain.local
##### Имя устройства уже настроено. Генерируем ключ шифрования. crypto key generate rsa 
#### Step 2 Создание ключа шифрования
##### Он запросит (длину) количество бит используемых для шифрования. Минимальный 360 и до 2048. Выбрал 1024.
##### ![2](https://user-images.githubusercontent.com/99610266/167269354-d17b1d38-8fee-43f1-9438-9f9e92d51047.png)
#### Step 3 Создание имя пользователя в локальной базе учетных записей.
##### Далее создается имя пользователя и пароль с высоким приоритетом. username admin privilege 15 secret Adm1nP@55
#### Step 4 Активация протокола SSH на линиях VTY
##### Заходим в интерфейс line vty 0 4. И с помощью команды transport input указываем какие протоколы активируем.
##### Также сразу настраимваем способ входа, привилегии, версию ssh.
##### ![3](https://user-images.githubusercontent.com/99610266/167269776-3827c895-3d5d-4214-ab02-8fab817f6aea.png)
##### Настройка маршрутизатора была произведена. Проверяем.
##### ![2](https://user-images.githubusercontent.com/99610266/166168950-2cb139fb-f52c-4feb-8112-cf81269da60a.png)
### 3. Настройка коммутатора для доступа по протоколу SSH
##### Настройка коммутатора была произведена аналогична маршрутизатору.
##### ![3](https://user-images.githubusercontent.com/99610266/166169428-15c23c58-2acf-4690-a834-694c80cdf329.png)
### 4. Установление с коммутатора S1 соединение с маршрутизатором R1 по протоколу SSH.
##### Установить соединение с коммутатора получилось.
##### ![4](https://user-images.githubusercontent.com/99610266/166169654-b12ef716-4f88-44b9-a5c2-b67232773391.png)
##### Какие версии протокола SSH поддерживаются при использовании интерфейса командной строки?
##### Ver.2
#### Вопрос для повторения
##### Как предоставить доступ к сетевому устройству нескольким пользователям, у каждого из которых есть собственное имя пользователя?
##### Создать каждому используя команду username ***** privilege 15 secret *****
