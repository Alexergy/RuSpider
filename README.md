# RuSpider: Русский датасет SQL-to-Text

## О проекте

**RuSpider** — это открытый русскоязычный датасет для задачи преобразования SQL-запросов в текстовые описания (SQL-to-Text). Создан на основе англоязычного датасета **Spider 1.0** путём перевода вопросов и генерации подробных описаний на русском языке.

## Характеристики датасета
- **Количество примеров**: 8,034
- **Источник**: Spider 1.0
- **Язык вопросов и описаний**: Русский
- **Формат**: JSON

| Набор данных | Количество примеров | Уровни сложности | Форматы |
|--------------|--------------------|-------------------|---------|
| **Train** | 7,000 | easy, medium, hard, extra_hard | JSON, CSV, TXT |
| **Dev** | 1,034 | easy, medium, hard, extra_hard | JSON, CSV, TXT |
| **Всего** | **8,034** | - | - |

## Авторы
- Основной автор Александра С. Носкова, студент ИКНК СПбПУ.
- Научный консультант по базам данных Олег Ю. Сабинин, к.т.н., доцент ВШТИИ СПБПУ

## Лицензия
CC BY-SA 4.0

## Структура репозитория
```yaml
RuSpider/
├── data/
│   ├── train/              # Тренировочные данные
│   │   ├── train.json      # Упрощённая версия
│   │   ├── train_full.json # Полная версия
│   │   ├── train.csv       # CSV
│   │   └── train_examples.txt
│   │
│   └── dev/                # Валидационные данные
│       ├── dev.json
│       ├── dev_full.json
│       ├── dev.csv
│       └── dev_examples.txt
│
├── examples/               # Примеры
├── stats/                  # Статистика
├── README.md
└── LICENSE
```

## Цитирование
Если вы используете **RuSpider** в своих исследованиях, пожалуйста, цитируйте его в следующем формате BibTeX:

```bibtex
@misc{RuSpider-2025,
  title     = {RuSpider: Russian SQL-to-Text Dataset},
  author    = {Noskova, Aleksandra and Sabinin, Oleg},
  year      = {2025},
  publisher = {GitHub},
  howpublished = {\url{https://github.com/Alexergy/RuSpider}}
}
