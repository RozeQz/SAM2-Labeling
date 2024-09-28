# SAM2-Labeling

Данный репозиторий используется для улучшения разметки датасета PKLot. Однако, такие же манипуляции можно применить к любым другим картинкам, где bbox'ы плохо расставлены.

## Структура

- В `images` лежат оригиналы картинок.
- В `labels` лежит разметка этих картинок в формате `class_id x_center y_center box_width box_height`.
- В `new_labels` лежит улучшенная разметка картинок в формате `class_id x_center y_center box_width box_height`.
- В `segmented` лежат автосегментированные SAM2 картинки.
- В `segmented_with_bboxes` лежат сегментированные картинки с использованием промпта в виде bbox'ов для SAM2.
- В `segmented_with_points` лежат сегментированные картинки с использованием промпта в виде центров bbox'ов для SAM2.
- В `segmented_with_both` лежат сегментированные картинки с использованием промпта в виде bbox'ов и их центров для SAM2.
- В `new_boxes` лежат картинки с новыми размечеными bboxes.

## Настройка окружения

### Linux

```bash
python3 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt
```

### Windows
```bash
python -m venv venv
.\venv\Scripts\activate
pip install -r requirements.txt
```
