## Хакатон 2023
# Команда Número UNO "Las Teteras Desesperadas"
<h1 align="center">Задача: Автоматизированная обработка сканов документов 

## Состав команды
- Загальский Игорь - Project Manager
- Мишин Илья - Product Manager
- Мурейко Елена
- Иванов Иван
- Санникова Юлия
- Майнгерт Владимир
- Репенко Диана

## <a href="https://miro.com/app/board/uXjVP2DInDc=/?moveToWidget=3458764543238787224&cot=14" target="_blank">Ссылка на Miro</a> 
 
## Идеи реализации задачи:
1) Использование библиотеки Python-Tesseract, которая является оболочкой для Google Tesseract-OCR Engine. 
2) Применение модели CRNN, которая представляет собой комбинацию свёрточной нейронной сети backbone CNN и рекуррентной нейронной сети RNN. 
3) Распознавание с помомощью библиотеки компьютерного зрения OpenCV, которая предназначена для анализа, классификации и обработки изображений; а также библиотеки Pillow, которая является ответвлением Python Imaging Library (PIL) для открытия и обработки изображений во многих форматах. 
 
## Выбранная идея реализации задачи:
Распознавание с помомощью библиотек OpenCV и Pillow.
 
<h2 align="center">Чек-поинт №1.  

#### *1. Подготовить первый вариант программы, выполняющей сегментацию документов на скане.*
Запустить скрипт test1.ipynb 
#### *2. Подготовить примеры работы первого варианта сегментации документов из предоставленного набора данных.*
```
 [         filename   x0   y0   x2   y2       line      label
 0    X00016469619   76   50  133   84        TAN          O
 1    X00016469619  138   50  214   84       WOON          O
 2    X00016469619  219   50  295   84       YANN          O
 3    X00016469619  110  165  156  188      INDAH  S-COMPANY
 4    X00016469619  161  165  198  188       GIFT  S-COMPANY
 ..            ...  ...  ...  ...  ...        ...        ...
 97   X00016469619   62  940  127  958    DEALING          O
 98   X00016469619  132  940  150  958         IN          O
 99   X00016469619  155  940  239  958  WHOLESALE          O
 100  X00016469619  244  940  272  958        AND          O
 101  X00016469619  277  940  342  958    RETAIL.          O
 
 [102 rows x 7 columns], 439, 1004]
```
#### *3. Оценить, какие документы удаётся сегментировать успешно, а при сегментации каких типов документов возникают проблемы. Описать успехи и проблемы сегментации.*
На данном этапе реализации проекта для выбранного набора документов сегментация проходит успешно во всех случаях, с небольшой погрешностью.
