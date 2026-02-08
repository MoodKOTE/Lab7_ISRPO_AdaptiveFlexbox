# Лабораторная работа №7: Адаптивная верстка с использованием Flexbox

## 📌 Описание
Лабораторная работа посвящена изучению и применению CSS-технологии Flexbox для создания адаптивных веб-интерфейсов.

## 🎯 Цели и задачи
- Освоить основные концепции Flexbox.
- Научиться создавать гибкие и адаптивные макеты.
- Практиковаться в использовании Git и GitHub для контроля версий.
- Сверстать навигационное меню, карточки товаров и центрированный блок с помощью Flexbox.

## 🛠 Используемые технологии
- HTML5
- CSS3 (Flexbox)
- Git, GitHub
- Visual Studio Code, Live Server

## 📂 Структура проекта

### Корневая папка проекта: Lab7_Adaptive_FIO
- index.html
- styles.css Flexbox
- flexbox.htmlFlexbox
- flexbox.css         
- README.md          
### Подкаталоги:

- img/
  - gitPushLab7_FIO.png
  - flex-direction_row_Lab7_FIO.png
  - flex-direction_column_Lab7_FIO.png
  - flex-direction_row-reverse_Lab7_FIO.png
  - flex-direction_column-reverse_Lab7_FIO.png
  - align-items_stretch_Lab7_FIO.png
  - align-items_flex-start_Lab7_FIO.png
  - align-items_flex-end_Lab7_FIO.png
  - align-items_center_Lab7_FIO.png
  - align-items_baseline_Lab7_FIO.png
  - flex-wrap_nowrap_Lab7_FIO.png
  - flex-wrap_wrap_Lab7_FIO.png
  - flex-wrap_wrap-reverse_Lab7_FIO.png
  - gap_Lab7_FIO.png
  - flex-grow_100_Lab7_FIO.png
  - flex-grow_350_Lab7_FIO.png
  - flexbox_html_Lab7_FIO.png
  - add_flexbox_Lab7_FIO.png
  - add_flexbox_cards_Lab7_FIO.png
  - add_flexbox_card_Lab7_FIO.png
  - flexbox_card_flex-start_Lab7_FIO.png
  - flexbox_centered-content_Lab7_FIO.png
  - flexbox_practice_Lab7_FIO.png

## Пример 1: Базовый Flex-контейнер
HTML:
```html
<div class="container">
  <div class="item">1</div>
  <div class="item">2</div>
  <div class="item">3</div>
</div>
```
```css
.container {
  display: flex;
  flex-direction: row;
  gap: 10px;
  padding: 20px;
  border: 2px solid #333;
}

.item {
  background-color: lightblue;
  padding: 20px;
  text-align: center;
  flex: 1;
}
```
## Пример 2: Навигационное меню
HTML:
```html
<nav class="navbar">
  <a href="#">Главная</a>
  <a href="#">О нас</a>
  <a href="#">Услуги</a>
  <a href="#">Контакты</a>
</nav>
```
CSS:
```css
.navbar {
  display: flex;
  justify-content: space-around;
  background-color: #333;
  padding: 15px;
}

.navbar a {
  color: white;
  text-decoration: none;
  padding: 10px 20px;
}

.navbar a:hover {
  background-color: #555;
}
```
## Пример 3: Карточки товаров
HTML:
```html
<section class="cards">
  <div class="card">
    <h3>Товар 1</h3>
    <p>Описание товара</p>
    <button>Купить</button>
  </div>
  <div class="card">
    <h3>Товар 2</h3>
    <p>Описание товара</p>
    <button>Купить</button>
  </div>
  <div class="card">
    <h3>Товар 3</h3>
    <p>Описание товара</p>
    <button>Купить</button>
  </div>
</section>
```
CSS:
```css
.cards {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
}

.card {
  flex: 1 1 250px;
  border: 1px solid #ccc;
  padding: 20px;
  border-radius: 10px;
  display: flex;
  flex-direction: column;
}

.card button {
  margin-top: auto;
  padding: 10px;
  background-color: #007bff;
  color: white;
  border: none;
  cursor: pointer;
}

.card button:hover {
  background-color: #0056b3;
}
```
## Пример 4: Центрирование элемента
HTML:
```html
<div class="centered-container">
  <div class="centered-content">
    Я в центре!
  </div>
</div>
```
CSS:
```css
.centered-container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 300px;
  border: 2px dashed #333;
}

.centered-content {
  padding: 40px;
  background-color: lightgreen;
  border-radius: 10px;
}
```
## Пример 5: Разные значения flex-direction
CSS:
```css
/* Строка (по умолчанию) */
.container-row { flex-direction: row; }

/* Строка справа налево */
.container-row-reverse { flex-direction: row-reverse; }

/* Колонка */
.container-column { flex-direction: column; }

/* Колонка снизу вверх */
.container-column-reverse { flex-direction: column-reverse; }
```
## Пример 6: Выравнивание (align-items)
```css
.container {
  display: flex;
  height: 200px;
  border: 2px solid #333;
}

/* Растянуть */
.stretch { align-items: stretch; }

/* В начале */
.flex-start { align-items: flex-start; }

/* В конце */
.flex-end { align-items: flex-end; }

/* По центру */
.center { align-items: center; }

/* По базовой линии текста */
.baseline { align-items: baseline; }
```

## Пример 7: Перенос элементов (flex-wrap)
```css
/* Без переноса */
.nowrap { flex-wrap: nowrap; }

/* С переносом */
.wrap { flex-wrap: wrap; }

/* Обратный перенос */
.wrap-reverse { flex-wrap: wrap-reverse; }
```
## Полные файлы проекта:
index.html — базовая страница с примерами Flexbox

styles.css — стили для базовых примеров

flexbox.html — страница с навигацией, карточками и центрированием

flexbox.css — стили для практических примеров

Автор: Lepilkin Maxim
Группа: ISP-232
