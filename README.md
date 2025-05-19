# Länkar:

- [Länk till presentationen](https://docs.google.com/presentation/d/17dd9Lq799zny2WnH6SpToA0RiJuXvi_Jcjn_55oUIBw/edit?usp=sharing)
- [CSS Flexbox Layout Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [Länk till övningar (fokusera på de sista om responsivitet och Media Queries)](https://docs.google.com/document/d/1_bWuo8l6KtyQi0JEvq3d2Sh_C8kiG2nONl9r4sHcA1s/edit?usp=sharing)

# 📦 Flexbox – snabbguide

Flexbox används för att enkelt skapa flexibla och responsiva layouter i CSS. Aktiveras med:

```css
display: flex;
```

## 🔁 Riktning (`flex-direction`)

| Värde        | Beskrivning             |
|--------------|--------------------------|
| `row`        | Horisontell, vänster → höger *(default)* |
| `row-reverse`| Horisontell, höger → vänster |
| `column`     | Vertikal, uppifrån → ner |
| `column-reverse` | Vertikal, nerifrån → upp |

## 📏 Justera längs main-axeln (`justify-content`)

| Värde             | Effekt |
|-------------------|--------|
| `flex-start`      | Placera till början |
| `flex-end`        | Placera till slutet |
| `center`          | Centrera |
| `space-between`   | Jämnt mellanrum, inget i kanterna |
| `space-around`    | Jämnt runt varje item, halvt i kanter |
| `space-evenly`    | Exakt jämnt mellanrum överallt |

## 🪜 Justera längs korsaxeln (`align-items`)

| Värde        | Effekt |
|--------------|--------|
| `stretch`    | Sträck till full höjd/bredd *(default)* |
| `flex-start` | Placera i början (toppen) |
| `center`     | Centrera vertikalt |
| `flex-end`   | Placera längst ner |

## 🔧 Flex-wrap

| Värde     | Beskrivning                |
|-----------|----------------------------|
| `nowrap`  | Allt på en rad *(default)* |
| `wrap`    | Bryt rader vid behov       |

## 🧱 På enskilda items (`flex-grow`, `flex-shrink`, `flex-basis`)

```css
.item {
  flex: 1 1 200px; /* grow shrink basis */
}
```

## 🔢 Sortering

```css
.item {
  order: 2;
}
```

---

## 🔎 Exempel

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
  justify-content: space-between;
  align-items: center;
}
```
