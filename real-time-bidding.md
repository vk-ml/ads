## Автоматический расчет ставки (Real Time Bidding)

### Задача
**Дано**   
Есть рекламное объявление, про которое известно: 
* признаки **x_ad**
* бюджет на день  **B**
* цель рекламного объяления (показы/клики/конверсии)
* примерное число показов **N**, которые оценил отдельный алгоритм (см. auction-forecasting).

Также дана информация об аукционах, в котором участвовало объявление. Для каждого аукциона известно:
* признаки пользователя **x_user**
* **𝜽** -- вероятность клика пользователя по объявлению (рассчитана отдельной моделью)
* был ли показ, был ли клик


Разработать алгоритм, который для каждого будущего аукциона рассчитывает оптимальную ставку **𝒃** такую, чтобы суммарное число кликов за день по объявлению было максимально и при этом объявление потратило не больше чем заданный бюджет **B**.

### Решения  

* [2020, MoTiAC: Multi-objective Actor-Critics for Real-time Bidding in Display Advertising, Tencent](https://arxiv.org/pdf/2002.07408.pdf)

* [2019, Real-Time Bidding with Soft Actor-Critic Reinforcement Learning in Display Advertising, FRUCT](https://ieeexplore.ieee.org/abstract/document/8981496)

:))))

* [2019, The Second-Price Knapsack Problem: Near-Optimal Real Time Bidding in Internet Advertisement, MIT](https://arxiv.org/pdf/1810.10661.pdf)

Показывают, что задача оптимизации ставки это задача о рюкзаке и приводят около оптимальное решение.

* [2018, Budget Constrained Bidding by Model-free Reinforcement Learning in Display Advertising, CIKM](https://dl.acm.org/doi/pdf/10.1145/3269206.3271748)

Решение задачи выбора ставки в терминах model-free обучения с подкреплением. Топ статья.


* [2017, Real-Time Bidding by Reinforcement Learning in Display Advertising, WSDM](https://dl.acm.org/doi/pdf/10.1145/3018661.3018702)

Решение задачи выбора ставки в терминах обучения с подкреплением.

* [2014, Optimal Real-Time Bidding for Display Advertising, KDD](https://dl.acm.org/doi/pdf/10.1145/2623330.2623633)

Решают задачу оптимизации функционала с условием. Оптимизируют функцию выбора ставки с учетом ограниченного бюджета.
Допускают, что оптимальная функция ставку нелинейна.
Находят оптимальное решение -- оптимальную функцию выбора ставки.
Красивая математическая статья.


* [2013, Real time bid optimization with smooth budget delivery in online advertising, ADKDD](https://dl.acm.org/doi/pdf/10.1145/2501040.2501979)

ормулируют задачу в терминах линейного программирования, решают задачу с помощью алгоритма плавной открутки бюджета объявления в течение дня.

* [2011, Real-time bidding algorithms for performance-based display ad allocation, ACM SIGKDD](https://dl.acm.org/doi/pdf/10.1145/2020408.2020604)

Формулируют задачу в терминах линейного программирования, решают ее и описывают итеративный алгоритм уточнения решения (обновления коэффициентов)

### Другие статьи по теме

* [2019, Bid Optimization by Multivariable Control in Display Advertising, Alibaba, KDD](https://dl.acm.org/doi/pdf/10.1145/3292500.3330681)

* [2018, Real-Time Bidding with Multi-Agent Reinforcement Learning in Display Advertising, Alibaba, CIKM](https://dl.acm.org/doi/pdf/10.1145/3269206.3272021)

* [2018, A Multi-Agent Reinforcement Learning Method for Impression Allocation in Online Display Advertising, Alibaba](https://arxiv.org/pdf/1809.03152.pdf)

* [2018, Optimization of a SSP’s Header Bidding Strategy using Thompson Sampling, KDD](https://dl.acm.org/doi/pdf/10.1145/3219819.3219917)

* [2018, Bidding Machine: Learning to Bid for Directly Optimizing Profits in Display Advertising, IEEE](https://arxiv.org/pdf/1803.02194.pdf)

* [2017, Improving Real-Time Bidding Using a Constrained Markov Decision Process](http://158.64.76.181/bitstream/10993/33478/1/paper9.pdf)


* [2016, Feedback Control of Real-Time Display Advertising, WSDM](https://dl.acm.org/doi/pdf/10.1145/2835776.2835843)


* [2013, Real-time bidding for online advertising: measurement and analysis, UCL, ADKDD](https://dl.acm.org/doi/pdf/10.1145/2501040.2501980)
* [2014, An Empirical Study of Reserve Price Optimisation in Real-Time Bidding](https://dl.acm.org/doi/pdf/10.1145/2623330.2623357)

Красивые графики распределения показов, кликов для объявлкния в течение дня. Какие-то эвристики про ставку через soft, hard floor.

