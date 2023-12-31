# HSE_Perm_tasks
Задание - на основе видеопотока с камер создать программный модуль, который определяет фотографию дня участка сварки, требуется отслеживать работу по каждой камере и собирать данные о работе участка сварки.

Для обучения модели глубокого обучения на задачу многоклассовой классификации видео или фоторяда вам понадобится следующий пайплайн: 
 
1. Предварительная обработка данных: Вначале необходимо предобработать видеоряд или видеофайлы, чтобы привести их к нужному формату для обучения модели. Это может включать в себя изменение разрешения видео, выделение определенных областей интереса, приведение к определенному формату фотографий и т.д. 
 
2. Извлечение признаков: После предварительной обработки данных вы можете использовать различные методы извлечения признаков, такие как кадры (для видео) или пиксели (для фотографий), чтобы представить данные в числовом формате. Это может включать в себя методы компьютерного зрения (CV) для обнаружения объектов, определения движения и т.д. 
 
3. Обучение модели: Затем можно обучить модель глубокого обучения, такую как сверточная нейронная сеть (CNN) или рекуррентная нейронная сеть (RNN), на извлеченных признаках. Вы можете использовать различные архитектуры нейронных сетей для этой задачи и настроить их параметры для достижения наилучших результатов. 
 
4. Оценка и валидация: После обучения модели необходимо оценить ее производительность, используя метрики, такие как точность, полнота и F-мера, и валидацию на тестовом наборе данных, чтобы убедиться в ее способности обобщения. 
 
Теперь давайте сравним пайплайн для обучения на видеоряде и фоторяде: 
 
Обучение на видеоряде: 
1. Предварительная обработка: Извлечь кадры из видео и предобработать их для извлечения признаков. 
2. Извлечение признаков: Использовать кадры для извлечения признаков, таких как текстуры, цвета, объекты и т.д. 
3. Обучение модели: Обучить модель на извлеченных признаках, возможно, используя методы дополнения данных и оптимизации гиперпараметров. 
 
Обучение на фоторяде: 
1. Предварительная обработка: Подготовить фотографии для обучения модели, возможно, изменить размеры и формат изображений. 
2. Извлечение признаков: Использовать фотографии для извлечения признаков, таких как гистограммы интенсивности, локальные бинарные шаблоны и т.д. 
3. Обучение модели: Обучить модель на извлеченных признаках, возможно, используя методы дополнения данных и оптимизации гиперпараметров. 
 
Сравнительный анализ: 
При сравнении обучения на видеоряде и фоторяде следует учитывать сложность предварительной обработки, объем данных, вычислительные ресурсы, а также качество и точность предсказаний. Обучение на видеоряде может быть более сложным из-за большего объема данных и временной последовательности, однако это может привести к более точным предсказаниям, особенно при анализе движения или динамических процессов. Обучение на фоторяде может быть более простым, но может потребовать большего количества примеров для обучения и может не захватить динамику процесса так хорошо, как видеоряд. 
 
Выбор между обучением на видеоряде и фоторяде зависит от специфики задачи, доступных ресурсов и требуемой точности предсказаний.

Наш тизер:
Мы представляем модель для автоматического определения статуса работников на рабочем месте, работник может быть занят полезной работой, может вынужденной работой, а может тратить рабочее время впустую. Компании требуется автоматизировать собственные ресурсы, тратящиеся на производство машин, поэтому можно использовать искусственный интеллект, создав программный модуль, который будет на основе видеопотока с камер на каждом участке сварки отслеживать состояние работы. Наше решение может помочь определять моменты простоев на определённом участке. Модель поможет классифицировать изображения с участка, разделив их на вынужденную работу, полезную работу, простои. Стек решения: Python, OpenCV, PyTorch, ResNet и YOLO.

Уникальность нашего решения в том, что мы используем предобученную модель, что повышает точность классификации.
