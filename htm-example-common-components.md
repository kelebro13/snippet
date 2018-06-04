### Пагинация и "Хлебные крошки"
Пример пагинации:
```html
<ul class="pagination__list">
  <li class="pagination__item"><a href="#">1</a></li>
  <li class="pagination__item pagination__item--current"><a>2</a></li>
  <li class="pagination__item"><a href="#">3</a></li>
  <li class="pagination__item"><a href="#">4</a></li>
</ul>
```
Пример "хлебных крошек"
```html
<ul class="breadcrumbs">
  <li class="breadcrumbs__item"><a href="index.html">Главная</a></li>
  <li class="breadcrumbs__item"><a href="catalog.html">Магазин</a></li>
  <li class="breadcrumbs__item breadcrumbs__item--current">Средства для ухода</li>
</ul>
```

**Обратим внимание** что в пагинации текущая страница (`pagination__item--current`) обернута в `a` без атрибута `href`,
а в "хлебных крошках" нет. Это из-за того что в пагинации выделенная страница всегда может стать не выделенным элементом и должна будет
вести на новую страницу (добавится `href`). А в "хлебных крошках" последний элемент никогда не станет ссылкой.

