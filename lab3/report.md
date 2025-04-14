University: [ITMO University](https://itmo.ru/ru/)

Faculty: [FICT](https://fict.itmo.ru)

Course: [IP-telephony](https://github.com/itmo-ict-faculty/ip-telephony)

Year: 2024/2025

Group: K34202

Author: Arefyev Dmitriy Vladimirovich

Lab: Lab3

Date of create: 18.03.2025

Date of finished: 14.04.2025

# Лабораторная работа №3 "Использование Asterisk в качестве SIP proxy"

<b>Цель работы:</b> Изучить программный комплекс Asterisk. Настройка Asterisk для локальных звонков.

## Ход выполнения работы 

1. Установим Asterisk на рабочее устройство

![Снимок экрана от 2025-04-02 13-11-14](https://github.com/user-attachments/assets/24cea051-210a-4f42-a901-669a67badcb7)

2. Отредактируем файл конфигурации ```sip.conf```

![Снимок экрана от 2025-04-02 13-22-11](https://github.com/user-attachments/assets/d5a447f3-b682-417a-b29d-1fa00a77d341)

3. Также измений файл ```extensions.conf``` и перезапустим сервис

![Снимок экрана от 2025-04-02 13-25-39](https://github.com/user-attachments/assets/9a4e0333-08b0-4545-bef8-ba701e584283)
![Снимок экрана от 2025-04-02 13-26-23](https://github.com/user-attachments/assets/285a4206-98ae-493a-84ef-e6c75c737d60)

4. Проверим, работает ли служба

![Снимок экрана от 2025-04-02 13-27-00](https://github.com/user-attachments/assets/5bc47b14-a053-4869-997b-d7451327a47a)

5.Установим утилиту ZoiPer5, скачав пакет с официального сайта

![Снимок экрана от 2025-04-02 13-36-05](https://github.com/user-attachments/assets/85a9ce34-1f66-4473-8ddc-af266958ca4c)

6. Заходим в ZoiPer под логином и паролем созданного ранее аккаунта

![Снимок экрана от 2025-04-02 13-38-06](https://github.com/user-attachments/assets/92b273c2-32f0-4472-b94e-56113789fd85)
![Снимок экрана от 2025-04-02 13-57-35](https://github.com/user-attachments/assets/78023fc8-9714-4f7f-8411-c6fa02b0cbc9)

7. Убедимся, что порт видно в Asterisk

![Снимок экрана от 2025-04-02 13-58-07](https://github.com/user-attachments/assets/6048e6b0-7bb0-4434-94dd-90b72c55f34c)

8. Установим wine - средство запуска на Linux тех приложений, которые предназначены только для Windows

![Снимок экрана от 2025-04-02 13-59-54](https://github.com/user-attachments/assets/9251e2e5-5585-4b60-8f67-d5c5cd25da4b)

9. Теперь через wine установим MicroSIP

![Снимок экрана от 2025-04-02 14-05-47](https://github.com/user-attachments/assets/fa5bdc37-0b59-466e-96ac-afbb8c52bb3d)

10. Далее в MicroSIP входим в созданный ранее аккаунт

![Снимок экрана от 2025-04-02 14-07-29](https://github.com/user-attachments/assets/3cbb6e47-c67d-4c48-9123-6fccb90fac1f)

11. Теперь проверим связность двух телефонов

![Снимок экрана от 2025-04-02 14-12-17](https://github.com/user-attachments/assets/c7e4a670-be9f-469b-ac9d-7e31cefb10b0)

<b>Вывод:</b> В ходе выполнения работы были получены навыки работы с Asterisk и MicroSIP, а также получены практические навыки настройки локальных звонков.
