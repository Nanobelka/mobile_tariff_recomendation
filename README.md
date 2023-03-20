# [Модель для рекомендации тарифа мобильного оператора](https://nbviewer.jupyter.org/github/Nanobelka/Yandex_Praktikum/blob/main/mobile_tariff_recomendation/mobile_tariff_recomendation.ipynb)
## На основании ряда характеристик порекомендовать клиенту архивного тарифа наиболее подходящий действующий тариф

**Заказчик:** некий мобильный оператор.

**Входные данные:** данные о поведении клиентов, использующих определенные тарифы; предобработка уже выполнена.

**Цель проекта:** построить модель, способную проанализировать поведение пользователей архивных тарифов и предложить один из действующих тарифов — «Смарт» или «Ультра».

**Задачи проекта:**

- построить модель для задачи классификации, которая выберет подходящий тариф;
- для оценки качества модели использовать метрику **accuracy**;
- минимально приемлемое значение **accuracy = 0.75**;
- дать рекомендации по дальнейшему развитию данного проекта.

## Содержание
        
0  Начальная подготовка

    0.1  Импорты
    0.2  Вспомогательные функции
    0.3  Вспомогательные элементы для оформления
    0.4  Настройки

1  Чтение и проверка входных данных

    1.1  Чтение данных
    1.2  Первичная информация о данных
    1.3  Распределение признаков для пользователей разных тарифов
        1.3.1  Графики распределений
        1.3.2  Статистики распределений
    1.4  Корреляция признаков с целевой переменной
    1.5  Попарные распределения признаков
        
2  Подготовка данных для моделей

    2.1  Выделение признаков и целевой переменной
    2.2  Разделение на обучающую и тестовую выборки
        
3  Обучение моделей

    3.1  Подготовка пайплайнов моделей
    3.2  Подготовка сеток гиперпараметров
    3.3  Объединение всех данных о моделях в датафрейм
    3.4  Случайный поиск по сетке гиперпараметров
    3.5  Проверка моделей на тестовой выборке
        
4  Анализ лучшей модели

    4.1  Функция для визуализации важности признаков
    4.2  RandomForestClassifier
        4.2.1  Обучение модели с лучшей комбинацией гиперпараметров
        4.2.2  Визуализация важности признаков
    4.3  ExtraTreesClassifier
        4.3.1  Обучение модели с лучшей комбинацией гиперпараметров
        4.3.2  Визуализация важности признаков
            
5  Вывод

    5.1  Краткий обзор проведенной работы
    5.2  Результаты анализа
    5.3  Рекомендации и риски
