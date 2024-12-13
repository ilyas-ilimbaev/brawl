# Изменения в стилях страницы продукта

## Контекст
Страница продукта: [Strong Check Cell](https://brawl.games/products/strong-check-cell)

На странице продукта были выполнены изменения в CSS-стилях, направленные на улучшение пользовательского интерфейса и адаптивности. Этот документ описывает внесенные правки.

---

## Внесенные изменения

### Общие изменения

#### 1. Блок изображений
Для класса `.product__card-info-images` добавлено:
```css
.product__card-info-images {
    overflow: hidden;
}
```

#### 2. Хинт (подсказка)
Для класса `.product__card-hint` изменена высота, а также заданы размеры изображений внутри:
```css
.product__card-hint {
    height: 30px;
}
.product__card-hint img, .product__card-hint picture {
    width: 20px;
    height: 20px;
}
```

### Изменения в блоке перков

#### Удалены свойства:
```css
.product__perks {
    /* padding: 20px 29px; */
    /* overflow: hidden; */
}
```

#### В swiper:
```css
.product__perks .swiper {
    padding: 20px 29px;
    height: 100%;
}
.product__perks .swiper .swiper-slide {
    height: auto;
}
```

#### Для перков:
```css
.product__perk {
    min-width: calc(100% / 4 - 21px);
}
```

### Адаптивность (медиа-запрос @media (max-width: 1200px))

#### Изменения в swiper:
```css
.product__perks .swiper {
    padding: 20px 20px;
}
```

#### Изменения в перках:
```css
.product__perk {
    min-width: calc(100% / 2 - 21px);
}
```

---

## Цели изменений
1. Улучшение адаптивности интерфейса для различных разрешений экрана.
2. Повышение читаемости и удобства взаимодействия пользователей с элементами интерфейса.
3. Оптимизация отображения перков на странице.

---

## Ссылки и ресурсы
- [Ссылка на страницу продукта](https://brawl.games/products/strong-check-cell)
- Ответственные за изменения: [Ilya](https://t.me/ilimbaev_webdev)
- Дата внесения изменений: 13.12.24 7:02

---

Если у вас есть вопросы или предложения, свяжитесь со мной.
