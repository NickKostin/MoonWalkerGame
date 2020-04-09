# MoonWalkerGame

## Игра

Игра происходит по ходам. Между ходами возможно получать состояние игры:

1. Информацию о расположении и жизнях всех объектов.
2. Информацию расположении и направлении движения пуль.

## Запуск игры

Для работы игры необходим установленный docker и docker-compose.
Игра распространяется в виде docker-compose файла, содержащего сервисы, необходимые для игры и пример пары ботов.
Для сборки необходимо в консоли перейти в папку, содержащую этот файл и ввести команду `docker-compose up`. Команда произведёт автоматическое скачивание необходимых для игры образов и запустит их с настроенными параметрами.

### Управление игрой

Во время проведения боя действуют следующие горячие клавиши:

`a` - включить/отключить автоматическое проигрывание

`space` - отключить автоматическое проигрывание и перейти на следующий ход

`n` - переключить состояние игры на ход вперед

`b` - переключить состояние игры на ход назад

`lshift+n` - переключить состояние игры на 10 ходов вперед

`lshift+b` - переключить состояние игры на 10 ходов назад

#### Пример JSON состояния игры
```json
{"ContentsInfo":[{"Coordinates":{"X":0,"Y":0},"HealthCount":255,"Type":2},{"Coordinates":{"X":1,"Y":0},"HealthCount":255,"Type":2},{"Coordinates":{"X":2,"Y":0},"HealthCount":1,"Type":1},{"Coordinates":{"X":11,"Y":2},"HealthCount":255,"Type":2},{"Coordinates":{"X":16,"Y":2},"HealthCount":255,"Type":2},{"Coordinates":{"X":21,"Y":2},"HealthCount":255,"Type":2},{"Coordinates":{"X":0,"Y":3},"HealthCount":255,"Type":2},{"Coordinates":{"X":7,"Y":3},"HealthCount":2,"Type":1},{"Coordinates":{"X":11,"Y":3},"HealthCount":255,"Type":2},{"Coordinates":{"X":20,"Y":3},"HealthCount":3,"Type":0,"UserId":"r1"},{"Coordinates":{"X":21,"Y":3},"HealthCount":255,"Type":2},{"Coordinates":{"X":0,"Y":4},"HealthCount":255,"Type":2},{"Coordinates":{"X":1,"Y":4},"HealthCount":255,"Type":2},{"Coordinates":{"X":5,"Y":4},"HealthCount":1,"Type":1},{"Coordinates":{"X":10,"Y":4},"HealthCount":255,"Type":2},{"Coordinates":{"X":11,"Y":4},"HealthCount":255,"Type":2},{"Coordinates":{"X":14,"Y":4},"HealthCount":1,"Type":1},{"Coordinates":{"X":21,"Y":4},"HealthCount":255,"Type":2},{"Coordinates":{"X":0,"Y":5},"HealthCount":255,"Type":2},{"Coordinates":{"X":1,"Y":5},"HealthCount":255,"Type":2},{"Coordinates":{"X":2,"Y":5},"HealthCount":255,"Type":2},{"Coordinates":{"X":11,"Y":5},"HealthCount":255,"Type":2},{"Coordinates":{"X":20,"Y":5},"HealthCount":255,"Type":2},{"Coordinates":{"X":21,"Y":5},"HealthCount":255,"Type":2},{"Coordinates":{"X":0,"Y":6},"HealthCount":255,"Type":2},{"Coordinates":{"X":1,"Y":6},"HealthCount":255,"Type":2},{"Coordinates":{"X":2,"Y":6},"HealthCount":255,"Type":2},{"Coordinates":{"X":7,"Y":6},"HealthCount":255,"Type":3},{"Coordinates":{"X":8,"Y":6},"HealthCount":255,"Type":3},{"Coordinates":{"X":9,"Y":6},"HealthCount":255,"Type":3},{"Coordinates":{"X":19,"Y":6},"HealthCount":255,"Type":2},{"Coordinates":{"X":20,"Y":6},"HealthCount":255,"Type":2},{"Coordinates":{"X":21,"Y":6},"HealthCount":255,"Type":2},{"Coordinates":{"X":0,"Y":7},"HealthCount":255,"Type":2},{"Coordinates":{"X":1,"Y":7},"HealthCount":255,"Type":2},{"Coordinates":{"X":8,"Y":7},"HealthCount":255,"Type":3},{"Coordinates":{"X":9,"Y":7},"HealthCount":255,"Type":3},{"Coordinates":{"X":16,"Y":7},"HealthCount":1,"Type":1},{"Coordinates":{"X":19,"Y":7},"HealthCount":255,"Type":2},{"Coordinates":{"X":20,"Y":7},"HealthCount":255,"Type":2},{"Coordinates":{"X":21,"Y":7},"HealthCount":255,"Type":2},{"Coordinates":{"X":0,"Y":8},"HealthCount":255,"Type":2},{"Coordinates":{"X":3,"Y":8},"HealthCount":1,"Type":1},{"Coordinates":{"X":9,"Y":8},"HealthCount":255,"Type":3},{"Coordinates":{"X":17,"Y":8},"HealthCount":2,"Type":1},{"Coordinates":{"X":20,"Y":8},"HealthCount":255,"Type":2},{"Coordinates":{"X":21,"Y":8},"HealthCount":255,"Type":2},{"Coordinates":{"X":0,"Y":9},"HealthCount":255,"Type":2},{"Coordinates":{"X":13,"Y":9},"HealthCount":255,"Type":2},{"Coordinates":{"X":14,"Y":9},"HealthCount":255,"Type":2},{"Coordinates":{"X":21,"Y":9},"HealthCount":255,"Type":2},{"Coordinates":{"X":0,"Y":10},"HealthCount":255,"Type":2},{"Coordinates":{"X":5,"Y":10},"HealthCount":255,"Type":2},{"Coordinates":{"X":7,"Y":10},"HealthCount":2,"Type":1},{"Coordinates":{"X":13,"Y":10},"HealthCount":255,"Type":2},{"Coordinates":{"X":14,"Y":10},"HealthCount":255,"Type":2},{"Coordinates":{"X":15,"Y":10},"HealthCount":255,"Type":2},{"Coordinates":{"X":21,"Y":10},"HealthCount":255,"Type":2},{"Coordinates":{"X":0,"Y":11},"HealthCount":255,"Type":2},{"Coordinates":{"X":5,"Y":11},"HealthCount":255,"Type":2},{"Coordinates":{"X":6,"Y":11},"HealthCount":255,"Type":2},{"Coordinates":{"X":15,"Y":11},"HealthCount":255,"Type":2},{"Coordinates":{"X":16,"Y":11},"HealthCount":255,"Type":2},{"Coordinates":{"X":18,"Y":11},"HealthCount":255,"Type":2},{"Coordinates":{"X":21,"Y":11},"HealthCount":255,"Type":2},{"Coordinates":{"X":0,"Y":12},"HealthCount":255,"Type":2},{"Coordinates":{"X":1,"Y":12},"HealthCount":3,"Type":0,"UserId":"r2"},{"Coordinates":{"X":4,"Y":12},"HealthCount":255,"Type":2},{"Coordinates":{"X":5,"Y":12},"HealthCount":255,"Type":2},{"Coordinates":{"X":6,"Y":12},"HealthCount":255,"Type":2},{"Coordinates":{"X":7,"Y":12},"HealthCount":255,"Type":2},{"Coordinates":{"X":16,"Y":12},"HealthCount":255,"Type":2},{"Coordinates":{"X":17,"Y":12},"HealthCount":255,"Type":2},{"Coordinates":{"X":18,"Y":12},"HealthCount":255,"Type":2},{"Coordinates":{"X":19,"Y":12},"HealthCount":255,"Type":2},{"Coordinates":{"X":20,"Y":12},"HealthCount":255,"Type":2},{"Coordinates":{"X":21,"Y":12},"HealthCount":255,"Type":2},{"Coordinates":{"X":0,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":1,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":2,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":3,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":4,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":5,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":6,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":7,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":8,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":9,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":10,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":11,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":12,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":13,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":14,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":15,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":16,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":17,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":18,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":19,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":20,"Y":13},"HealthCount":255,"Type":2},{"Coordinates":{"X":21,"Y":13},"HealthCount":255,"Type":2}],"BulletsInfo":[{"Coordinates":{"X":17,"Y":3},"Direction":2,"OwnerId":"r1"}],"ZoneRadius":94}
```

Примеры JSON хода игрока

```json
[{"Type":1,"Direction":3}]
```
```json
[{"Type":0,"Direction":0}]
```
