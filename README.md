#Работа с git и bash
Bash2 
1. cd 
    Зайти в домашнюю директорию через терминал
2. mkdir 
    test3 Создать папку test 3
3.  echo -e "row1\nrow2\nrow3\nrow4" > 4.txt
    echo -e "row1\nrow2\nrow3\nrow4" > 5.txt
    echo -e "row1\nrow2\nrow3\nrow4" > 6.txt
Добавить в папку test 3 три файла 4, 5 и 6, в каждом из которых должно быть по 4 строки row1, row2, row3, row4
4. grep "row2" 5.txt
    Найдите строку row2 в файле 5
5.grep -r "row" 
    Найдите строку row в папке test3
6. grep -c "row" 6.txt
    Посчитайте сколько строк с содержимым row в файле 6
7.выполнить cd 
find test3 -name "5.txt"
    Найдите файл 5 внутри папки test3
8. find test3 -name "5.txt" -exec rm {} \;
    Используя команду find, удалите файл 5
9.echo "test" > test3/4.txt 
    Используя команду echo, добавить слово test в файл 4 (без сохранения содержимого)
10.sed -i 's/test/fail/g' 4.txt // ????? invslid code 
    Заменить слово test в файле 4 на fail
11.echo "test" >> /4.txt 
    Добавить в файл 4 слово test, сохраняя его содержимое
12. ps aux
П   росмотреть все процессы для пользователей, не только в консоли, которые происходят в системе
13.kill 666
    Убить процесс с ID 666 в консоли 
14.ping rusau.net
    Узнать доступность ресурса rusau.net, используя ping
15.ping -c 5 rusau.net
    Отправить 5 пакетов на сайт rusau.net
16.curl -X GET "https://petstore.swagger.io/v2/pet/findByStatus?status=sold"
    Используя GET и команду curl, получить информацию о зарегистрированных питомцах с любым статусом на https://petstore.swagger.io/:curl -X GET "https://petstore.swagger.io/v2/pet/findByStatus?status=available"
17. curl -X POST "https://petstore.swagger.io/v2/user" -H "Content-Type: application/json" -d '{"id": 1111, "username": "lizard", "firstName": "li", "lastName": "love", "email": "user@example.com", "password": "lizkinc", "phone": "1234567890", "userStatus": 0}'
    Используя POST и команду curl, создать нового пользователя на https://petstore.swagger.io/
