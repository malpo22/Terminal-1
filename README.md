# Terminal-1
Terminal (GitBash) Commands
HW 1 Terminal (GitBash) commands

1) Посмотреть где я
- pwd
2) Создать папку
- mkdir group_30_hw
3) Зайти в папку
- cd group_30_hw
4) Создать 3 папки
- mkdir folder_1 folder_2 folder_3
5) Зайти в любую папку
- cd folder_1
6) Создать 5 файлов (3 txt, 2 json)
- touch qq_1.txt qq_2.txt qq_3.txt
- cat > qq_4.json ^C
- cat > qq_5.json ^C
7) Создать 3 папки
- mkdir f_1 f_2 f_3
8) Вывести список содержимого папки
- ls -la
9) Открыть любой txt файл
- vim qq_1.txt
10) написать туда что-нибудь, любой текст.
- i -
This is my first homework at this course. It seems to be quite difficult. I hope I can manage it. Thank you

11) сохранить и выйти
- esc :wq
12) Выйти из папки на уровень выше
- cd ..
13) переместить любые 2 файла, которые вы создали, в любую другую папку
- mv folder_1/qq_2.txt folder_2/qq_1.txt
- mv folder_1/qq_4.json folder_2/qq_4.json
14) скопировать любые 2 файла, которые вы создали, в любую другую папку
- cp folder_1/qq_3.txt folder_3/qq_3.txt
- cp folder_1/qq_5.json folder_3/qq_5.json
15) Найти файл по имени
- find . -name qq_1.txt
- find . -name *.json
16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает
- grep this folder_1/qq_1.txt
- grep -v homework folder_1/qq_1.txt
- grep -c this folder_1/qq_1.txt
- grep -R this folder_1
- grep -i this folder_1/qq_1.txt
17) вывести несколько первых строк из текстового файла
- head -2 folder_1/qq_1.txt
18) вывести несколько последних строк из текстового файла
- tail -2 folder_1/qq_1.txt
19) просмотреть содержимое длинного файла (команда less) изучите как она работает.
- less qq_1.txt
- /be
- -q (завершить работу в less)
20) вывести дату и время
- date



=========

Задание *

21) Отправить http запрос на сервер.
http://162.55.220.72:5005/terminal-hw-request

curl "http://162.55.220.72:5005/terminal-hw-request"

curl: (7) Failed to connect to 162.55.220.72 port 5005: Connection refused MacBook-Air-MacBook:~ macbook$

22) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

#!/bin/bash

MacBook-Air-MacBook:~ macbook$ cat > script.sh << E0F

#!/bin/bash

-pwd
- mkdir group_30_hw
- cd group_30_hw
- mkdir folder_1 folder_2 folder_3
- cd folder_1
- touch qq_1.txt qq_2.txt qq_3.txt qq_4.json qq_5.json
- mkdir f_1 f_2 f_3
- ls -la
- mv folder_1/qq_1.txt folder_2/qq_1.txt
- mv folder_1 qq_4.json folder_2/qq_4.json E0F

-Enter
- chmod +x script.sh
- ./script.sh

MacBook-Air-MacBook:~ macbook$ ./script.sh

-bash: ./script.sh: Permission denied

=====================

Посмотреть где я
- pwd
Создать папку
- mkdir foldername
Зайти в папку
- cd foldername
