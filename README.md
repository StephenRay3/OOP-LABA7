Часть 1
Программу, разработанную в лабораторной работе No 6, преобразовать
следующим образом: для обеспечения движения геометрических фигур в окне
вместо таймера использовать потоки. Для каждой геометрической фигуры
использовать свой поток. Потоковая функция должна быть одна, объект
«Фигура» передается в потоковую функцию через параметр (для передачи
дополнительных данных в потоковую функцию в качестве параметра можно
задать указатель на структуру). При необходимости использовать
синхронизацию.
Часть 2
Необходимо обеспечить синхронизацию двух приложений.
Первое приложение. Приложение с потоками преобразовать так, чтобы
движение фигур в потоках начиналось не сразу, а после получения сигнала от
второго приложения. При получения сигнала потоки начинают работать до тех
пор, пока от второго приложения не придет другой сигнал, при получении
второго сигнала потоки завершают свою работу.
Второе приложение – консольное приложение Windows (запускается
только при запущенном первом приложении). После нажатия клавиши
посылается сигнал для начала работы потоков в первом приложении. После
следующего нажатия клавиши посылается сигнал на завершение работы потоков
в первом приложении.
Продемонстрировать совместную работу двух приложений.

Алгоритм
1. Создаем массив базового класса Figure в Windows приложении
2. Заполняем массив классами наследниками и задаем им свои параметры в Windows приложении
3. Ожидание нажатия клавиши в консольном приложении
3. Вход в цикл i в Windows приложении
4. Рисуем фигуру i в Windows приложении
5. Меняем координаты фигуры i в Windows приложении
6. Рисуем фигуру i в Windows приложении
7. Если нажата клавиша в консольном приложении, то остановить прориросовку фигур
8. Если нажата клавиша еще раз в консольном приложении, то остановить программу
9. Иначе возвращаемся к шагу 3
Часть 2 (Ссылка на видео https://1drv.ms/v/s!AgLRl5i9yERW3S2rr7cJLjUvyWOp?e=LaYptC
