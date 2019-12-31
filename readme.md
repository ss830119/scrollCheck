# ScrollCheck
Demo: 
<a href="https://codepen.io/ss830119/pen/rNaGWZd?editors=0010" target="_blank">https://codepen.io/ss830119/pen/rNaGWZd?editors=0010</a>

## Getting Started
```html
<script src="https://ss830119.github.io/assets/scrollCheck.js"></script>
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
  classname: 'section', // object classname
  repeat: true // scroll animation
})
page.init() // after all setting or feature
```
### use class `active` to add animation
```css
.section {
  height: 100vh;
  background: #ccc;
  border-bottom: 1px solid #aaa;
  transition-duration: 1s;
}
.section.active {
  background: #666;
  color: #fff;
  transition-duration: 1s;
}
```

## feature
### setPoint
`setPoint()` set before `init()`
```js
scrollCheck.setPoint({
  id: 'totop', // element
  stay: 1,  // 'active' class appear which interval
  repeat: true  // repeat or once, 'false' is default
  range: 2 // toggle 'active' range
})
```