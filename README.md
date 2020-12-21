# Multi-agent-pathfinding
## Запуск
Для запуска необходимо скачать этот репозиторий (или сделать git clone https://github.com/Stepan-Makarenko/Multi-agent-pathfinding.git).  
Для демонстрации работы достаточно выполнить Explore.ipynb.
## Задача
Имеется карта и набор агентов, для каждого из которых определены стартовая и целевая позиции. Задача заключается в нахождении путей для каждого агента так, чтобы избежать столкновений между ними. В результате работы данного алгоритма ищется решение - набор путей для каждого агента.
## Формат входных данных
Для тестирования следует использовать карты и задачи, где будут указаны стартовые и целевые точки агентов, форматов .map и .scen Moving AI.  
Данные (карты и задачи) можно взять отсюда: https://www.movingai.com/benchmarks/mapf.html  
Описание форматов .map и .scen: https://www.movingai.com/benchmarks/formats.html  
Также возможно использование программы для карт, заданных строкой (. - пустая область, # - препятствие), и произвольных агентов, заданных набором (x start, y start, x goal, g goal). 
## Формат выходных данных
Выходные данные - либо набор путей для каждого агента, либо набор путей вместе с отрисовкой агентов, перемещающихся по этим путям (изображение и видео формата .mp4).  
## Работа с произвольными данными
Для карт, заданных строкой, и произвольных агентов, заданных набором (x start, y start, x goal, g goal), можно использовать функцию test из tests.py.
Для файлов movingai можно использовать функцию movingai_test из tests.py.  
С помощью параметров use_pc и diagonal_movements регулируется, используется ли приоритизация конфликтов и допускаются ли перемещения по диагонали.
Примеры выполнения test и movingai_test - в файле Explore.ipynb.
## Примеры работы
![1](media/empty.gif)

![2](media/room.gif)
