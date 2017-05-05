# Исходные файлы

### Организация файлов

Все модули, используемые в проектах среды программирования Delphi, должны содержать следующие элементы в указанном порядке:

1. Копирайт, идентификационный комментарий.
2. Название модуля.
3. Раздел интерфейса.
4. Раздел реализации.
5. Признак конца модуля `end.`.

Данные элементы должны быть разделены как минимум одной пустой строкой.

Порядок расположение остальных элементов остается на усмотрение разработчика, однако в начале файла должен находиться комментарий с копирайтом, затем - название модуля и условные определения, директивы компилятора, подключения файлов и список подключений:

```Pascal
{*******************************************************}
{                                                       }
{       Borland Delphi Visual Component Library         }
{                                                       }
{       Copyright (c) 1995,98 Inprise Corporation       }
{                                                       }
{*******************************************************}

unit Buttons;

{$S-,W-,R-}
{$C PRELOAD}

interface

uses 
  Windows, Messages, Classes, 
  Controls, Forms, Graphics, 
  StdCtrls, ExtCtrls, CommCtrl;
```

В исходном коде продуктов компании Embarcadero используется следующий идентификационный комментарий:

```Pascal
//---------------------------------------------------------------------------

// This software is Copyright (c) 2017 Embarcadero Technologies, Inc.
// You may only use this software if you are an authorized licensee
// of Delphi, C++Builder or RAD Studio (Embarcadero Products).
// This software is considered a Redistributable as defined under
// the software license agreement that comes with the Embarcadero Products
// and is subject to that software license agreement.

//---------------------------------------------------------------------------
```

Не имеет значения, располагается ли раздел описаний типов перед списком констант, порядок их представления может изменяться по усмотрению разработчика.

Раздел реализации требуется начинать с ключевого слова `implementation`. За ним должен следовать список подключений. Далее могут находиться любые подключения или директивы компилятора языка:

```Pascal
implementation

uses 
  Consts, SysUtils, ActnList, 
  ImgList;

{$R BUTTONS.RES}
```



