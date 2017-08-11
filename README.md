# Header-Generator
Генератор заголовков.
Автор: David Vox

1. Вопросы
2. Программа для откладки кода

## 1. Вопросы:
	
Как добавить категорию?

	1) Добавить в $catName название категории таким образом, чтобы ключ названия категории и условия совпадал.
	2) Условия добавляются в $conditions.
	
Как добавить категорию-исключение?

	1) Добавить в $exceptArr название исключаемой категории.
	2) Добавить условия исключаемого в $conditions, не нарушая последовательность. Исключения добавляются последними.

## 2. Программа для откладки:

1) Поместить между условными операторами в цикле while:


 	``` echo "<b> Проверка данных:", "<br>", "</b>";
	echo $numIdArr, "Ключ массива IdArr", "<br>";
	echo $id_arr[$numIdArr], "Значение idArr с ключом $numIdArr", "<br>";
	echo $numCheck, "Проверочный ключ", "<br>";
	echo $conditions_arr[0], "-conditions_arr[0]", "<br>";
	echo $conditions_arr[1], "-conditions_arr[1]", "<br>"; 
	```

2) Поместить в любую часть программы, но после объявления массивов:

        
	``` echo "<b>Проверка массивов: ", "<br>";
	echo "Количество $id_arr", $id, "<br>", "Count=", count($id_arr), "<br>";
	echo "Массив conditions=", print_r($conditions), "<br>";
	echo "Массив catName=", print_r($catName), "<br>";
	echo "Массив catArch=", print_r($catArch), "<br>";
	echo "Массив exceptArr=", print_r($exceptArr), "<br>", "</b>"; 
	```
        
	
3) Поместить после строки "$catArch[$id_arr[$numIdArr]] = $catName[$numIdArr];":

	```
	echo "Найден и добавлен: ", $catName[$numIdArr], "<br>";  	
	```
	
	
