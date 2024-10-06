# primoExample

# Для запуска необходимо снабдить робота стартовыми данными, такие как дата запуска и список компаний
# Успешный запуск предполагает наличие файлов в корневой директории
-RunDate.txt
********Содержит дату запуска в формате dd.MM.yyyy
-CompanyData.txt
********Содержит список компаний, которые будут обработаны
-ResultData.txt
********Содержит шаблон для консолидируемых данных
********Результат работы формируется накопительным итогом

# Работа с датой 
Дата, с которой данные файла являются неполными и требуют получения дополнительных данных с ресурса 
по умолчанию берутся из листа компании файла ResultData.xlsx из столбца A последней строки.
Если по какой то компании сбор данных делается впервые, создается лист компании для сбора данных, на 
основе шаблона, дата с которой необходимо собрать данные берется из файла RunDate.txt, пример:
Дата в файле 30.09.2024
Данные будут собираться с временного среза 30.09.2024 00:00:00
