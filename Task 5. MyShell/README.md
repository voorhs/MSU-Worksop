# Задание 5.1
1. программа должна выполнять чтение строк (со стандартного ввода или из файла) **в цикле**. В каждой строке необходимо выделить и напечатать столбиком отдельные слова. При этом:
- любое количество идущих подряд пробельных символов обрабатывается так же, как один пробел. 
- текст, заключенный в двойные кавычки, рассматривается как одно слово или часть слова, то есть, внутри двойных кавычек пробельные символы рассматриваются как обычные символы. *Например:*
```
вход>    aaa "bbb ccc" ddd
результат:     aaa
             bbb ccc
             ddd

вход>    aaaa    "bbb"ccc"ddd" eee
результат:     aaaa
             bbbcccddd
             eee
```

2. допускаются строки произвольной длины, то есть, программа должна вести себя корректно вне зависимости от того, какой длины строка подана на ввод (!). 
3. программа завершает работу в ситуации "конец файла" на стандартном вводе (или в файле). Обработка конца файла должна быть реализована корректно.
4. как отдельные слова выделяются управляющие символы myshell, которые также выполняют роль разделителей слов (не требуют вокруг себя пробелов):
```
&, &&, |, ||, ;, >, >>, <, (, ) .
```

5. Требование к коду: после считывания очередной строки должен быть сформирован массив строк (слов) или список полученных слов, и только после этого слова должны выводиться на экран, чтобы продемонстрировать корректную работу.