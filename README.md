
Tampermonkey® by Jan Biniok
v5.1.1
	
Âu mon bypass fluxu on top
by Playvora
1
// ==UserScript==
2
// @name        Âu mon bypass fluxu on top
3
// @namespace    http://tampermonkey.net/
4
// @version      1.2.7
5
// @description  FLUXUS IS DOWN!!!!
6
// @author       Playvora
7
// @match        https://keysystem.flux.li/android/checkpoint/start.php?HWID=*
8
// @match        https://flux.li/android/checkpoint/check1.php
9
// @match        https://linkvertise.com/580726/fluxus1
10
// @match        https://linkvertise.com/580726/fluxus
11
// @match        https://flux.li/android/checkpoint/main.php
12
// @grant        GM_setClipboard
13
// @downloadURL https://update.greasyfork.org/scripts/488192/FLUXUS%20BYPASS%20NO%20CAPTCHA%20AT%20CHECKPOINT%201%20AND%202.user.js
14
// @updateURL https://update.greasyfork.org/scripts/488192/FLUXUS%20BYPASS%20NO%20CAPTCHA%20AT%20CHECKPOINT%201%20AND%202.meta.js
15
// ==/UserScript==
16
​
17
(function() {
18
    'use strict';
19
​
20
    const warningMessage = "Trying to bypass the Fluxus key system will get you banned from using Fluxus!!";
21
​
22
    function showOnlyRefreshButton() {
23
        const refreshButton = document.createElement('button');
24
        refreshButton.textContent = 'Only Refresh when you see "Trying to bypass the Fluxus key system will get you banned from using Fluxus!!"';
25
        refreshButton.style.position = 'fixed';
26
        refreshButton.style.top = '20px';
27
        refreshButton.style.right = '20px';
28
        refreshButton.style.backgroundColor = 'yellow';
29
        refreshButton.style.color = 'black';
30
        refreshButton.style.padding = '10px';
31
        refreshButton.style.border = 'none';
32
        refreshButton.style.borderRadius = '5px';
33
        refreshButton.style.cursor = 'pointer';
34
​
35
        document.body.appendChild(refreshButton);
Tam - Bot dịch vụ của bạn

Bạn có cần trợ giúp về việc tìm đầu ra console của Tampermonkey không?
Tắt
Tampermonkey Bot
