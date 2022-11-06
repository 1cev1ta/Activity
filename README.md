# Activity #1 Homework

### Задание #1

1. Cоздайте 4 класса Activity и назовите их **ActivityA**-**ActivityD**.
    - В layout файл **ActivityA** добавьте кнопку с текстом “Open ActivityB”
    - В layout файл **ActivityB** добавьте кнопку с текстом “Open ActivityC”
    - В layout файл **ActivityC** добавьте кнопки с текстом “Open ActivityA”, “Open ActivityD”, “Close ActivityC”, “Close Stack”
1. Покрасьте бекграунды Activity: **ActivityA** в `#f44336`, **ActivityB** в `#4caf50,` **ActivityC** в `#2196f3`, **ActivityD** в `#ffeb3b`

    <aside>
    💡 Используйте атрибут `android:background`

    </aside>

2. Подготовьте пустые `onClickListener`’ы для обработки нажатия на кнопки

### Задание #2

1. По клику на кнопку “Open ActivityB” запустите **ActivityB** в отдельном стеке, при этом предусмотрите возможность открывать другие Activity в том же стеке где расположена **ActivityA**

![Untitled](art/Untitled.png)

1. По клику на кнопку “Open ActivityC” запустите **ActivityC** в том же стеке, в котором расположена **ActivityB**

![Untitled](art/Untitled%201.png)

1. По клику на кнопку “Open ActivityA” запустите **ActivityA**, таким образом, чтобы мы попали на существующий экземпляр  **ActivityA** и у него был вызван метод `onNewIntent`, независимо от того находится **ActivityA** наверху своего стека или нет

![Untitled](art/Untitled%202.png)

1. По клику на кнопку “Open ActivityD” запустите **ActivityD** в том же стеке, где расположены **ActivityB** и **ActivityC**, при этом завершите все предыдущие Activity, которые находятся в текущем стеке

![Untitled](art/Untitled%203.png)

1. По клику на кнопку “CloseActivityC”, завершите **ActivityC**, и перейдите на предыдущий экран в стеке

![Untitled](art/Untitled%204.png)

1. По клику на кнопку “Close Stack” завершите текущий стек, в котором находятся **ActivityB** и **ActivityC**, и перейдите на **ActivityA**

![Untitled](art/Untitled%205.png)