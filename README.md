# Лабораторная работа №3 — Извлечение разметки из видео

## Описание

«Воровство разметки» — извлечение bounding box'ов из аннотированного видео,
формирование COCO-датасета и дообучение детектора транспортных средств.

## Структура

```
lab3/
├── lab3.ipynb
├── annotations.xml
├── annotations/
│   ├── coco.json
│   ├── train.coco.json
│   ├── val.coco.json
│   └── test.coco.json
├── frames/
│   ├── input/
│   └── output/
├── input.mp4
├── output.mp4
├── output_result.mp4
├── predictions.mp4
├── best_model.pth
└── README.md
```

## Запуск

1. Открыть `lab3.ipynb` в Jupyter
2. Запустить все ячейки по порядку (`Run All`)
3. Первые две ячейки установят зависимости и скачают файлы автоматически

## Результаты

| Метрика | Значение |
|---|---|
| Лучший метод извлечения | `diff_contours_th15` |
| F1 извлечения | 0.545 |
| Mean IoU извлечения | 0.508 |
| Val mAP (лучшая эпоха 9) | 0.702 |
| Test mAP@0.5 | 0.767 |
| Test mAP@0.5:0.95 | 0.538 |
