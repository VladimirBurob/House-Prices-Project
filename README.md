## Группа 1 "ValueError Team"
[Владимир Буробин](https://github.com/VladimirBurob) ——
[Максим Сафарян](https://github.com/safsafsaf187) ——
[Зиярат Гаджиева](https://github.com/Ziiarat)

<img src="https://github.com/VladimirBurob/House-Prices-Project/blob/d7e0cff75555d17e88285b682750bc55d119da97/ValueError.jpg" width="500">

<br/>

### Репозиторий с предсказанием цен на недвижимость (ML-project)

### Обработка дата сета
Загрузка train.csv и test.csv и объединение в один датасет через concat для анализа полных данных в столбцах-признаках
На основании числовых столбцов выстроили heatmap график корреляции величин с таргет величиной SalePrice
На основании графика удалили признаки с корр >|0.3|

Так же на основании графика удалили 3-4 взаимозаменяемые признака на основании хитмепа 
(были убраны признаки с высокой корреляцией к таргету и друг другу (больше 0.60))

Анализ проспусков данных и выявление кол-ва уникальных значений в столбцах
для выстроения логики заполнения пропусков, метода кодирования каждого признака и удаления неинформативных столбцов


### Возвращаемся к исходному train/test файлам и переходим к созданию пайплайна, который представляет из себя cлед структуру
<br/>
-удаление столбцов<br/>
-заполняем пропуски<br/>
-скалируем/кодируем (стандарт скейлер числовые признаки, таргет/уанхот/лейб енкодинг для соотв. объектных признаков) <br/>
-применение различных моделей для расчета таргета и MSLE <br/>


### Резюме
Выбор лучшей модели на основе результатов
Буст модели через optuna
Анализ влияния способа енкондинга столбцов и выявление идеального набора признаков для удаления и targetencoder

### 🚀 ValueError 🚀
