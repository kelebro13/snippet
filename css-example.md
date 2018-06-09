## Сокрытие текста ##

Паттерн если необходимо скрыть текст (например: заголовок которого нет на макете), но приэтом его видели экранные читалки.
```css
.visually-hidden {
  position: absolute;
  width: 1px;
  height: 1px;
  margin: -1px;
  border: 0;
  padding: 0;
  clip: rect(0 0 0 0);
  overflow: hidden;
}
```
Текст скрытый через `display: none` игнорируется (как будто его нет) экранными читалками.
