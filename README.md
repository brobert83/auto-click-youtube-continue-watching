Install tampermonkey

Add this script
```
// ==UserScript==
// @name         Auto click continue watch on youtube
// @namespace    http://tampermonkey.net/
// @version      0.1
// @description  try to take over the world!
// @author       You
// @grant        none
// @include      https://www.youtube.com/*
// ==/UserScript==

(function () {
    'use strict';

    (function close() {
        try {
            var button = document.getElementById("confirm-button").children[0].children[0].children[0];
            console.log(button);
            button.click();
        } catch (e) {
        }
        console.log("close");
        setTimeout(close, 1000);
    })();

})();
```

Enjoy