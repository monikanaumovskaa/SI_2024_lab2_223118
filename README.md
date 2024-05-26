# Втора лабораториска вежба по Софтверско инженерство
Моника Наумовска 223118

# Control Flow Graph
![Screenshot 2024-05-26 170602](https://github.com/monikanaumovskaa/SI_2024_lab2_223118/assets/129433410/80b7ab8b-1392-4677-87e6-5f012fe3b7ad)


# Цикломатска комплексност
Цикломатската комплекност на овој код изнесува 10, истата ја добив преку формулата Е-Н+2P, каде Е е бројот на ребра (edges) во графот, а N е бројот на јазли (nodes) во графот. Во задачата тие изнесуваат 36-28+2*1=10, соодветно.

# Тест случаи според критериумот Every branch
![Screenshot 2024-05-26 181535](https://github.com/monikanaumovskaa/SI_2024_lab2_223118/assets/129433410/c1ebdaea-855c-4fb0-81bb-3f2ce6eefb2d)


Првиот тест случај е кога листата ни е празна и го фрла исклучокот што пишува "allItems list can't be null".
Вториот тест случај е кога не фрламе исклучок и ги изминуваме сите линии.
Третиот случај е која името на item не е null.
Четвртиот случај е кога баркофот е null и се фрла исклучот "No barcode!".
Петтиот случај е кога во баркодот имаме и карактери и се фрла исклучок "Invalid character in item barcode!".
# Тест случаи според критериумот Multiple conditions
![Screenshot 2024-05-26 183749](https://github.com/monikanaumovskaa/SI_2024_lab2_223118/assets/129433410/ca704f40-06a7-454a-877b-0443a2b30b1a)


Првиот тест случај е кога првиот услов не е исполнет(price<300) и тоа доведува до false statment.
Вториот тест случај е кога првиот услов е исполнет, но вториот не е (discount>0), со тоа доведуваме до false statment.
Третиот тест случај е кога првите два се исполнети, но третиот не е(баркодот да почнува 0), повторно доведува до false statment.
Четвртиот тест случај е ога сите се точни, одведува до true statment.
Објаснување на напишаните unit tests
Првиот тест е наречен testEveryBranch и во него има 5 тест случаи:

Во првиот тест случај користиме RuntimeException ex, каде ex = assertThrows со што потоа ја проверуваме пораката на исклучокот со assertTrue за да се осигураме дека се работи за истиот исклучок.

Во вториот и третиот тест случај креираме List test, каде test ќе биде еднаква на точните одговори кој ги очекуваме како резултат, а за да ги провериме користиме assertTrue.

Во четвртиот и петтиот тест случај користиме RuntimeException ex, каде ex = assertThrows со што потоа ја проверуваме пораката на исклучокот со assertTrue за да се осигураме дека се работи за истиот исклучок, само пораката е различна.

Вториот тест е наречен multipleConditions и во него има 4 тест случаи

Во сите од случаите креираме List test, каде test ќе биде еднаква на точните одговори кој ги очекуваме како резултат, а за да ги провериме користиме assertFalse во првите три случаи, само во последниот assertTrue.