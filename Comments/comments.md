# Комментарии

### Общая информация

В языке Delphi существует два вида комментариев: однострочные и многострочные. Вот несколько полезных советов относительно их использования:

* Полезно использовать комментарии в начале модуля для указания его назначения;
* Комментарии можно использовать для описания класса перед его объявлением;
* Комментарии можно использовать для описания методов класса перед их объявлением;
* Не стоит пояснять очевидные вещи:

```Pascal
Counter := Counter + 1;    // Увеличить Counter на единицу
```

* Код с ложной информацией в комментариях гораздо хуже кода без комментариев;
* Не стоит указывать информацию, которая может быстро потерять актуальность;
* Различного рода "украшения" в комментариях не приветствуются;
* Временные комментарии должны быть помечены специальным тэгом `???:`. Впоследствии это поможет быстрее их найти. Наличие временных комментариев в коде готовой программы - признак плохого стиля.

Пример:

```Pascal
// ???: Изменить строку с вызовом MySort после исправления
List.MySort;
```


