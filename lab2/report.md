University: [ITMO University](https://itmo.ru/ru/)

Faculty: [FICT](https://fict.itmo.ru)

Course: [IP-telephony](https://github.com/itmo-ict-faculty/ip-telephony)

Year: 2024/2025

Group: K34202

Author: Arefyev Dmitriy Vladimirovich

Lab: Lab2

Date of create: 16.03.2025

Date of finished: 14.04.2025

# Лабораторная работа №2 "Конфигурация voip в среде Сisco packet tracer"

<b>Цель работы:</b> Изучить построение сети IP-телефонии с помощью маршрутизатора Cisco 2811, коммутатора Cisco catalyst 3560 и IP телефонов Cisco 7960.

## Ход выполнения работы 

### Часть 1

1. Соберем схему сети.

![Снимок экрана от 2025-03-31 15-39-38](https://github.com/user-attachments/assets/4a1498ec-6cd0-4aab-a91f-a1a5062e0943)

2. Отключим ввод слов от DNS серверов.

![Снимок экрана от 2025-03-31 15-41-21](https://github.com/user-attachments/assets/079ab552-c234-48ac-86d9-f533978109de)  

3. Зададим пароли для защиты маршрутизатора сначала в удаленном режиме, потом в режиме консоли

![Снимок экрана от 2025-03-31 15-42-38](https://github.com/user-attachments/assets/1be60dc0-69ca-4557-af78-4e6869a80a0b)
![Снимок экрана от 2025-03-31 15-43-03](https://github.com/user-attachments/assets/5596dd7a-b91d-43d4-a0e5-320b9fe5a301)

4. Настроим интерфейс fa0/0 на маршрутизаторе

![Снимок экрана от 2025-04-01 13-02-32](https://github.com/user-attachments/assets/820e565f-a472-4c8d-b910-ce84b1c68afb)

5. Снова, как и в первой работе, настроим dhcp сервер для передачи данных и пропишем option 150

![Снимок экрана от 2025-04-01 13-03-41](https://github.com/user-attachments/assets/2b6fd3c9-3204-4d97-a24f-c986cd65ccfd)

6. Далее настроим Cisco CallManager Express.

![Снимок экрана от 2025-04-01 13-09-15](https://github.com/user-attachments/assets/160a7553-b8fe-4a0a-8719-fc7e0596a564)

7. Выдадим телефонам собственные номера

![Снимок экрана от 2025-04-01 13-12-48](https://github.com/user-attachments/assets/fc6e1a85-db95-40ab-95bf-c673ad1e0419)

8. Назначим порты для vlan1

![Снимок экрана от 2025-04-01 13-18-17](https://github.com/user-attachments/assets/eacaaad7-f834-4d9d-aedc-c36a452e3604)

8. Проверим связность телефонов. Успешно.

![Снимок экрана от 2025-04-01 13-20-11](https://github.com/user-attachments/assets/51966a7b-b6cf-44a1-abbd-3df2cd361543)

### Часть 2

1. Соберем новую схему сети

![Снимок экрана от 2025-04-01 13-25-39](https://github.com/user-attachments/assets/12cdc882-d2b3-4a5b-90d6-58b68fafc581)

2. Создадим нужные vlan порты на коммутаторе и сразу укажем маршрут по умолчанию

![Снимок экрана от 2025-04-01 14-33-22](https://github.com/user-attachments/assets/3cf6eca0-17f8-428e-a045-31fc461c9282)
![Снимок экрана от 2025-04-01 14-34-54](https://github.com/user-attachments/assets/4c30bd04-f08a-4c32-be1b-50ec164d64be)

3. Настроим интерфейсы 

![Снимок экрана от 2025-04-01 14-36-51](https://github.com/user-attachments/assets/18e707f3-a137-42b9-9b96-d97b85856b4c)
![Снимок экрана от 2025-04-01 14-38-14](https://github.com/user-attachments/assets/ac3af150-8976-4b6e-9f77-463391342950)

4. Создадим логические саб-интерфейсы для VLAN

![Снимок экрана от 2025-04-01 14-42-18](https://github.com/user-attachments/assets/14275512-25f1-4f49-b828-97c5a7a48926)

5. Исключим из пула адреса маршрутизатора и DNS-сервера
   
![Снимок экрана от 2025-04-01 14-43-07](https://github.com/user-attachments/assets/503894cc-9207-49b7-a269-8de932104270)

6. Настроим DHCP-сервер.

![Снимок экрана от 2025-04-01 14-44-51](https://github.com/user-attachments/assets/a6e46cc2-b343-4582-a373-b405fe3180ab)

7. Настроим телефонию.

![Снимок экрана от 2025-04-01 14-45-20](https://github.com/user-attachments/assets/5912c85e-cef9-4dbe-9fe9-03e6ab28e7a1)

7. Выдадим телефонам номера.

![Снимок экрана от 2025-04-01 14-46-26](https://github.com/user-attachments/assets/74319051-79e0-4dc8-86da-b84215e9b274)

8. На компьютерах включим режим DHCP и проверим связность компьютеров и телефонов

![Снимок экрана от 2025-04-01 14-47-47](https://github.com/user-attachments/assets/648d5688-ef30-4027-a389-883fb044440b)
![photo_2025-04-14_12-30-13](https://github.com/user-attachments/assets/4774deaa-0c5a-4b2b-a604-643fbd35a32e)

<b>Вывод:</b> В ходе выполнения данной работы были получены навыки построения сложной сети, в которой одновременно присутствуют и компьютеры, и телефоны, с помощью маршрутизатора Cisco 2811 и коммутатора Cisco catalyst 3560.
