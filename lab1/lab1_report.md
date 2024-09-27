
> University: [ITMO University](https://itmo.ru/ru/)</br>
> Faculty: [FICT](https://fict.itmo.ru)</br>
> Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/)</br>
> Year: 2023/2024</br>
> Group: U4125</br>
> Author: Malov Igor Vyacheslavovich</br>
> Lab: Lab1</br>
> Date of create: 27.09.2024</br>
> Date of finished: 27.09.2024</br>



## Лабораторная работа №1 "Обзор Google Cloud и исследование основных сервисов."
### Шаг 1.
Зашел в Google Cloud. Перешел во вкладку IAM и в разделе Service Accounts создал сервис-аккаунт, назвал его "imalov-sa-lab1" и назначил роль сервис-аккаунту доступ Storage admin.
![photo_2024-09-27_16-20-21](https://github.com/user-attachments/assets/2bd5b27c-9351-4fa8-a70d-43c405065af2)


### Шаг 2.
Зашел во вкладку Computee Engine,  создал виртуальную машину. Задал название и нужные параметры - type e2-micro в режиме spot . Выбарал свой аккаунт в качестве администратора.
![Снимок экрана 2024-09-27 165057](https://github.com/user-attachments/assets/45575e2f-7695-4ccd-9f44-a15375006f50)


### Шаг 3.
Нажал на кнопку SSH. Открылась консоль и в ней я с помощью утилиты gsutils нашел бакет lab1-bucket-itmo. Скопировал оттуда 3 файла в локальную папку на VM. 
При помощи команды ls -lah отобразил что эти файлы хранятся на моей VM.
![Снимок экрана 2024-09-27 165847](https://github.com/user-attachments/assets/721c3d67-c6e9-46da-bf59-341cbc9f4c16)


### Шаг 4.
Зашел во вкладку IAM, Поменял права доступа своего сервис-аккаунта со Storage Admin на Compute Viewer. 
![Снимок экрана 2024-09-27 170356](https://github.com/user-attachments/assets/3acb5ba9-175f-4346-bc76-0b393d393242)
После этого было отказано в доступе при копировании файла
![Снимок экрана 2024-09-27 170725](https://github.com/user-attachments/assets/028eb508-c909-4e15-8fb7-c499b5cf071c)

### Шаг 5.
Удалил за собой VM 
![Снимок экрана 2024-09-27 170825](https://github.com/user-attachments/assets/0ee8c404-283d-4f6c-922b-f776da8b1177)

**Вывод**: Google Cloud дает возможность эффективно управлять доступом к рабочим ресурсам, делая этот процесс гибким 
