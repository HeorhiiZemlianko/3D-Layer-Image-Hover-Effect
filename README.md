<div align="center">

# 🧊 3D Layer Image Hover Effect

**Эффект наведения на изображение с имитацией 3D-слоёв, построенный на чистом HTML и CSS.**

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)

</div>

---

## 📖 О проекте

Небольшой демонстрационный проект, показывающий, как из **4 статичных изображений**, наложенных друг на друга, можно собрать объёмную композицию. При наведении курсора слои «расходятся» в стороны, создавая эффект глубины.

Проект реализован **без JavaScript, без сборщиков и без библиотек** — только HTML и CSS.

---

## ✨ Что внутри

- 🧊 **Многослойная композиция** — 4 изображения наложены друг на друга
- 🎯 **Hover-эффект** — при наведении слои смещаются и раскрываются
- 🌀 **3D-перспектива** — используется `rotate()` и `skew()` для имитации объёма
- 🎨 **Прозрачность слоёв** — разные уровни `opacity` создают эффект глубины
- ⚡ **Без зависимостей** — чистый HTML + CSS
- 📱 **Простота** — достаточно открыть `3dimaje.html` в браузере

---

## 🚀 Быстрый старт

```bash
# 1. Клонировать репозиторий
git clone https://github.com/HeorhiiZemlianko/3D-Layer-Image-Hover-Effect.git

# 2. Перейти в папку проекта
cd 3D-Layer-Image-Hover-Effect

# 3. Открыть 3dimaje.html в браузере
open 3dimaje.html        # macOS
start 3dimaje.html       # Windows
xdg-open 3dimaje.html    # Linux
```

> Никаких сборок, установок и локальных серверов не требуется.

---

## 📁 Структура проекта

```
3D-Layer-Image-Hover-Effect/
├── 3dimaje.html      # Основная HTML-страница
├── 3dimaje.css       # Стили и 3D-эффекты
├── layer-1.jpg       # Слой 1
├── layer-2.jpg       # Слой 2
├── layer-3.jpg       # Слой 3
├── layer-4.jpg       # Слой 4
└── README.md
```

---

## 🛠️ Технологии

| Технология | Роль |
|------------|------|
| **HTML5** | Разметка страницы и подключение изображений |
| **CSS3** | Позиционирование, `transform`, `transition`, `opacity`, `box-shadow` |

JavaScript **не используется** — вся анимация построена на CSS-переходах.

---

## 🎨 Как это работает

1. **Контейнер** содержит 4 тега `<img>` с одинаковыми размерами.
2. Слои **абсолютно позиционированы** друг поверх друга.
3. Каждому слою задан свой `z-index` и уровень `opacity`.
4. При `:hover` на контейнер срабатывают `transform: translate(...)` и `transition`, которые смещают слои в стороны.
5. Комбинация смещений и прозрачности создаёт **иллюзию 3D-объёма**.

---

## 🎨 Кастомизация

### Замена изображений

Просто положите свои картинки в корень проекта и укажите их в `3dimaje.html`:

```html
<img src="layer-1.jpg" alt="Layer 1">
<img src="layer-2.jpg" alt="Layer 2">
<img src="layer-3.jpg" alt="Layer 3">
<img src="layer-4.jpg" alt="Layer 4">
```

### Изменение эффекта

Открой `3dimaje.css` и настрой:

- `width` / `height` — размер карточки;
- `opacity` — прозрачность каждого слоя;
- `transition` — плавность и длительность анимации;
- `transform: translate(...) rotate(...) skew(...)` — направление и угол смещения слоёв при `:hover`.

---

## 🗺️ Идеи для развития

- [ ] Добавить поддержку любого количества слоёв
- [ ] Сделать реверс-эффект (слои внутрь вместо наружу)
- [ ] Добавить адаптивность под мобильные устройства
- [ ] Добавить переключатель тем (светлая / тёмная)
- [ ] Уважение `prefers-reduced-motion`

---

## 🤝 Contributing

Pull request'ы приветствуются.

1. Форкни репозиторий
2. Создай ветку: `git checkout -b feature/my-feature`
3. Закоммить: `git commit -m "Add my feature"`
4. Запушь: `git push origin feature/my-feature`
5. Открой Pull Request

---

## 📄 Лицензия

Проект распространяется под лицензией **MIT**.
Автор — [Heorhii Zemlianko](https://github.com/HeorhiiZemlianko).

---

<div align="center">

**Сделано с ❤️ на чистом HTML и CSS**

[⬆ Наверх](#-3d-layer-image-hover-effect)

</div>
