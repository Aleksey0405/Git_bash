1) Посмотреть где я 
* command: `pwd`
2) Создать папку
* command: `mkdir folder_name`
3) Зайти в папку
* command: `cd folder_name` (если в одном каталоге)
* command: `cd c:/` - конкретный каталог
* command: `cd d:/steam/bin/shadersmkd` - абсолютный путь
4) Cоздать 3 папки
* command: `mkdir nn_1 nn_2 nn_3`
5) Зайти в любую папку
* command: `cd nn_1`
6) Создать 5 файлов (3 txt, 2 json)
* command: `touch text_1.txt text_2.txt text_3.txt`
* command: `touch text_1.json text_2.json`
7) Cоздать 3 папки
* command: `mkdir 1 2 3`
8) Вывести список содержимого папки
* command: `ls` - вывод всех файлов
* command: `ls -la` - подробный вывод содержимого папки
9) Открыть любой txt файл
* command: `vim text_1.txt`
10) Написать туда что-нибудь, любой текст.
* `i` (insert) - режим редактирования
11) Сохранить и выйти.
`Esc` - выход из редактирования
* `:wq` - записать и выйти
12) Выйти из папки на уровень выше
* `cd ..`
* `cd ../..` - выйти на два уровня выше.
13) Переместить любые 2 файла, которые вы создали, в любую другую папку.
* command: `mv text_1.txt text_2.txt 1`
14) Cкопировать любые 2 файла, которые вы создали, в любую другую папку.
* command: `cp text_1.json text_2.json 2`
15) Найти файл по имени
* command `find . -name "text_2.json"`
16) Просмотреть содержимое в реальном времени
* command: `tail -f abab.txt`
17) Вывести несколько первых строк из текстового файла
* command: `head -3 text_1.txt`
18) Вывести несколько последних строк из текстового файла
* command: `tail -3 text_1.txt`
19) Просмотреть содержимое длинного файла (команда less) изучите как она работает.
* command: `less book.txt`
* `q` - выход из режима чтения
20) Вывести дату и время
* command: `date`
__________________________________________________________
##Задание*
* 1) Отправить http запрос на сервер.
http://162.55.220.72:5005/terminal-hw-request

        curl "http://162.55.220.72:5005/get_method?name=Aleksey&age=24" --verbose (доп.сведения)

##Задание**
* 2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13
```css
 #!/bin/ash

 echo "Let's create a random folder to navigate into it..."
 mkdir folder_random
 echo "Coming into..."
 cd folder_random
 echo "Let's create three folders..."
 mkdir folder_1 folder_2 folder_3
 echo "Let's navigate to one of them..."
 cd folder_3
 echo "Let's create 5 files : 3 txt and 2 json..."
 touch text_11 text_22 text_33 text_11.json text_22.json
 echo "Let me show you what's inside..."
 ls -la
 echo "Let's move some files to another folder..."
 mv text_11.json text_22.json D:/QA/sds/as/
 ```