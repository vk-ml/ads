## Прогнозирование распределения ставок в RTB аукционах

### Задача
**Дано**   
Исторические данные об участии объявлений в аукционах   
Если объявление выиграло аукцион  
* Признаки пользователя 𝒙_𝒖𝒔𝒆𝒓 и объявления 𝒙_𝒂𝒅
* Cтавка 𝑏𝑖𝑑_𝑤𝑖𝑛
* Стоимость показа 𝑧_𝑤𝑖𝑛
Если объявление проиграло аукцион  
* Признаки пользователя 𝒙_𝒖𝒔𝒆𝒓 и объявления 𝒙_𝒂𝒅
* Cтавка 𝑏𝑖𝑑_𝑙𝑜𝑠𝑒

Разработать алгоритм, который для каждого аукциона рассчитывает плотность вероятности выигрыша аукциона со ставкой x.

### Решения
* [2019. Deep Landscape Forecasting for Real-time Bidding Advertising, KDD](https://arxiv.org/pdf/1905.03028.pdf)  
С помощью нейронной сети

* [2016. Functional Bid Landscape Forecasting
for Display Advertising, ECML-PKDD 2016](http://www.saying.ren/slides/functional-bid-lands.pdf)  

* [2011. Bid Landscape Forecasting in Online Ad Exchange Marketplace, KDD](http://www2009.eprints.org/50/1/p491.pdf)  
С помощью градиентного бустинга

* [2009. A Search-Based Method for Forecasting Ad Impression in Contextual Advertising, WWW](http://www2009.eprints.org/50/1/p491.pdf)  
Подбор параметров распределения с помощью статических методов
