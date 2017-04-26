# Калькулятор

| свойство |          тип          |                                описание                               |
|----------|-----------------------|-----------------------------------------------------------------------|
| visible  | * bool                | Свойсво, определяющее отображается ли компонент.                      |
| value    | * string/number       | Текущее значение калькулятора.                                        |
| onChange | * func                | Возникает каждный раз, когда значение калькулятора изменяется.         |
| onClose  | * func                | Возникает при нажатии на кнопку "OK" или при нажатии вне калькулятора. |
| position | top/bottom/left/right | Позиция относительно родительского элемента.                          |

## Кнопка калькулятора

| свойство |   тип   |                        описание                        |
|----------|---------|--------------------------------------------------------|
| text     | string  | Текст кнопки.                                          |
| icon     | object  | Иконка, отображаемая перед текстом.                    |
| style    | object  | Inline-стиль, применяемый к корневому элементу кнопки. |
| onClick  | func    | Событие возникаемое при нажатии на кнопку.             |
| red      | bool    | Если true, то кнопка будет красного цвета.             |
| menu     | element | Элемент меню, отображаемый внутри кнопки.              |
| disabled | bool    | Если true, то кнопка будет отключена.                  |

## Поле ввода калькулятора

|       свойство      |       тип       |                                                           описание                                                           |
|---------------------|-----------------|------------------------------------------------------------------------------------------------------------------------------|
| value               | * string/number | Текущее значение калькулятора.                                                                                               |
| onChange            | * func          | Возникает при изменении значения в поле ввода. Значение изменяется при условии, что оно удовлетворяет определенному условию. |
| isExpression        | bool            | Если true, то поле ввода работает в режиме ввода выражений.                                                                  |
| onOperationKeyPress | func            | Возникает при ввода операции.                                                                                                |
| onRemoveKeyPress    | func            | Возникает при нажатии клавиши Backspace.                                                                                     |
| onPercentsKeyPress  | func            | Возникает при нажатии клавиши с процентами.                                                                                  |
| onInputCleared      | func            | Возникает если была запрошена очистка поля ввода и поле было очищено (введено новое значение).                               |
| onMenuToggleClick   | func            | Возникает при нажатии на кнопку справа от поля ввода.                                                                        |
| clearInputRequired  | bool            | Запрос сброса значения в поле. Если true, то следующее введенное число очистить предыдущее значение.                         |
| menu                | element         | Элемент меню, который будет передан ниже в кнопку.                                                                           |