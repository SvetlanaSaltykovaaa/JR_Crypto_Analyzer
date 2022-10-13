# CryptoAnalyzerProject
Encoder/Decoder of english text
Итоговая программа должна быть собрана в формате jar (Сборку пока игнорируйте, на лекции потом покажем как. Можете вносить параметры в Run configuraiton > program arguments)
Запуск программы происходит со следующими параметрами

operation filePath key - именно в таком порядке. То есть вызова самой программы будет выглядеть как "java -jar myApp.jar operation filePath key"

filepath - путь к файлу, который кодируется
operation - три доступных варианта: encode/decode/bruteForce
key - целое число


в случае передачи encode/decode key обязателен

Результатом работы программы в папке с исходным файлом должен появиться файл с тем же именем что и входой файл, но с пометкой (encoded/decoded) в зависимости от выполненной операции
Содержимое файла должно быть закодировано\декодировано используя Алгоритм Цезаря. Кодируются только буквы английского алфавита(большие и маленькие), остальные символы остаются неизменными

Программа должна использовать один и тот же ключ для корректного кодирования и декодирования файла

Код программы и готовый собранный файл jar выложить на GitHub

примеры исопльзования:
java -jar myApp.jar encode folder/textFile1.txt 20   // результат файл folder/textFile1(encoded).txt
java -jar myApp.jar decode folder/textFile1(encoded).txt 20   // результат файл folder/textFile1(decoded).txt  

ДОПОЛНИТЕЛЬНО

в случае передачи bruteForce key не обязателен, вместо него передается ссылка на файл для статистического анализа кода
operation filePath filePathForstaticAnalisis
Добавить к имени файла значение найденого ключа

примеры исопльзования:
java -jar myApp.jar bruteForce folder/textFile1.txt folder/textExample.txt   // результат файл folder/textFile1(decoded key-20).txt


ДОПОЛНИТЕЛЬНО 2
добавить поддержку кодирования текста на русском языке

ДОПОЛНИТЛЕЬНО 3 
GUI (Swing, JavaFX)
