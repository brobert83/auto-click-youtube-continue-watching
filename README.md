Install tampermonkey

Add this script
```
// ==UserScript==
// @name         Auto click continue watch on youtube
// @namespace    http://tampermonkey.net/
// @version      0.1
// @description  try to take over the world!
// @author       You
// @match        https://www.youtube.com/watch?v=qWZL5RnfgtI
// @grant        none
// @include      https://www.youtube.com
// ==/UserScript==

(function() {
    'use strict';
    setTimeout(function(){document.getElementById("confirm-button").children[0].children[0].children[0].click()}, 1000);
})();
```

Enjoy