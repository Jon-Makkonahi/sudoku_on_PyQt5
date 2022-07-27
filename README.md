# sudoku_on_PyQt5

### Авторы:
- Daniil Bibikov (Jon-Makkonahi) https://github.com/Jon-Makkonahi

### Приложение «Судоку» 
выполнено в традиционном ключе, присущем обычным Windowsприложениям. 
Ее окно (рис. 32.2) включает в себя главное меню, панель инструментов, 
основное содержимое — поле судоку и набор кнопок для установки цифр в ячейки, и строку состояния.

В самом поле судоку группы ячеек выделены различными цветами фона: оранжевым
и светло-серым. Установленные в них цифры выводятся черным цветом.

Одна из ячеек является активной — именно с активной ячейкой осуществляется взаимодействие. 
Активная ячейка закрашена желтым цветом.
Чтобы сделать какую-либо ячейку активной, следует:

 * либо, пользуясь клавишами-стрелками, переместить на нее желтый фокус выделения;
 * либо просто щелкнуть на ней мышью.

Чтобы установить в активную ячейку какую-либо цифру, следует:

 * либо нажать соответствующую кнопку в наборе, расположенном ниже поля;
 * либо нажать соответствующую цифровую клавишу.

Чтобы убрать цифру из активной ячейки, нужно:
 * либо нажать кнопку Х, что находится в расположенном под полем наборе;
 * либо нажать клавишу пробела, <Backspace> или <Del>

Чтобы случайно не занести в какую-либо ячейку другую цифру, есть возможность заблокировать ее. 
Для этого следует сделать нужную ячейку активной и нажать клавишу <F2>.
В заблокированной ячейке цифра выводится красным шрифтом.
Отметим, что блокировать можно только ячейки, содержащие цифры.
Снять блокировку с ячейки можно, сделав ее активной и нажав клавишу <F4>. 
  
Главное меню приложения содержит следующие пункты:
* меню Файл:
** Новый (с ним связана комбинация клавиш <Ctrl>+<N>) — очистка поля;
** Открыть (<Ctrl>+<O>) — загрузка сохраненной ранее головоломки из выбранного
пользователем файла;
** Сохранить (<Ctrl>+<S>) — сохранение головоломки в файле с указанным пользователем именем.
При выборе этого пункта производится сохранение в полном формате, т. е. для каждой ячейки, помимо находящейся в ней цифры, сохраняется признак того, заблокирована ли она;
** Сохранить компактно — сохранение головоломки в файле в компактном формате.
Компактный формат не предусматривает хранения признака блокировки ячейки.
Вследствие этого файл, сохраненный в компактном формате, вдвое меньше полноформатного.
При открытии файла, сохраненного в компактном формате, производится автоматическая блокировка всех ячеек, содержащих цифры;
** Печать (<Ctrl>+<P>) — вывод головоломки на печать;
** Предварительный просмотр — просмотр головоломки в том виде, в котором она
будет выведена на печать;
** Параметры страницы — настройка параметров печатаемой страницы;
** Выход (<Ctrl>+<Q>) — завершение работы приложения;
* меню Правка:
** Копировать (<Ctrl>+<C>) — копирование головоломки в буфер обмена в полном
формате (аналогичном тому, в котором сохраняется файл при выборе пункта Сохранить меню Файл);
** Копировать компактно — копирование головоломки в буфер обмена в компактном
формате (аналогичном тому, в котором сохраняется файл при выборе пункта Сохранить компактно меню Файл);
** Копировать для Excel — копирование головоломки в буфер обмена в формате,
предназначенном для вставки в таблицу Microsoft Excel;
** Вставить (<Ctrl>+<V>) — вставка головоломки, скопированной ранее в любом формате.
Если головоломка была скопирована в компактном формате, все ячейки, содержащие
цифры, будут автоматически заблокированы;
** Вставить из Excel — вставка из буфера обмена головоломки, скопированной из таблицы Microsoft Excel;
** Блокировать (<F2>) — блокировка активной ячейки;
