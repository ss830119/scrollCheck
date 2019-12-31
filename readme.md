# ScrollCheck
Demo: [https://codepen.io/ss830119/pen/rNaGWZd?editors=0010](https://codepen.io/ss830119/pen/rNaGWZd?editors=0010)

## Getting Started
```
<script src="https://unpkg.com/aos@next/dist/aos.js"></script>
```

## Usage

```html
<div class="section">
  <p>A</p>
</div>
<div class="section">
  <p>B</p>
</div>
<div class="section">
  <p>C</p>
</div>
<div class="section">
  <p>D</p>
</div>
```
```js
var page = new scrollCheck({
  classname: 'section',
  repeat: true
})
page.init()
```

