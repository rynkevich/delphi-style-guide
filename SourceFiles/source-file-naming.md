# Исходные файлы

### Именование файлов

Язык программирования Delphi поддерживает длинные названия файлов. Если в имени файла используется несколько слов, следует их выделять с помощью заглавных букв в начале каждого слова: `MyFile.pas`. Такой способ именования известен как InfixCase или [CamelCase](https://ru.wikipedia.org/wiki/CamelCase). Расширения файлов должны быть представлены строчными буквами. По историческим причинам, в названиях исходном коде Delphi часто использовался шаблон именования 8:3, но разработчики программ, в том числе создатели компиляторов языка, уже давно не ограничены этими рамками.

Хорошим тоном является применение префиксной формы именования модулей. Разработчиками из Embarcadero часто используются такие названия, как `uMain.pas` или `uHelp.pas`. Префикс "u" означает "Unit" \("Модуль"\). Допускается использование различных шаблонов имен, однако в рамках одного проекта вид наименований не должен различаться.

При переводе заголовочных файлов языков C/C++ на Delphi их названия, за исключением расширения, изменять не следует. Так, например, `Windows.h` должен быть представлен как `Windows.pas`. Если необходимо объединить несколько заголовочных файлов в один модуль, используется имя модуля-приемника: результат слияние файлов `WinBase.h` и `Windows.h` в последний на языке Delphi должен иметь название `Windows.pas`.
