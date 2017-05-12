# Выражения и конструкции

### Конструкция case

Существует несколько корректных способов оформления конструкции `case`. Выбор между ними может осуществляться в зависимости от таких факторов, как, к примеру, длина выражений конструкции и уровень ее вложенности.

Примеры оформления конструкции `case`:

```Pascal
// ПРАВИЛЬНО:
case Control.Align of
  alLeft, alNone: NewRange := Max(NewRange, Position);
  alRight: Inc(AlignMargin, Control.Width);
end;

// ПРАВИЛЬНО:
case X of

  csStart:
    begin
      J := UpdateValue;
    end;

  csBegin: X := J;

  csTimeOut:
    begin
      J := X;
      X := UpdateValue;
    end;

end;

// ПРАВИЛЬНО:
case ScrollCode of
  SB_LINEUP, SB_LINEDOWN:
    begin
      Incr := FIncrement div FLineDiv;
      FinalIncr := FIncrement mod FLineDiv;
      Count := FLineDiv;
    end;
  SB_PAGEUP, SB_PAGEDOWN:
    begin
      Incr := FPageIncrement;
      FinalIncr := Incr mod FPageDiv;
      Incr := Incr div FPageDiv;
      Count := FPageDiv;
    end;
else
  Count := 0;
  Incr := 0;
  FinalIncr := 0;
end;
```



