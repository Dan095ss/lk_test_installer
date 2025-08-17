1. Чтобы понять где сделан инсталлятор, скачаю пакет утилит sysinternals suite.
<img width="689" height="377" alt="image" src="https://github.com/user-attachments/assets/ce3ed4dd-325b-4d02-8c70-18d0ec1a7752" />

2. В рамках этого пакета запущу через терминал утилиту strings. Обнаружим название inno setup!!!! Пазл начинает собираться
<img width="763" height="54" alt="image" src="https://github.com/user-attachments/assets/d01c8ea3-b4af-4122-af37-315c01f71a83" />

3. Скачаем сразу Inno Setup Compilator, чтобы собрать инсталлятор, а также innounp, чтобы наш сломанный инсталлятор разобрать.
4. Разбираем наш инсталлятор
<img width="864" height="211" alt="image" src="https://github.com/user-attachments/assets/fe64282b-11ef-4a5a-ad92-63c2c6845acd" />

5. Получаем на выходе множество файлов, а также файл .iss c конфигом. Он нам и нужен
6. Открываем полученный файл через Inno Setup и меняем ошибочный параметр директории (был указан диск Б вместо С)
<img width="1280" height="680" alt="image" src="https://github.com/user-attachments/assets/30b2d6c5-6238-4b78-adf2-35c44782fb93" />

7. А также даем возможность пользователю самому выбрать директорию. Лишние строки вызывающие конфликты - удаляем.
<img width="462" height="177" alt="image" src="https://github.com/user-attachments/assets/42b391e0-641a-42c1-b8e4-b2cb4f8ca38a" />

8. Компилируем и получаем красивый и рабочий установщик. Проверяем работоспособность
<img width="829" height="768" alt="image" src="https://github.com/user-attachments/assets/dd4b180d-90be-4f85-bdd9-2e2ff6d154b4" />
<img width="540" height="421" alt="image" src="https://github.com/user-attachments/assets/4259e9b2-570a-41f7-86c1-086daaf2ba5c" />
<img width="639" height="142" alt="image" src="https://github.com/user-attachments/assets/9ce1e238-38e4-4111-b089-4f15735c5678" />
<img width="823" height="379" alt="image" src="https://github.com/user-attachments/assets/8e396f5c-d19f-4ab3-9674-59f6ff578b5d" />
