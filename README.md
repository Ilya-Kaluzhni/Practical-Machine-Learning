# Practical-Machine-Learning

Недавно решил перебрать все свои файлы гугл коллаба, время от времени буду сюда загружать файлы.

## Содержание
1. [Классификация морских животных](#классификация-морских-животных)
2. [Практика по основам TensorFlow](#практика-по-основам-tensorFlow- (в двух частях))
3. [Распознавание_автомобильных_номеров](#распознаваниез-автомобильных-номеров)

## Классификация морских животных
В данной работе выполняется аугментация изображений и обучение модели нейронной сети для классификации изображений с применением библиотек Keras, TensorFlow, pandas и matplotlib. В ходе работы были достигнуты следующие результаты:

1. Проведена настройка трансформации изображений с использованием ImageDataGenerator для увеличения набора данных.
2. Подготовлены и загружены исходные изображения из Google Drive.
3. Сгенерированы новые изображения посредством аугментации и сохранены в директорию.
4. Проведена классификация изображений с созданием и обучением сверточной нейронной сети.
5. Осуществлена подготовка данных, включая разметку и разделение на обучающую и проверочную выборки.
6. Обучена модель нейронной сети, настроены обратные вызовы для улучшения процесса обучения.
7. Визуализированы результаты обучения и предсказания на тестовых данных.

*****

## Практика по основам TensorFlow (в двух частях)
В этом файле демонстрируются основные возможности и операции TensorFlow, включая работу с различными типами данных, тензорами, использование GPU, создание и использование графов, работу с сессиями и визуализацию с помощью TensorBoard. Основные моменты включают:

1. Типы данных: Объявление постоянных (Constant), переменных (Variable) и контейнеров для данных (Placeholder).
2. Основные операции с тензорами: Сложение, умножение, возведение в квадрат и суммирование элементов.
3. Совместимость с NumPy: Преобразование данных между NumPy и TensorFlow.
4. Использование GPU: Определение доступных устройств и запуск вычислений на GPU.
5. Работа с датасетами: Создание и обработка данных с использованием tf.data.Dataset.
6. Сессии и графы: Запуск вычислений в сессиях, создание и использование графов, управление переменными.
7. Визуализация с TensorBoard: Создание графиков и визуализация обучения модели.
8. Код включает комментарии и примеры для каждой функциональности, что делает его хорошим руководством для изучения TensorFlow.

*****

## Распознавание_автомобильных_номеров
Данный скрипт предназначен для автоматического извлечения и распознавания текстовой информации с номерных знаков транспортных средств на изображениях. Система использует методы компьютерного зрения для идентификации и обработки изображений номерных знаков, а также технологию OCR (Optical Character Recognition) для преобразования изображения текста в машинно-читаемый формат.
1. С помощью инструментов из библиотеки OpenCV производится загрузка изображения автомобиля.
2. С помощью каскада Хаара, специально обученного для обнаружения номерных знаков, система определяет координаты прямоугольников, содержащих номера.
3. На основе координат прямоугольников с номерами извлекается часть изображения, содержащая номер. Также производится её увеличение для провышения качества распознавания.
4. Извлеченное изображение номерного знака конвертируется в оттенки серого, что упрощает последующее распознавание текста.
5. Используется библиотека Tesseract OCR для преобразования изображения номерного знака в текст. Параметры конфигурации Tesseract настроены для распознавания букв и цифр.

*****
