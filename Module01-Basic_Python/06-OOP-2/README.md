Домашнее задание к лекции «Объекты и классы. Инкапсуляция, наследование и полиморфизм»
======================================================================================
Привет! Домашняя работа по данной теме является продолжением [задания после лекции «Объекты и классы. Взаимодействие между ними»](https://github.com/AndriusRU/Netology_Tasks/tree/master/Module%2001%20-%20Basic%20Python/06%20OOP-1). Возьмите выполненные работы за основу и продолжите работу над ними. Ссылки на решения могут остаться прежними. Удачи!

Задача №1 "Ферма Дядюшки Джо". Продолжение.
-------------------------------------------
Вы уже реализовали классы животных и определили методы взаимодействия между ними. У всех животных есть общее поведение: каждое животное можно накормить, каждое животное может подать голос. Но есть поведение, принадлежащее только определенным животным. Например, собирать яйца можно только с кур, утки и гусей.

Задание 1:
----------
Вам нужно реализовать родительский класс для всех животных и вынести общее поведение в него.<br/>
От родительского класса должны будут отнаследоваться все остальные животные.<br/>
В родительском классе должно быть 2-3 общих класса и общие поля.<br/>

Задание 2:
----------
Используя методы из родительского класса, вызовите их в цикле у списка всех животных.

Задача №2 "Аудиоколлекция". Продолжение.
----------------------------------------
В первой части задания вы создали 2 альбома с 3 треками и вывели длительность для каждого. Попробуйте получить более подробную информацию о них, опираясь на примеры использования методов в описании заданий:

Задание 1:
----------
Вместо метода `show` использовать магический метод `__str__` у трека для вывода информации по треку.
Пример использования
```python
print(track1)
Bohemian rhapsody-6min
```
У Класса Альбом также реализовать магический метод `__str__` для вывода информации по альбому и его треков. Пример использования
```python
print(my_album)
Name group: Queen
Name album: Bohemian rhapsody
Tracks:
        Bohemian rhapsody-6min
        The show must go on-4min
```
Задание 2:
----------
Реализовать возможность сравнивать треки по длительности. Для этого нужно будет определить магические методы. Пример
```python
track1 = Track('Bohemian rhapsody', 6)
track2 = Track('The show must go on', 4)
track1 > track2
True
```