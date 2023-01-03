### CSS Debugger in any webssite through bookmark

1. Go to [zaydek.github.io/debug.css](https://zaydek.github.io/debug.css)
2. Bookmark “Debug CSS” (just simply drag the lint to your Bookmarks Bar)
2. Click the bookmark to **toggle it on and off**

Sources:
- https://github.com/zaydek-old/zaydek.github.io
- https://medium.com/free-code-camp/heres-my-favorite-weird-trick-to-debug-css-88529aa5a6a3

About Zaydek:
- https://github.com/zaydek-old
- https://github.com/zaydek
- https://zaydek.github.io/


| Debugger OFF | Debugger ON |
|--------------|-------------|
|<img width="500" alt="CleanShot 2022-04-23 at 01 19 35@2x" src="https://user-images.githubusercontent.com/22046823/164816509-50f89cd7-6a71-4519-aa42-14c82fc2fdf9.png"> | <img width="500" alt="CleanShot 2022-04-23 at 01 19 20@2x" src="https://user-images.githubusercontent.com/22046823/164816495-4c46e3fc-a3c1-46c3-9baf-a4b9b001a614.png"> |

### JS Code form Zaydek
javascript:/* debug.css | MIT License | zaydek.github.com/debug.css */ if (!("is_debugging" in window)) { is_debugging = false; var debug_el = document.createElement("style"); debug_el.append(document.createTextNode(`*:not(path):not(g) { color: hsla(210, 100%, 100%, 0.9) !important; background: hsla(210, 100%,  50%, 0.5) !important; outline: solid 0.25rem hsla(210, 100%, 100%, 0.5) !important; box-shadow: none !important; filter: none !important; }`)); } function enable_debugger() { if (!is_debugging) { document.head.appendChild(debug_el); is_debugging = true; } } function disable_debugger() { if (is_debugging) { document.head.removeChild(debug_el); is_debugging = false; } } !is_debugging ? enable_debugger() : disable_debugger();
