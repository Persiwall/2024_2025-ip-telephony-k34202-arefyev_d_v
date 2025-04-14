University: [ITMO University](https://itmo.ru/ru/)

Faculty: [FICT](https://fict.itmo.ru)

Course: [IP-telephony](https://github.com/itmo-ict-faculty/ip-telephony)

Year: 2024/2025

Group: K34202

Author: Arefyev Dmitriy Vladimirovich

Lab: Lab1

Date of create: 14.03.2025

Date of finished: 14.04.2025

# Лабораторная работа №1 "Базовая настройка ip-телефонов в среде Сisco packet tracer"

<b>Цель работы:</b> Изучить рабочую среду Cisco Packet Tracer, ознакомиться с интерфейсами основных устройств, типами кабелей, научиться собирать топологию. Изучить построение сети IP-телефонии с помощью маршрутизатора, коммутатора и IP телефонов Cisco 7960 в среде Packet tracer. 

## Ход выполнения работы 

### Часть 1

1. Соберём схему сети из описания работы.

![Снимок экрана от 2025-03-30 18-55-14](https://github.com/user-attachments/assets/1880850e-0f8a-450e-af10-8d6d80d394ce)

2. Выдадим компьютерам ip-адреса.

![Снимок экрана от 2025-03-31 14-34-38](https://github.com/user-attachments/assets/8dad0bff-0a30-4ee0-a2d6-35e285af9486)

3. Далее поднимем интерфейсы и проверим связность устройств.

![Снимок экрана от 2025-03-31 14-48-24](https://github.com/user-attachments/assets/3aa107d5-b2b1-4dec-a072-613f56813658)


Итог: сеть работает корректно, устройства видят друг друга и могут взаимодействовать

### Часть 2

1. Соберем схему сети из второй части задания

![Снимок экрана от 2025-03-31 15-30-59](https://github.com/user-attachments/assets/ac228cd7-9aca-45a3-83e3-803ef1b3fe87)

2. Переименуем роутер в CMERouter

![Снимок экрана от 2025-03-31 15-02-25](https://github.com/user-attachments/assets/e3fc4af3-7fe8-4e60-b92d-016be9c93a47)

3. Настроим интерфейс на роутере

![Снимок экрана от 2025-03-31 14-59-54](https://github.com/user-attachments/assets/5f24982e-55ee-465e-a208-0a278afe70f0)

3. Настроим DHCP: пропишем pool,сеть, а также добавим option 150, чтобы телефоны автоматически использовали настройки с TFTP сервера:

![Снимок экрана от 2025-03-31 15-07-48](https://github.com/user-attachments/assets/94e00201-ab12-4dab-b5f6-746371c2242e)
![Снимок экрана от 2025-03-31 15-08-37](https://github.com/user-attachments/assets/21741cce-7109-4b58-8b36-e79c0a26a310)

4. Далее настроим Cisco CallManager Express

![Снимок экрана от 2025-03-31 15-12-41](https://github.com/user-attachments/assets/d06ade50-a3b2-45ca-a660-bb1b85a941c8)

5. Телефонам были назначены номера 111 и 222

![Снимок экрана от 2025-03-31 15-15-28](https://github.com/user-attachments/assets/d8bb9280-181d-4669-8143-58569ff70e9d)

6. Также был настроен диапазон портов для vlan, с сами порты были переведены в режим access

![Снимок экрана от 2025-03-31 15-18-00](https://github.com/user-attachments/assets/bf7c1fdf-93de-456d-b84e-066145af272e)

7. Проверим связность устройств, позвонив с одного телефона на другой. Телефоны успешно принимают звонки друг от друга.

![Снимок экрана от 2025-03-31 15-29-25](https://github.com/user-attachments/assets/bccc4e58-ecb4-4431-b4a3-ccfe3af43c3c)

<b>Вывод:</b> в ходе выполнения работы были изучены инструменты построения и настройки IP-телефонии в Cisco Packet Tracer, а также получены практические навыки построения сетей, состоящих из телефонов, коммутаторов и маршрутизаторов.
