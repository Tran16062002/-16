САНКТ-ПЕТЕРБУРГСКИЙ НАЦИОНАЛЬНЫЙ ИССЛЕДОВАТЕЛЬСКИЙ УНИВЕРСИТЕТ

ИНФОРМАЦИОННЫХ ТЕХНОЛОГИЙ, МЕХАНИКИ И ОПТИКИ

ФАКУЛЬТЕТ ИНФОКОММУНИКАЦИОННЫХ ТЕХНОЛОГИЙ



Отчет по лабораторной работе №1 по курсу «Информатика »

**Тема: Docker**

***Чан Тхи Лиен***

***К3140***

1. Создать папку **aafire** и файл **Dockerfile**.

![1](https://github.com/user-attachments/assets/36b5c83b-9b69-434d-8d4c-a410d6a910ec)

2. Записать файл.

![9](https://github.com/user-attachments/assets/89d13a94-50b4-416b-85dd-a17004a412fe)

- **libaa-bin** — это утилита, которая запускает анимацию огня в терминале.
- **iputils-ping** — пакет, который включает утилиту ping для тестирования сети.

3. Сборка Docker-образа.

После того как Dockerfile готов, откройте терминал в той же директории, где находится этот файл, и выполните команду для сборки образа:

![2](https://github.com/user-attachments/assets/5b4cc53f-35ec-4128-9a5e-2b873036747a)

Это создаст Docker-образ с тегом **aafire_image**, который содержит приложение aafire и утилиту **ping**.

4. Запуск двух контейнеров с **aafire**.

![7](https://github.com/user-attachments/assets/65182f36-c5fe-4c59-8288-e47e352c0b5c)
![8](https://github.com/user-attachments/assets/6763dce0-e2f5-44bf-abfd-60b358e4532d)

**--name** позволяет задать имена контейнерам для удобства.

5. Создание сети Docker.

Для того чтобы настроить сеть между контейнерами, создайте новую Docker-сеть:

- Выполнит команду: **sudo docker network create myNetwork**

- Проверка настройки созданной вами сети.

![3](https://github.com/user-attachments/assets/fd186ebb-1688-4db2-bb18-298026ead325)

6. Подключение контейнеров к сети.

![4](https://github.com/user-attachments/assets/34620900-7046-4c7b-b028-ff5355239fd8)

7. Тестирование соединения с помощью **ping**.

![5](https://github.com/user-attachments/assets/da627dfc-a7e2-4acc-98b9-39436522cf8c)
![6](https://github.com/user-attachments/assets/8f41337c-6cfd-46bf-9af1-7798b4b34d95)

**Вывод**:

- Использование **docker**.
- Создание контейнер и сети **Docker**.
- Проверка соединения между контейнерами.
