```html
<div class="container">
  <!-- .container>.item.item--$*6 -->
  <div class="item item--1">1: Orange</div>
  <div class="item item--2">2: Green</div>
  <div class="item item--3">3: Violet</div>
  <div class="item item--4">4: Pink</div>
  <div class="item item--5">5: Blue</div>
  <div class="item item--6">6: Brown</div>
</div>
```

```css
.container {
  background-color: #eee;
  width: 1000px;
  margin: 30px auto;

  display: grid;
  grid-template-rows: 150px 150px;
  grid-template-columns: 150px 150px 150px;

  // grid-row-gap: 30px;
  // grid-column-gap: 30px;
  grid-gap: 30px;

  .item {
    padding: 20px;
    font-size: 20px;
    font-family: sans-serif;
    color: #fff;

    &--1 {
      background-color: orangered;
    }
    &--2 {
      background-color: yellowgreen;
    }
    &--3 {
      background-color: blueviolet;
    }
    &--4 {
      background-color: palevioletred;
    }
    &--5 {
      background-color: royalblue;
    }
    &--6 {
      background-color: goldenrod;
    }
  }
}
```

```json
scripts": {
    "start": "nodemon npx node-sass scss/styles.scss css/styles.css",
    "dev": "nodemon -watch --update ./sass -x \"node-sass ./sass -o ./css --output-style compressed\" ",
    "dev2": "nodemon -w src/sass -x \"node-sass src/sass -o public/css --output-style compressed\""
  }
```
