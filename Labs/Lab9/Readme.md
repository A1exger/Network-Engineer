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
#### Как настраивал:
#### 1. ip dhcp snooping
#### 2. ip dhcp snooping vlan 10
#### 3. В интерфейсе в сторону коммутатора S1 настроил Trust
#### 4. На интерфейсе в сторону ПК-Б настроил лимит в 5 пакетов как указано в методичке.
![15](https://user-images.githubusercontent.com/99610266/172690804-71931ee5-24d4-4bef-b419-fb3da199160b.png)
#### После настройки DHCP Snooping в EVE-NG ПК-Б получает адрес успешно.
![16](https://user-images.githubusercontent.com/99610266/172691320-a333a3f6-fa4f-4dae-a48f-08367e15878f.png)
### Реализация PortFast и BPDU Guard
#### Настройки для PortFast и BPDU Guard были произведены.
![17](https://user-images.githubusercontent.com/99610266/172692667-75e05a49-6eac-4dc8-b67f-05df8e39810c.png)
### Проверка наличия сквозного подключения 
#### Пинги успешно доходят до всех устройств.
![18](https://user-images.githubusercontent.com/99610266/172693265-d62f902c-a70a-45ed-a4f7-4f7e4a16791e.png)
