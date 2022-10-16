# FileAnalyser 

* Функциональность: настоящее приложение позволяет обработать файл и в качестве результата предоставить информацию о наименовании файла, 
количестве строк, количестве всех символов, статистику по каждому из символов (сколько раз встречается в тексте), топ N популярных символов. 
В приложении реализовано API. 

* Логика работы приложения: 
1. С помощью команды imports (http://localhost:8080/imports) в программу загружается путь к файлу, который необходимо проанализировать. Результат 
работы приложения будет выведен на экран, а также сохранен внутри приложения.
2. С помощью команды getSummary (http://localhost:8080/getSummary) указывается путь к файлу, в котором необходимо сохранить результат.

* Пример результата работы приложения, если файл будет содержать строку "Hello!":

fileName: input.txt
rowsCount: 1
totalSymbols: 6
symbolsStatistics: {'H': 1, 'e': 1, 'l': 2, 'o': 1}
top3PopularSymbols: 'l', 'H', 'e'