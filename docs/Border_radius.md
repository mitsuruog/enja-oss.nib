## Border radius

Nib's `border-radius` supports both the regular syntax as well as augmenting it to make the value more expressive.

Nibの `border-radius` は通常の記法と同様に、値をもっとわかりやすできる追加記法にも対応しています。

```stylus
button {
  border-radius: 1px 2px / 3px 4px;
}

button {
  border-radius: 5px;
}

button {
  border-radius: bottom 10px;
}
```

yielding:

結果:

```css
button {
  -webkit-border-radius: 1px 2px/3px 4px;
  -moz-border-radius: 1px 2px/3px 4px;
  border-radius: 1px 2px/3px 4px;
}
button {
  -webkit-border-radius: 5px;
  -moz-border-radius: 5px;
  border-radius: 5px;
}
button {
  -moz-border-radius-topleft: 10px;
  -webkit-border-top-left-radius: 10px;
  border-top-left-radius: 10px;
  -moz-border-radius-bottomright: 10px;
  -webkit-border-bottom-right-radius: 10px;
  border-bottom-right-radius: 10px;
}
```
