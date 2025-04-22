## Transfer Learning с ResNet

## Описание

В этом задании вы научитесь применять **transfer learning** — обучение с переносом — с использованием предобученной нейросети **ResNet** для задачи классификации изображений. Вы можете выбрать один из предложенных датасетов:

- 🍎 [Fruit and Vegetable Recogniser](https://www.kaggle.com/datasets/kritikseth/fruit-and-vegetable-image-recognition)
- 🦋 [Butterfly Classification](https://www.kaggle.com/datasets/gpiosenka/butterfly-images40-species/data)

## 📝 Задание

1. Выберите и скачайте один из датасетов (через Kaggle).
2. Подготовьте данные для обучения и валидации, используя `torchvision.datasets.ImageFolder` или свою загрузку.
3. Используйте `tensorflow.keras.applications.resnet50` или `MobileNetV2` с предобученными весами.
4. Замените финальный `fc`-слой, чтобы он соответствовал числу классов.
5. Заморозьте все веса кроме классификатора и дообучите только его.
6. Затем разморозьте всю модель и дообучите заново.
7. Постройте графики:
   - Точности и функции потерь (loss) на обучении и валидации
   - Несколько предсказаний (с изображениями и метками)
8. Сделайте выводы об эффективности переноса обучения.

## Полезные материалы

- Официальная документация `torchvision.models` (предобученные модели):  
  https://pytorch.org/vision/stable/models.html

- Transfer Learning в PyTorch (официальный туториал):  
  https://pytorch.org/tutorials/beginner/transfer_learning_tutorial.html

- Использование `ImageFolder`:  
  https://pytorch.org/vision/stable/generated/torchvision.datasets.ImageFolder.html

- Как работать с `DataLoader`:  
  https://pytorch.org/docs/stable/data.html

- Визуализация изображений в PyTorch:  
  https://pytorch.org/tutorials/beginner/data_loading_tutorial.html#visualize-a-few-images

- Основы ResNet (статья на русском):  
  https://habr.com/ru/articles/436210/
