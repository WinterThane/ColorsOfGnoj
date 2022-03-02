# Colors of Gnoj

Zip file contains:
- ColorsOfGnoj.options.json
- ColorsOfGnoj.storage.json
- ColorsOfGnoj.user.js

// ==UserScript==
// @name         ColorsOfGnoj
// @namespace    http://tampermonkey.net/
// @version      0.1
// @description  fsa tota leta
// @author       WinterThane
// @match        https://mn3njalnik.com/index.php?/forum/21-gnoji%C5%A1%C4%8De/
// @icon         https://www.google.com/s2/favicons?sz=64&domain=simply-how.com
// @grant        none
// ==/UserScript==

(function() {
    'use strict';

    var css = ".roomWrapper { background-color: #000000; } " +
              ".chatbox_msg { color: #FFFFFF; font-weight: bold; font-size: 14px; background-image: url('https://cdn-icons-png.flaticon.com/512/2336/2336319.png'); background-size: 17px 17px; background-repeat: no-repeat; padding-left: 20px; } " +
              ".chatterName { font-weight: bold; font-size: 14px; background-image: url('https://cdn-icons-png.flaticon.com/512/2336/2336319.png'); background-size: 17px 17px; background-repeat: no-repeat; padding-left: 22px; } " +
              //".chatbox_msg { font-color: #111111; font-weight: bold; font-size: 14px; background-image: url('https://cdn-icons-png.flaticon.com/512/3050/3050031.png'); background-size: 17px 17px; background-repeat: no-repeat; padding-left: 20px; } " +
              //".chatterName { font-weight: bold; font-size: 14px; background-image: url('https://cdn-icons-png.flaticon.com/512/3050/3050031.png'); background-size: 17px 17px; background-repeat: no-repeat; padding-left: 20px; } " +
              ".cbTime { color: #FFFFFF; font-weight: bold } ";
    var style = document.createElement("style");
    style.type = "text/css";
    style.appendChild(document.createTextNode(css));
    document.head.appendChild(style);

    //data-member="WinterThane" -- target
    //class="chatterName" -- mn3 name
    //data-action="mention" -- text row with @ mention
    //class="ipsDataItem -- text row
    //https://cdn-icons-png.flaticon.com/512/3050/3050031.png
    //class="ipsFieldRow_content" -- text enter row
})();
