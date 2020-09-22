# Метод главных компонент

Еще одно решение проблемы мультиколлинеарности заключается в том,
чтобы подвергнуть исходные признаки некоторому функциональному преобразованию, гарантировав линейную независимость новых признаков, и,
возможно, сократив их количество, то есть уменьшив размерность задачи.


В **методе главных компонент** *(principal component analysis, PCA)* строится
минимальное число новых признаков, по которым исходные признаки восстанавливаются линейным преобразованием с минимальными погрешностями.
PCA относится к методам обучения без учителя (unsupervised learning), поскольку матрица «объекты–признаки» F преобразуется без учета целевого
вектора y.

Важно отметить, что PCA подходит и для регрессии, и для классификации,
и для многих других типов задач анализа данных, как вспомогательное преобразование, позволяющее определить эффективную размерность исходных
данных.

**Постановка задачи.** Рассмотрим матрицу «объектов–признаков»

![фото 1](https://github.com/serega14736/ML/blob/master/формула1.png)

