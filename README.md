# Модель для принятия решений на фондовой бирже
## Описание файлов:
**Market_research.ipynb** - черновой ноутбук, где проводилось исследование задачи: предобработка данных, выбор оптимальной разметки датасета на основе предложенной моей командой торговой стратегии, выбор модели, настройка её параметров.  

**For_prod.ipynb** - ноутбук с финальной версией кода. Он включает в себя:  
- Функцию для разметки датасета, которая принимает на вход данные, профит (gain, %), который мы ожидаем от заключения сделки по свече, максимальное падение (fall, %). Последние два параметра зависят от конкретного варианта стратегии (семейства стратегий).
- Обученную модель
- Функция, которая принимает параметры предыдущей свечи и составляет из них строку типа DataFrame - в удобоваримом для модели формате.
