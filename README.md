## Цели анализа:

Данный анализ был проведен на основе данных, которое были взята из [Dominick’s dataset](https://www.chicagobooth.edu/research/kilts/research-data/dominicks).

Необходимо прогнозировать спрос на товар или категорию товаров.

**1. Провести исследовательский анализ данных (EDA), чтобы:**

* Понять структуру данных.

* Найти возможные зависимости спроса от параметров, включая сезонность, тренды и другие факторы.

**2. Построить модель(и) прогноза спроса:**

* Необходимо попробовать несколько способов прогноза(бустинг, AutoML,  etc.).

* Выбор моделей должен быть обоснован.

**3. Выделить зависимость спроса от цены и построить кривые эластичности:**

### Файловая структура:

* **data**- папка, содержащая в себе данные для анализа:

        beer_sales_data.parquet - продажи пива

        cig_sales_data.parquet - продажи сигарет

        ana_sales_data.parquet - продажи анальгетиков

        demographic_data.parquet - данные демографии и магазина

        beer_upc.parquet - таблица с описанием товара пиво 

        cig_upc.parquet - таблица с описанием товара сигареты

        ana_upc.parquet - таблица с описанием товара анальгетики

### Описание таблиц:        

**1. Tables sales:** 

        upc - Universal Product Code.

        store - store number.

        week - week number.

        move - number of unit sold.

        price - retail price.

        qty - number of item bundled together.

        sale - sale code(B, C, S). This variable indicates whether the product was sold on a promotion that week. A code of 'B' indicates a Bonus Buy, 'C' indicates a coupon, 'S' indicates a simple price reduction.

**2. Tables upc:**

        com_node - not important. 

        upc - Universal Product Code.

        descrip - product name.

        size - product size.

        case - not important.

        nitem - number of items in a case.

**3. Tables demographic:**

        store - store number.

        age60 - % population over age 60.

        age9 - % population under age 9.

        educ - % college graduates.

        ethnic - % blacks and hispanics.

        income - log of median income.

        hhlarge - % of households with 5 or more persons.

        workwom - % working women with full-time jobs.

        hval150 -  % of households with value over $150,000.

        sstrdist - distance to the nearest warehouse store.

        sstrvol - ration of sales of this store to the nearest warehouse store.

        cpdist5 - average distance in miles to the nearest 5 supermarkets.

        cpwvol5 - ration of sales of this store to the average of the nearest five stores.        

___

### Результаты:

**1. Описательный EDA:**

**2. Модели, их сравнение и интерпритация:**

**3. Анализ эластичности и графики зависимости спроса от цены:**

_Rabov A.A_