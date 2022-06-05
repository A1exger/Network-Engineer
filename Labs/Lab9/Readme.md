#  Конфигурация безопасности коммутатора 
## Topologie
![Снимок экрана 2022-06-05 113005](https://user-images.githubusercontent.com/99610266/172042229-1484dfe0-d052-4d36-8ac0-fe524848de32.png)
### Настройка маршрутизоатора и настройка сетей коммутаторов в Части 2 была произведена.
![1](https://user-images.githubusercontent.com/99610266/172042299-648948b5-430d-47d5-a514-99fbd1ae75ff.png)
## Настройка безопасности коммутатора.
### Релизация магистральных соединений 802.1Q.
#### Done.
![2](https://user-images.githubusercontent.com/99610266/172042839-dca4ee96-aedb-456a-9171-e1023afb6c9f.png)
### Отключить согласование DTP F0/1 на S1 и S2. 
#### Done.
![3](https://user-images.githubusercontent.com/99610266/172042898-ddaf4a71-115f-4ab0-9681-f1e5ef74c1e4.png)
### Настройка портов доступа и безопасность неиспользуемых портов коммутатора
#### Done.
![4](https://user-images.githubusercontent.com/99610266/172043339-8934c3c4-3b51-4088-b161-5ea02ec7f7f1.png)
### Документирование и реализация функций безопасности порта.
![5](https://user-images.githubusercontent.com/99610266/172043590-def61648-8467-4252-961b-2a87141a7d21.png)
#### CPT не реализована команада.
![6](https://user-images.githubusercontent.com/99610266/172046148-e1fe65c6-0e06-4400-b3b6-c613b9b4941e.png)
#### Задать тип нет возможности.
#### Остальные настройки успешно установлены на портах коммутаторов.
![7](https://user-images.githubusercontent.com/99610266/172046193-d6b1b666-93fc-47f6-8fcc-1b7b87a2ed76.png)
### Реализация безопасности DHCP snooping
#### При включении DHCP snooping компютер подключенный к коммутатору S2 перестает получать IP address. 
#### Как настраивал:
#### 1. ip dhcp snooping
#### 2. ip dhcp snooping vlan 10
#### 3. В интерфейсе Fa-0/1 в сторону коммутатора S1 настроил Trust
#### 4. На интерфейсе Fa-0/18 настроил лимит в 5 пакетов как указано в методичке.
#### 5. Добавил для проверки включил другой пк на 2-й порт. Адрес также не получает, при установлении этого порта в trust получает. 

![8](https://user-images.githubusercontent.com/99610266/172061778-7e00fe12-c5ed-4e91-81f4-c271b3ff08ef.png)

![9](https://user-images.githubusercontent.com/99610266/172061783-d5184e93-2ffd-4bf3-9c37-ec8ce137586b.png)

![10](https://user-images.githubusercontent.com/99610266/172061790-a79b7c08-e016-468a-9dc0-ba14544b2986.png)

![11](https://user-images.githubusercontent.com/99610266/172061792-c0fe1b9f-890a-4189-b353-be7779c43514.png)

![12](https://user-images.githubusercontent.com/99610266/172061794-c5451aac-9c3c-4f39-9e06-ef0a3f801ec9.png)


