
# Классификация эмоций по аудио и тексту

![image](https://github.com/user-attachments/assets/fc6605f1-05b5-4ca9-9e73-fae73f1dfeaa)

## Описание проекта

Этот репозиторий содержит реализацию системы **бинарной классификации эмоций** с использованием признаков из аудио и текста. Цель проекта — определить, является ли речь **нейтральной** или **не нейтральной** по эмоциональной окраске.

В работе применяются различные подходы: от базовой логистической регрессии до мультимодальной нейросети. Каждый из этапов оформлен в отдельном Jupyter Notebook.

---

## Описание ноутбуков

| Файл              | Описание                                                                 |
|-------------------|--------------------------------------------------------------------------|
| `baseline.ipynb`  | Простая модель логистической регрессии на объединённых признаках.        |
| `NN.ipynb`        | Полносвязная нейросеть (MLP), обучающаяся на объединённом векторе.       |
| `concat.ipynb`    | Мультимодальная модель: отдельная обработка аудио и текста, затем слияние.|

---


## Что реализовано

- Загрузка и обработка текстовых и аудиопризнаков
- Классификация с помощью:
  - Логистической регрессии (baseline)
  - Нейросети с одним входом
  - Мультимодальной нейросети с двумя входами (текст и аудио)
- Метрики качества:
  - Accuracy
  - F1-score
  - Матрица ошибок

