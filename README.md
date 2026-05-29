# Modern CSS Tooltip with Dynamic Anchor Positioning

A lightweight, high-performance, and 100% pure CSS tooltip implementation that leverages modern web standards.

## Key Features

* **CSS Anchor Positioning:** Zero-JavaScript layout positioning that anchors the tooltip precisely to trigger elements using `position: fixed`.
* **Native Try-Tactics:** Leverages built-in `flip-block` and `flip-inline` browser fallbacks to dynamically reposition the tooltip on viewport overflow.
* **Cross-Browser Corner Arrows:** Uses standard CSS border intersections and `background-clip: padding-box` to render sharp 45-degree corner arrows with perfect compatibility.
* **Dynamic Masking:** Utilizes a `clip-path: inset(0px) margin-box` mask driven by native margin-swapping to automatically hide irrelevant arrows based on active layout positioning.
* **Symmetric Transitions:** Smooth, animatable hover transitions driven by flipped margins that automatically adjust their slide-in direction on flip.

## Setup

Simply link `style.css` in your HTML and add the `data-tooltip` attribute to any triggering element:

```html
<link rel="stylesheet" href="./style.css">

<button data-tooltip="This is a dynamic tooltip!">Hover me</button>
```

## Styling Customization

Adjust the tooltip properties dynamically by updating the CSS variables:

```css
[data-tooltip] {
    --arrow-size: 11.3px; /* Controls both the arrow size and 45-degree diagonal proportions */
}
```
