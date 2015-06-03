# firefox-dark-theme-fix
CSS configuration file for Firefox that fixed some appearance problems when using a dark theme on Ubuntu.
Copy the following to the userContent.css file located in "~/.mozilla/firefox/randomstring.default/chrome".
If the directory does not exist, create one. If the file does not exist, create one.

These settings will override some (not all, but most) of the conflicts on Firefox when using a dark theme.

```css
input {
  border: 2px inset white;
  background-color: white;
  color: black;
  -moz-appearance: none !important;
}

textarea {
  border: 2px inset white;
  background-color: white;
  color: black;
  -moz-appearance: none !important;
}

select {
  border: 2px inset white;
  background-color: white;
  color: black;
  -moz-appearance: none !important;
}

input[type="radio"],
input[type="checkbox"] {
  border: 2px inset white ! important;
  background-color: white ! important;
  color: ThreeDFace ! important;
  -moz-appearance: none !important;
}

*|*::-moz-radio {
  background-color: white;
  -moz-appearance: none !important;
}

button,
input[type="reset"],
input[type="button"],
input[type="submit"] {
  border: 2px outset white;
  background-color: #eeeeee;
  color: black;
  -moz-appearance: none !important;
}

body {
  background-color: white;
  color: black;
  display: block;
  margin: 8px;
  -moz-appearance: none !important;
}
```
