# Лучший результат на public

## Результаты

- **Лучший сид (seed):** 0042
- **Лучший Validation Dice:** 0.9197 (эпоха 62)
- **Лучший Validation IoU:** 0.8638 (эпоха 79)

## Модель

- **Архитектура:** UnetPlusPlus
- **Энкодер:** timm-efficientnet-b3
- **Предобучение:** ImageNet

## Обучение

Мы обучили модель сегментации на трех различных сидах (2026, 9999, 0042) для оценки стабильности обучения. Лучшие результаты показал сид **0042**.

**Параметры обучения:**
- Эпох: 85
- Размер батча: 4
- Размер изображения: 512x512
- Оптимизатор: AdamW (LR=3e-4, Weight Decay=1e-4)
- Функция потерь: Combined Loss (BCE + Dice)
- Планировщик LR: ReduceLROnPlateau
- Аугментация: HorizontalFlip, VerticalFlip, RandomRotate90

## Веса моделей:

https://vk.com/away.php?to=https%3A%2F%2Fdrive.google.com%2Fdrive%2Ffolders%2F1-cLjAVSxjW8YMljtZmT4kwbDoRuz7l6Q%3Fusp%3Ddrive_link&utf=1

## Таблицы с метриками по эпохам

*Будут добавлены после загрузки на Kaggle*

## Графики обучения

*Будут добавлены после загрузки на Kaggle*
