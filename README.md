# Docker
В цьому репозиторії я показую як ознайомлювався з докером


1. Після того як ми встановили докер, нам потрібно переконатися що все встановилося корректно, можна це зробити за допомогою команди
docker run -d -p 8080:80 docker/welcome-to-docker та перейдіть до сайту http://localhost:8080

[screenshots/photo_5_2024-09-09_21-49-46.jpg](https://github.com/T1mber-W0lf/Docker/blob/main/screenshots/photo_5_2024-09-09_21-49-46.jpg)

якщо ви все зробили вірно, то на сайті буде показана картинка

[screenshots/photo_4_2024-09-09_21-49-46.jpg](https://github.com/T1mber-W0lf/Docker/blob/main/screenshots/photo_4_2024-09-09_21-49-46.jpg)

2.Тепер клонуємо або завантажуємо проєкт, та переходимо в каталог проєкту.
  Скопіювати проєкт можна за допомогою команди:
    git clone https://github.com/docker/getting-started-todo-app
  Перейти до каталогу проєкту:
    cd getting-started-todo-app
Коли ми перейшли до каталогу, треба запустити докер за допомогою команди
docker compose watch

[screenshots/photo_10_2024-09-09_21-49-46.jpg](https://github.com/T1mber-W0lf/Docker/blob/main/screenshots/photo_10_2024-09-09_21-49-46.jpg)

якщо все зроблено вірно, то на сайті буде показуватися наступне

[screenshots/photo_2_2024-09-09_21-49-46.jpg](https://github.com/T1mber-W0lf/Docker/blob/main/screenshots/photo_2_2024-09-09_21-49-46.jpg)

Тепер пропоную змінити деякі файли, та подивитися на результат,я змінив файли getGreeting.js, AddNewItemForm.jsx, index.scss
А саме я змінив колір сторінки, зробив різні написи, та в полі для введеня тексту зробив заглушку у виді тексту

  getGreeting.js:[screenshots/photo_8_2024-09-09_21-49-46.jpg](https://github.com/T1mber-W0lf/Docker/blob/main/screenshots/photo_8_2024-09-09_21-49-46.jpg)

Ось що змінилося після зміни:[screenshots/photo_9_2024-09-09_21-49-46.jpg](https://github.com/T1mber-W0lf/Docker/blob/main/screenshots/photo_9_2024-09-09_21-49-46.jpg),[screenshots/photo_13_2024-09-09_21-49-46.jpg](https://github.com/T1mber-W0lf/Docker/blob/main/screenshots/photo_13_2024-09-09_21-49-46.jpg)

  AddNewItemForm.jsx:[screenshots/photo_14_2024-09-09_21-49-46.jpg](https://github.com/T1mber-W0lf/Docker/blob/main/screenshots/photo_14_2024-09-09_21-49-46.jpg)

ось що змінилося після зміни:[screenshots/photo_11_2024-09-09_21-49-46.jpg](https://github.com/T1mber-W0lf/Docker/blob/main/screenshots/photo_11_2024-09-09_21-49-46.jpg)

  index.scss:[screenshots/photo_7_2024-09-09_21-49-46.jpg](https://github.com/T1mber-W0lf/Docker/blob/main/screenshots/photo_7_2024-09-09_21-49-46.jpg)

Результат зміни усіх файлів:[screenshots/photo_1_2024-09-09_21-49-46.jpg](https://github.com/T1mber-W0lf/Docker/blob/main/screenshots/photo_1_2024-09-09_21-49-46.jpg)

3. Наступним кроком буде створення репозиторію для докера, для цього потрібно авторизуватися та створити докер на сайті Docker Hub
Я вже авторизувався та створив репозиторій 

[screenshots/photo_3_2024-09-09_21-49-46.jpg](https://github.com/T1mber-W0lf/Docker/blob/main/screenshots/photo_3_2024-09-09_21-49-46.jpg)

Оскільки ви вже завантажили/скопіювали проєкт, та перейшли до каталогу проєкту, потрібно ввести наступну команду:
docker build -t <DOCKER_USERNAME>/getting-started-todo-app . де замість DOCKER_USERNAME ви підставляете свій юзернейм

[screenshots/photo_12_2024-09-09_21-49-46.jpg](https://github.com/T1mber-W0lf/Docker/blob/main/screenshots/photo_12_2024-09-09_21-49-46.jpg)

Щоб переконатися що зображення існують, використовуйте команду docker image ls

[screenshots/photo_6_2024-09-09_21-49-46.jpg](https://github.com/T1mber-W0lf/Docker/blob/main/screenshots/photo_6_2024-09-09_21-49-46.jpg)

Для того щоб відправити зображення, використовуйте команду docker push <DOCKER_USERNAME>/getting-started-todo-app, де замість DOCKER_USERNAME ви підставляете свій юзернейм
Але мені це не потрібно, оскільки під час виконання команди docker build -t <DOCKER_USERNAME>/getting-started-todo-app,він відправляв зображення

На цьому все, дякую за увагу!


