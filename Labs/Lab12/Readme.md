# Настройка NAT для IPv4
### Topolgie
![Topologie](https://user-images.githubusercontent.com/99610266/173250607-a0313138-b7de-4d0d-83ca-b73decfa8f84.png)
## Настройка и проверка NAT для IPv4.
#### Настройка произведена согласно пунктам в методичке.
#### Пинг проходит.
![2](https://user-images.githubusercontent.com/99610266/173357071-d117016c-1140-4feb-ba4c-cb4b3a50f614.png)
#### Во что был транслирован внутренний локальный адрес PC-B?
#### PC-B - 209.165.200.228 
#### Какой тип адреса NAT является переведенным адресом?
#### Inside global
#### Пинг с коммутаторов уже не проходит, т.к адреса все заняты.
#### Очистка NAT прошла успешно.
![3](https://user-images.githubusercontent.com/99610266/173255543-eec2ccd0-369c-4687-b1dc-c4d976959206.png)
### Настройка и проверка PAT для IPv4
#### ip nat inside source list 1 pool PUBLIC_ACCESS overload 
#### Настроен PAT
![4](https://user-images.githubusercontent.com/99610266/173661847-c41532bf-b552-42cc-8a47-7537abaa1802.png)
#### Во что был транслирован внутренний локальный адрес PC-B?
#### Во внешний адрес outside global(сокет с указанием порта)
#### Какой тип адреса NAT является переведенным адресом?
#### Outside global
#### Чем отличаются выходные данные команды show ip nat translations из упражнения NAT?
#### Заполнился стоблец с outside global and ouside local. Отображаются сокеты, для определения порта.
#### При одновременном трафике адрес используется один.
![6](https://user-images.githubusercontent.com/99610266/173664788-ff897709-6e5c-421a-bd1e-62e0e63ececf.png)
#### Как маршрутизатор отслеживает, куда идут ответы? 
#### За счет портов.
