### Github theme switcher
```
javascript:!function(){"use strict";const e=e=>{if(null==e)return new DocumentFragment;const t=document.createElement("template");return t.innerHTML=e,t.content};e.one=t=>{var s;return null!==(s=e(t).firstElementChild)&&void 0!==s?s:void 0};const t=Symbol("null");let s=0;var r=class extends Map{constructor(){super(),this._objectHashes=new WeakMap,this._symbolHashes=new Map,this._publicKeys=new Map;const[e]=arguments;if(null!=e){if("function"!=typeof e[Symbol.iterator])throw new TypeError(typeof e+" is not iterable (cannot read property Symbol(Symbol.iterator))");for(const[t,s]of e)this.set(t,s)}}_getPublicKeys(e,t=!1){if(!Array.isArray(e))throw new TypeError("The keys parameter must be an array");const s=this._getPrivateKey(e,t);let r;return s&&this._publicKeys.has(s)?r=this._publicKeys.get(s):t&&(r=[...e],this._publicKeys.set(s,r)),{privateKey:s,publicKey:r}}_getPrivateKey(e,r=!1){const o=[];for(let n of e){null===n&&(n=t);const e="object"==typeof n||"function"==typeof n?"_objectHashes":"symbol"==typeof n&&"_symbolHashes";if(e)if(this[e].has(n))o.push(this[e].get(n));else{if(!r)return!1;{const t=`@@mkm-ref-${s++}@@`;this[e].set(n,t),o.push(t)}}else o.push(n)}return JSON.stringify(o)}set(e,t){const{publicKey:s}=this._getPublicKeys(e,!0);return super.set(s,t)}get(e){const{publicKey:t}=this._getPublicKeys(e);return super.get(t)}has(e){const{publicKey:t}=this._getPublicKeys(e);return super.has(t)}delete(e){const{publicKey:t,privateKey:s}=this._getPublicKeys(e);return Boolean(t&&super.delete(t)&&this._publicKeys.delete(s))}clear(){super.clear(),this._symbolHashes.clear(),this._publicKeys.clear()}get[Symbol.toStringTag](){return"ManyKeysMap"}get size(){return super.size}};var o=()=>{const e={};return e.promise=new Promise(((t,s)=>{e.resolve=t,e.reject=s})),e};const n=new r;var i=(e,{target:t=document,stopOnDomReady:s=!0,timeout:r=1/0}={})=>{const i=[t,e,s,r],c=n.get(i);if(c)return c;let l;const a=o(),{promise:u}=a;n.set(i,u);const m=()=>{cancelAnimationFrame(l),n.delete(i,u),a.resolve()};return r!==1/0&&setTimeout(m,r),function r(){const o=t.querySelector(e);o?(a.resolve(o),m()):!s||"interactive"!==document.readyState&&"complete"!==document.readyState?l=requestAnimationFrame(r):m()}(),Object.assign(u,{stop:m})};(async()=>{const t=document.createElement("style");t.innerHTML="\n  .github-theme-switch:hover {\n    color: var(--color-text-primary);\n    background-color: var(--color-bg-overlay);\n  }\n  ",document.head.appendChild(t);const s=document.createElement("span");s.setAttribute("role","menuitem"),s.classList.add("dropdown-item","github-theme-switch"),s.textContent="Theme preference";const r=await i('.dropdown-item[href="https://gist.github.com/mine"]',{stopOnDomReady:!1}),o=await(async()=>{const t=await fetch("https://github.com/settings/appearance"),s=await t.text(),r=e(s).querySelector(".js-color-mode-settings");r.classList.add("mt-1","ml-1"),r.querySelector(".flex-column").classList.remove("flex-lg-row");for(const e of r.querySelectorAll("img"))e.parentElement.style.border="none",e.parentElement.style.fontWeight="normal",e.remove();for(const e of r.querySelectorAll(".position-relative"))e.classList.remove("mb-4");return r})();r.after(s,o)})()}();
```
### Light House
```
javascript:window.location='https://developers.google.com/speed/pagespeed/insights/?url='+encodeURI(window.location);
```
### G Translate
```
javascript:void(open('https://translate.google.co.in/translate?hl=en&sl=sq&tl=en&u='+location.href));
```
### Sticky header remover
```
javascript:(function() {    document.querySelectorAll('*').forEach(function(n) {        var p = getComputedStyle(n).getPropertyValue('position');        if (p === 'fixed' || p === 'sticky') {            n.style.cssText += ' ; position: absolute !important;';        }    });})();
```
### Website diguiser
```
javascript:(function() { setInterval(function() { var link = document.querySelector("link[rel*='icon']") || document.createElement('link'); link.type = 'image/x-icon'; link.rel = 'shortcut icon'; link.href = 'https://www.google.com/s2/favicons?domain=google.com'; document.getElementsByTagName('head')[0].appendChild(link); document.title = "Google"; console.log("Stealth Activated");; }, 1000); })();
```
----
[![Repo-name](https://img.shields.io/badge/Visit-configs-lightblue?style=for-the-badge&logo=github) ](https://github.com/fynks/configs)
[ ![Author-Fynks](https://img.shields.io/badge/Author-Fynks-yellow?style=for-the-badge&logo=atom)](#)
