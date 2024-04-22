# Предсказание успешности стартапов.
[Полный отчёт можно почитать в Report.md.](https://github.com/FedorSafonov/Predicting-the-success-of-startups/blob/main/Report.MD)

## Описание

Прогнозирование закрытия стартапов является актуальной задачей в современной экономике, где инновации и предпринимательство играют ключевую роль. Успех стартапа зависит от множества факторов, таких как финансирование, команда, продукт, рынок и внешние условия. Разработка эффективных моделей прогнозирования может помочь снизить риски инвестиций и повысить шансы на успех новых предприятий.

Целью данного исследования является построение модели машинного обучения, способной прогнозировать закрытие стартапов с высокой точностью. В рамках исследования будут идентифицированы ключевые факторы, влияющие на успех или провал стартапов, а также проанализирована эффективность модели на различных временных периодах и для разных категорий стартапов.

Результаты исследования могут быть использованы инвесторами для принятия более обоснованных решений о финансировании стартапов, а также предпринимателями для оценки рисков и повышения шансов на успех. В конечном итоге, это может способствовать развитию инновационной экосистемы за счёт снижения уровня неудачных проектов.

**Вопрос:**
- Прогнозирование закрытия стартапов является важной задачей для инвесторов, предпринимателей и исследователей.
- Существует множество факторов, влияющих на успех или провал стартапа, включая финансирование, команду, продукт, рынок и внешние условия.
- Разработка эффективных моделей прогнозирования может помочь снизить риски инвестиций и повысить шансы на успех новых предприятий.


**Цель исследования:**
- Построить модель машинного обучения, способную прогнозировать закрытие стартапов с высокой точностью.
- Идентифицировать ключевые факторы, влияющие на успех или провал стартапов.
- Проанализировать эффективность модели на различных временных периодах и для разных категорий стартапов.


**Бизнес-задача:**
- Помочь инвесторам принимать более обоснованные решения о финансировании стартапов.
- Предоставить предпринимателям инструменты для оценки рисков и повышения шансов на успех.
- Способствовать развитию инновационной экосистемы за счёт снижения уровня неудачных проектов.

## Результаты

В данном исследовании была разработана модель машинного обучения на основе LightGBM для прогнозирования закрытия стартапов. Модель продемонстрировала высокую эффективность, особенно для стартапов с lifetime более 2 лет, достигнув F1-меры 0.9845.

Анализ важности признаков выявил, что ключевыми факторами, влияющими на успех стартапа, являются устойчивое финансирование, темпы развития, год первого финансирования и регион. Модель оставалась стабильной и надежной на разных временных периодах, что подтверждает её обобщающую способность.

Результаты исследования могут быть использованы инвесторами и предпринимателями для оценки рисков и принятия обоснованных решений. Фокус на стартапах с lifetime более 2 лет делает модель особенно ценной для анализа долгосрочного потенциала.

В качестве направлений для дальнейшей работы можно рассмотреть:
- Создание веб-приложения на Strimlit для комфортного использования
- Использование дополнительных данных, особенно добавление последних актуальных данных (недостающих данных за 2016-2017 год, а так же новых данных после 2018 г.)
- Исследование других моделей машинного обучения и методов ансамблирования.
- Преобразование датасета с дублированием строк долгоживущих стартапов с указанием разного lifetime.
- Рассмотреть задачу как задачу временных рядов ("Сколько проживёт стартап?","Закроется-ли стартап в течении следующих 3-х лет?")

## Статус
- Создание приложения Strimlit.

## Стэк

***pandas, numpy, skimpy, matplotlib, seaborn, sklearn, pycaret, Catboost, LightGBM, XGBoost***