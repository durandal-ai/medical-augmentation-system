# medical-augmentation-system
Medical data augmentation system that can be deployed fast and easy to use for doctors
"""
# Инструкция по использованию

Этот Jupyter Notebook предназначен для запуска в Google Colab Pro на GPU A100 и содержит
систему аугментации медицинских изображений с разрешением 128x128 с использованием DCGAN, DDPM и StyleGAN.

## Настройка окружения
1. Загрузите этот notebook в Google Colab
2. Выберите Runtime -> Change runtime type -> Hardware accelerator: GPU (A100)
3. Выполните все ячейки последовательно

## Параметры обучения
- DCGAN: 30 эпох
- DDPM: 15 эпох, 1000 шагов диффузии
- StyleGAN: 30 эпох
Для лучших результатов увеличьте количество эпох (например, до 50-100).

## Ограничение набора данных
По умолчанию ограничение отключено (`use_limited_dataset = False`). Если нужно ограничить, установите `use_limited_dataset = True` и задайте `limit_size`.

## Сохранение результатов
Результаты сохраняются в /content/drive/MyDrive/med_image_augmentation/

## Интерфейс Gradio
После обучения запускается веб-интерфейс для генерации изображений с выбором модели.
"""
