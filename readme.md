# 📘 Модуль 4.1: Декоративні елементи

## 🗂 План заняття

- 🖼 Контентні та декоративні зображення  
- 🎨 Властивості: `background-color`, `background-image`, `background-repeat`, `background-position`, `background-size`  
- 🧅 Багатошаровий фон  
- 🌈 Градієнти: лінійний, радіальний  
- 🕶 CSS-тіні та властивість `box-shadow`  
- 📐 Векторна графіка (SVG)  
- ✏️ Основи SVG-фігур  
- 🧩 Способи використання SVG  
- 🧰 Створення та робота з SVG-спрайтом  
- 🧙‍♀️ Псевдоелементи `::before` та `::after`  

---

## 🖼 Властивість `background-image`

### 🔁 background-repeat

- `repeat` — повторювати X і Y. Значення за замовчуванням.  
- `repeat-x` — повторювати тільки X (горизонтально).  
- `repeat-y` — повторювати тільки Y (вертикально).  
- `no-repeat` — не повторювати.

### 📍 background-position

- `x y`  
- `50% 50%`  
- `100px 200px`  
- `right bottom`  
- `left top`

### 📏 background-size

- `auto auto`  
- `200px`  
- `200px 300px`  
- `cover` — масштабувати, щоб покрити весь елемент  
- `contain` — масштабувати, щоб вмістити зображення всередину елемента

---

## 🧅 Багатошаровий фон

Приклад:  
`background-image: url(шлях до зображення 1), url(шлях до зображення 2);`

---

## 🌈 Градієнти

### 🔄 Лінійний градієнт

Синтаксис:  
`background-image: linear-gradient(<напрямок>, <колір-1>, <колір-2>, ...)`

Приклад з фоном:  
`background-image: linear-gradient(to top, rgba(17, 17, 17, 0.4), rgba(17, 17, 17, 0.4)), url("path_to_image");`

### 🎯 Радіальний градієнт

Приклад:  
`background-image: radial-gradient(rgba(17, 17, 17, 0.3), rgba(17, 17, 17, 1)), url("path_to_image");`

---

## 🧰 background (скорочена форма)

Приклад:  
`background: url(шлях до зображення) repeat-x;`

---

## 🕶 Властивість `box-shadow`

Синтаксис:  
`box-shadow: <x-offset> <y-offset> <blur> <spread> <color>;`

Можна додати `inset` для внутрішньої тіні:  
`box-shadow: inset <x-offset> <y-offset> <blur> <spread> <color>;`

### 🔳 Багатошарова тінь

Приклад:  
`box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1), 0px 6px 20px rgba(0, 0, 0, 0.1);`

🔗 Приклади: [getcssscan.com/css-box-shadow-examples](https://getcssscan.com/css-box-shadow-examples)

---

## 📐 Векторна графіка

- Вбудований SVG (`inline`)
- Властивість `fill` — визначає колір заливки
- Властивість `stroke` — визначає колір рамок

---

## 🧰 SVG-спрайт

- Генерація через: [icomoon.io/app](https://icomoon.io/app/)
- Оптимізація SVG: [svgomg.net](https://svgomg.net/)

- Приклад написання HTML для додавання svg за допомогою спрайту
-   `<svg class="class-name" width="24" height="24">`
        `<use href="./sprite.svg#icon-instagram"></use>`
    `</svg>`

---

## 📍 Позиціонування

- `position`: `static` | `relative` | `absolute` | `fixed` | `sticky`  
- `z-index`

---

## 🎬 CSS-переходи

- `transition-property`: `<властивість>` | `color`, `background-color`  
- `transition-duration`: `<час>` | `2s` | `0.5s` | `2000ms` | `500ms`  
- `transition-timing-function`: `<функція розподілу часу>` | `ease`, `linear`, `ease-in`, `ease-out`, `ease-in-out`  
- `transition-delay`: `<затримка>`

- `transition`: `[property] [duration] [timing-function] [delay]`  
- `transition`: `background-color 500ms linear, transform 500ms ease-in-out;`

### Властивість `transition-timing-function`

- `ease` — перехід починається повільно, швидко прискорюється, а потім знову сповільнюється в кінці.  
- `linear` — перехід має рівномірну швидкість.  
- `ease-in` — починається повільно, швидкість переходу збільшується до повного завершення переходу.  
- `ease-out` — починається швидко, уповільнюється протягом переходу.  
- `ease-in-out` — починається повільно, прискорюється, а потім знову сповільнюється.

---

## 🌀 2D-трансформації

- `transform`: `none` | `<тип трансформації>` `<тип трансформації>` ...  
- `transform: scale(1.15)` — маштабування  
- `transform: rotate(45deg)` — прокручування  
- `transform: translate(100px, 200px)` — зміщення  
- `transform: translate(-50%, -50%)` — центрування елемента  
- `transform: skew(30deg)` — викривлення

---

## 🧙‍♀️ Псевдоелементи

Використання:  
`.box::before`, `.box::after`, `.box:hover::before`

---

