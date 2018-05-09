# Home work №3
## Задания
*Задание с самостоятельной работы:
Написать метод, в который передается номер дня (1-7) и в консоль выводится день недели (Понед - Воскр)
Примечание: кто сделал на уроке, может не делать*

*Дополнение к задаче 6
Усовершенствовать предыдущий метод так, что передав 8 выведется снова же Понедельник, а передав 9 выведется Вторник, 14 - воскресенье, 16 - вторник и тд для любых чисел.
Примечание: кто сделал на уроке, может не делать*

## String:
### Задания Easy
0. Прочесть главу "Strings and Characters" http://swiftbook.ru или https://developer.apple.com/documentation/swift/string
1. Создать строку со своим именем. Написать метод который получает это имя и возвращает кол-во символов в строке с вашим именем. Возвращенное значение показать в консоль
2. Написать метод который принимает 2 слова, например имя и фамилию, возвращает юзернейм который имеет буквы нижнего регистра и разделяет имя и фамилию символом “_”
3. Создать строку с именем и своим отчеством. Создать метод который проверит его на окончание “ич/на”. Выводит “М” или “Ж” в зависимости от окончания. Также учитывать регистр букв, то есть ИЧ или Ич или На и тд.
Подсказка: в классе написан метод который позволяет проверить на суффикс или префикс, найдите и используйте его

**Внимание: если задачи сложные по String будут слишком сложные, то лучше перейти и делать легкие по коллекциям, а потом уже вернуться обратно к сложным String.**

### Задания Hard
1. Создать метод который будет принимать строку где слитно написано Ваши ИмяФамилия “TungFam" и возвращать строку,  где они будут разделены пробелом
input = “TungFam”
output = “Tung Fam"
Сложность задачи в том, что имя может быть любое. Например:
Введя “ArtemPigor” должно вернуть “Artem Pigor”
Введя “AnnaSecure” должно вернуть “Anna Secure”
Введя “BlaCar” должно вернуть “Bla Car”
То есть алгоритм разбивает два слова которые начинаются на большую букву
2. Создать метод который принимает как аргумент строку. Метод выводит строку зеркально, например Ось -> ьсО, Привет -> тевирП. не используя reverse (сделать алгоритм самому посимвольно)
3. Добавить запятые в строку как их расставляет калькулятор 
1234567 -> 1,234,567
12345 -> 12,345
(не использовать встроенный метод для применения формата)
4. проверить пароль на надежность от 1 до 5
* если пароль содержит числа +1
* символы верхнего регистра +1
* символы нижнего регистра +1
* спец символы +1
* если длина пароля 8 или более символов +1

## Collections
### Задания Easy
1. Создать массив со значениями типа Int. Выполнить удаление всех элементов массива.
2. Создать 2 массива со значениями типа Int. Сделать соединение данных массивов. Результат вывести в консоль.
3. Создать массив с любыми значениями типа строка(во viewDidLoad()). Создать метод который будет принимать как аргумент    массив. Метод должен выводить в консоль элементы массива (по одному в одной строке)

4. Создать массив с любыми значениями типа строка. Создать метод который будет принимать как аргумент массив. Метод должен возвращать массив который состоит из первого и последнего элемента массива, который был параметром
5. Создать словарь в котором ключ будет Строкой а значение Целым. Например ключ - имя, значение - возраст. Должно быть 3 элемента (3 пары).
Добавить в данный словарь еще 2 новых элемента.
6. Создать словарь в котором ключ будет Строкой а значение Целым. Например ключ - имя, значение - возраст. Должно быть 3 элемента (3 пары).
Создать метод который будет иметь 2 параметра: словарь (типа “Строка : Целое”) и ключ типа Строка. Данный метод должен удалить из полученного (как первый аргумент) словаря элемент ключ которого был передан (как второй аргумент).
Например: передаваемый словарь будет такой: 
["Max": 1, "Dasha": 2, "Sergey": 3]
И если передать второй аргумент "Sergey", то метод должен удалить элемент из передаваемого массива с ключом "Sergey".

### Задания Hard
1. Создать метод который принимает 2 аргумента: массив строк и просто строку. Метод возвращает true или false в зависимости есть ли данный элемент (тот второй аргумент, который строка) в массиве (тот первый аргумент, который массив строк). 
например массив
`let array = [“one”, “two”]`
и если передать в этот метод “one“ то должно вернуть true
а если передать “three” то должно вернуть false

2. метод который выведет все ключи словаря и метод который выведет все значения словаря
3. сортировка массива не встроенным методом по возрастанию + удалить дубликаты
Например задается массив [3, 6, 1, 2, 2, 6, 13, 77, 36]
Результат должен быть [1, 2, 3, 6, 13, 36, 77]
4. Во ViewDidLoad создать словарь внутри которого будет 2 словаря (ключ - строка, значение - словарь). С любыми данными. Их мы будем передавать в метод, который напишем. Создать метод который будет принимать как параметры: словарь (такого типа как выше) и строку. Данный метод должен вернуть значение которое хранится внутри элемента ключ которого был передан как аргумент.
