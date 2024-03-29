[![](https://img.shields.io/badge/python-3.7.0-green)](https://img.shields.io/badge/python-3.7.0-green)
[![](https://img.shields.io/badge/pygame-2.1.2-yellowgreen)](https://img.shields.io/badge/pygame-2.1.2-yellowgreen)

# Conway`s Game of life на Python

### Правила
- Каждая клетка может находиться в одном из двух состояний: живая (заполненная) или мёртвая (пустая).
- Каждый ход у каждой клетки определяется ее состояние и состояние всех её 8-ми соседей.
- Если это пустая клетка и соседей ровно 3, то эта клетка оживает. Во всех остальных случаях пустая клетка остается пустой.
- Если же это живая клетка, то подсчитывается количество живых соседей.
- Если соседей 0 или 1, то клетка умирает от одиночества.
- Если соседей 2 или 3, то клетка продолжает жить.
- Если соседей 4 или больше, то клетка умирает от перенаселения.

### Структура проекта
1. Создаем сетку
2. Пишем функцию определения кол-ва соседей:
    - Создаем систему соседства `system`
    - Создаем переменную счетчик `count`
    - Проходимся по каждому элементу системы
    - Если сосед клетки по системе "живой", увеличиваем `counter`
    - Возвращаем `count`
3. Создаем основную логику, см. выше `Правила`
