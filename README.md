# anki-theme
My Anki card theme.

Font used: [Hack](https://sourcefoundry.org/hack/)

## Front
```html
<div class="card-display shadow">
<div class="title">Ion</div>
{{Front}}
</div>
```

## CSS styling
(I really need to clean this up sometime)
```css
.card {
 background: #282a36;
}

.title {
 font-size: 15px;
 color: #ffb86c;
 margin-bottom: 10px;
 margin-top: -10px;
 padding: 5px;
 border-radius: 5px;
 background-color: #282a36;
 display: table;  /* https://stackoverflow.com/questions/7611030/css-display-inline-block-does-not-accept-margin-top */
 margin-left: auto;
 margin-right: auto;
}

.shadow {
 box-shadow: 0 3px 10px black;
}

.card-display {
 margin-top: 40px;
 margin-left: auto;
 margin-right: auto;
 padding: 20px;
 border-radius: 10px;
 width: 40%;
 max-width: 60%;
 height: auto;
 font-family: "Hack";
 font-size: 25px;
 text-align: center;
 color: #ff79c6;
 background: #44475a;
}

.card-display .mobile {
 width: 80%;
 max-width: 80%;
}

.front-display {
 border-radius: 10px 10px 0 0;
}

.answer {
 /*background: #6272a4;*/
 margin-top: 0;
 border-radius: 0 0 10px 10px;
 color: #50fa7b;
}

.mid {
width: calc(40% + 40px);
max-width: calc(60% + 40px);
height: 3px;
background: #6272a4;
margin-left: auto;
margin-right: auto;
}

.mid .mobile {
 width: calc(80% + 40px);
 max-width: calc(80% + 40px);
}
```

## Back
```css
<div class="card-display front-display shadow">
<div class="title">Ion</div>
{{Front}}
</div>
<div class="mid shadow"></div>
<div class="card-display answer shadow">
{{Back}}
</div>
```
