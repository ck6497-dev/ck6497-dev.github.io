[Logistics_Dashboard_2026_Jan_Report_Fixed.html](https://github.com/user-attachments/files/24728822/Logistics_Dashboard_2026_Jan_Report_Fixed.html)
<html lang="ko"><head><script>(function(firebaseConfig, initialAuthToken, appId) {
        window.__firebase_config = firebaseConfig;
        window.__initial_auth_token = initialAuthToken;
        window.__app_id = appId;
            })("\n{\n  \"apiKey\": \"AIzaSyCqyCcs2R2e7AegGjvFAwG98wlamtbHvZY\",\n  \"authDomain\": \"bard-frontend.firebaseapp.com\",\n  \"projectId\": \"bard-frontend\",\n  \"storageBucket\": \"bard-frontend.firebasestorage.app\",\n  \"messagingSenderId\": \"175205271074\",\n  \"appId\": \"1:175205271074:web:2b7bd4d34d33bf38e6ec7b\"\n}\n","eyJhbGciOiJSUzI1NiIsImtpZCI6IjI2NmM5YTIxZDM4NGQzZmU0OGMyZjNhYjNiZmE1NjQ0Yzk0ZmY3Y2UiLCJ0eXAiOiJKV1QifQ.eyJzdWIiOiJmaXJlYmFzZS1hZG1pbnNkay1mYnN2Y0BiYXJkLWZyb250ZW5kLmlhbS5nc2VydmljZWFjY291bnQuY29tIiwiYXVkIjoiaHR0cHM6Ly9pZGVudGl0eXRvb2xraXQuZ29vZ2xlYXBpcy5jb20vZ29vZ2xlLmlkZW50aXR5LmlkZW50aXR5dG9vbGtpdC52MS5JZGVudGl0eVRvb2xraXQiLCJ1aWQiOiIxNDM0MzE4NzU5MjQ0NjY3NzM0MCIsImlzcyI6ImZpcmViYXNlLWFkbWluc2RrLWZic3ZjQGJhcmQtZnJvbnRlbmQuaWFtLmdzZXJ2aWNlYWNjb3VudC5jb20iLCJjbGFpbXMiOnsiYXBwSWQiOiJjXzAxNWMyYmE5YjZmNDJhZjZfbG9naXN0aWNzX2Rhc2hib2FyZF92Mi5odG1sLTczOCJ9LCJleHAiOjE3Njg4OTEyNjcsImlhdCI6MTc2ODg4NzY2NywiYWxnIjoiUlMyNTYifQ.DbKAm63YBrYpabhlDEoczR6-FBWHnpsiExyM5MHBdd76130iJ_gYc-7YR4TAZvZeObuZ6Z1t9ohpOQRLmN_sjgWG8V2as23ZjXkCP4yLQwb1_QasdQnBZnVrY1upixtPZrLM4J7O5f5CeKR-k9wEa_nubxLnx5sQ6yCBwH8YEnpqnezrAVozdNN17r0uLqYEHI4-rX_yUgOrC9p-9wTgHN7QyVxEsf7dEBGqE2kOz1rDlIVPKhOIdFe2et2AM73biJAMxtgRNppj2HeWdOeceJ2vgQRhzjT06hlvdca11F4KXW2RNzp-4bn2TZ1kagKorUhE4We_ihY3tBL7dxBJPA","c_015c2ba9b6f42af6_logistics_dashboard_v2.html-738")</script><script>'use strict';var h=typeof Object.defineProperties=="function"?Object.defineProperty:function(a,b,d){if(a==Array.prototype||a==Object.prototype)return a;a[b]=d.value;return a};function l(a){a=["object"==typeof globalThis&&globalThis,a,"object"==typeof window&&window,"object"==typeof self&&self,"object"==typeof global&&global];for(var b=0;b<a.length;++b){var d=a[b];if(d&&d.Math==Math)return d}throw Error("Cannot find global object");}var n=l(this);
function p(a,b){if(b)a:{var d=n;a=a.split(".");for(var c=0;c<a.length-1;c++){var e=a[c];if(!(e in d))break a;d=d[e]}a=a[a.length-1];c=d[a];b=b(c);b!=c&&b!=null&&h(d,a,{configurable:!0,writable:!0,value:b})}}function r(a){function b(c){return a.next(c)}function d(c){return a.throw(c)}return new Promise(function(c,e){function f(g){g.done?c(g.value):Promise.resolve(g.value).then(b,d).then(f,e)}f(a.next())})}function t(a){return r(a())}
p("Object.values",function(a){return a?a:function(b){var d=[],c;for(c in b)Object.prototype.hasOwnProperty.call(b,c)&&d.push(b[c]);return d}});p("Array.prototype.includes",function(a){return a?a:function(b,d){var c=this;c instanceof String&&(c=String(c));var e=c.length;d=d||0;for(d<0&&(d=Math.max(d+e,0));d<e;d++){var f=c[d];if(f===b||Object.is(f,b))return!0}return!1}});/*

 MIT License

 Copyright (c) 2017-2023 W.Y.

 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:

 The above copyright notice and this permission notice shall be included in
 all copies or substantial portions of the Software.

 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.

*/
function u(a,b){const d=a.style;b.backgroundColor&&(d.backgroundColor=b.backgroundColor);b.width&&(d.width=`${b.width}px`);b.height&&(d.height=`${b.height}px`);const c=b.style;c!=null&&Object.keys(c).forEach(e=>{d[e]=c[e]})};var v=(()=>{let a=0;return()=>{a+=1;return`u${`0000${(Math.random()*1679616<<0).toString(36)}`.slice(-4)}${a}`}})();function w(a){const b=[];for(let d=0,c=a.length;d<c;d++)b.push(a[d]);return b}let x=null;function y(a={}){return x?x:a.l?x=a.l:x=w(window.getComputedStyle(document.documentElement))}function z(a,b){return(a=(a.ownerDocument.defaultView||window).getComputedStyle(a).getPropertyValue(b))?parseFloat(a.replace("px","")):0}
function A(a,b={}){var d;if(!(d=b.width)){d=z(a,"border-left-width");var c=z(a,"border-right-width");d=a.clientWidth+d+c}(b=b.height)||(b=z(a,"border-top-width"),c=z(a,"border-bottom-width"),b=a.clientHeight+b+c);return{width:d,height:b}}function B(a){return new Promise((b,d)=>{const c=new Image;c.onload=()=>{c.decode().then(()=>{requestAnimationFrame(()=>b(c))})};c.onerror=d;c.crossOrigin="anonymous";c.decoding="async";c.src=a})}
function C(a){return t(function*(){return Promise.resolve().then(()=>(new XMLSerializer).serializeToString(a)).then(encodeURIComponent).then(b=>`data:image/svg+xml;charset=utf-8,${b}`)})}
function D(a,b,d){return t(function*(){const c=document.createElementNS("http://www.w3.org/2000/svg","svg"),e=document.createElementNS("http://www.w3.org/2000/svg","foreignObject");c.setAttribute("width",`${b}`);c.setAttribute("height",`${d}`);c.setAttribute("viewBox",`0 0 ${b} ${d}`);e.setAttribute("width","100%");e.setAttribute("height","100%");e.setAttribute("x","0");e.setAttribute("y","0");e.setAttribute("externalResourcesRequired","true");c.appendChild(e);e.appendChild(a);return C(c)})}
var E=(a,b)=>{if(a instanceof b)return!0;a=Object.getPrototypeOf(a);return a===null?!1:a.constructor.name===b.name||E(a,b)};function F(a,b){return y(b).map(d=>{const c=a.getPropertyValue(d),e=a.getPropertyPriority(d);return`${d}: ${c}${e?" !important":""};`}).join(" ")}
function G(a,b,d,c){a=window.getComputedStyle(a,d);var e=a.getPropertyValue("content");if(e!==""&&e!=="none"){var f=v();try{b.className=`${b.className} ${f}`}catch(k){return}e=document.createElement("style");var g=e.appendChild;d=`.${f}:${d}`;a.cssText?(c=a.getPropertyValue("content"),c=`${a.cssText} content: '${c.replace(/'|"/g,"")}';`):c=F(a,c);g.call(e,document.createTextNode(`${d}{${c}}`));b.appendChild(e)}};function H(a){return a.search(/^(data:)/)!==-1}function I(a,b,d){return t(function*(){const c=yield fetch(a,b);if(c.status===404)throw Error(`Resource "${c.url}" not found`);const e=yield c.blob();return new Promise((f,g)=>{const k=new FileReader;k.onerror=g;k.onloadend=()=>{try{f(d({o:c,result:k.result}))}catch(m){g(m)}};k.readAsDataURL(e)})})}const J={};function K(a,b,d){let c=a.replace(/\?.*/,"");d&&(c=a);/ttf|otf|eot|woff2?/i.test(c)&&(c=c.replace(/.*\//,""));return b?`[${b}]${c}`:c}
function L(a,b,d){return t(function*(){const c=K(a,b,d.C);if(J[c]!=null)return J[c];d.u&&(a+=(/\?/.test(a)?"&":"?")+(new Date).getTime());let e;try{const f=yield I(a,d.i,({o:g,result:k})=>{b||(b=g.headers.get("Content-Type")||"");return k.split(/,/)[1]});e=`data:${b};base64,${f}`}catch(f){e=d.B||""}return J[c]=e})};const M={P:"application/font-woff",R:"application/font-woff",N:"application/font-truetype",v:"application/vnd.ms-fontobject",H:"image/png",F:"image/jpeg",D:"image/jpeg",A:"image/gif",M:"image/tiff",L:"image/svg+xml",O:"image/webp"};function N(a){return(a=/\.([^./]*?)$/g.exec(a))?a[1]:""};function O(a){return t(function*(){const b=a.toDataURL();return b==="data:,"?a.cloneNode(!1):B(b)})}function aa(a,b){return t(function*(){if(a.currentSrc){var d=document.createElement("canvas");const c=d.getContext("2d");d.width=a.clientWidth;d.height=a.clientHeight;c==null||c.drawImage(a,0,0,d.width,d.height);d=d.toDataURL();return B(d)}d=a.poster;d=yield L(d,M[N(d).toLowerCase()]||"",b);return B(d)})}
function ba(a,b){return t(function*(){try{let d;if(a==null?0:(d=a.contentDocument)==null?0:d.body)return yield P(a.contentDocument.body,b,!0)}catch(d){}return a.cloneNode(!1)})}function ca(a,b){return t(function*(){return E(a,HTMLCanvasElement)?O(a):E(a,HTMLVideoElement)?aa(a,b):E(a,HTMLIFrameElement)?ba(a,b):a.cloneNode(a.tagName!=null&&a.tagName.toUpperCase()==="SVG")})}
function da(a,b,d){return t(function*(){if(b.tagName!=null&&b.tagName.toUpperCase()==="SVG")return b;let c=[];if(a.tagName!=null&&a.tagName.toUpperCase()==="SLOT"&&a.assignedNodes)c=w(a.assignedNodes());else{let e;if(E(a,HTMLIFrameElement)&&((e=a.contentDocument)==null?0:e.body))c=w(a.contentDocument.body.childNodes);else{let f;c=w(((f=a.shadowRoot)!=null?f:a).childNodes)}}if(c.length===0||E(a,HTMLVideoElement))return b;yield c.reduce((e,f)=>e.then(()=>P(f,d)).then(g=>{g&&b.appendChild(g)}),Promise.resolve());
return b})}function ea(a,b,d){const c=b.style;if(c){var e=window.getComputedStyle(a);e.cssText?(c.cssText=e.cssText,c.transformOrigin=e.transformOrigin):y(d).forEach(f=>{let g=e.getPropertyValue(f);f==="font-size"&&g.endsWith("px")&&(g=`${Math.floor(parseFloat(g.substring(0,g.length-2)))-.1}px`);E(a,HTMLIFrameElement)&&f==="display"&&g==="inline"&&(g="block");f==="d"&&b.getAttribute("d")&&(g=`path(${b.getAttribute("d")})`);c.setProperty(f,g,e.getPropertyPriority(f))})}}
function fa(a,b){E(a,HTMLSelectElement)&&(b=Array.from(b.children).find(d=>a.value===d.getAttribute("value")))&&b.setAttribute("selected","")}
function ha(a,b){return t(function*(){var d=a.querySelectorAll?a.querySelectorAll("use"):[];if(d.length===0)return a;var c={};for(var e=0;e<d.length;e++){var f=d[e].getAttribute("xlink:href");if(f){const g=document.querySelector(f);a.querySelector(f)||!g||c[f]||(c[f]=yield P(g,b,!0))}}d=Object.values(c);if(d.length){c=document.createElementNS("http://www.w3.org/1999/xhtml","svg");c.setAttribute("xmlns","http://www.w3.org/1999/xhtml");c.style.position="absolute";c.style.width="0";c.style.height="0";
c.style.overflow="hidden";c.style.display="none";e=document.createElementNS("http://www.w3.org/1999/xhtml","defs");c.appendChild(e);for(f=0;f<d.length;f++)e.appendChild(d[f]);a.appendChild(c)}return a})}
function P(a,b,d){return t(function*(){return d||!b.filter||b.filter(a)?Promise.resolve(a).then(c=>ca(c,b)).then(c=>da(a,c,b)).then(c=>{E(c,Element)&&(ea(a,c,b),G(a,c,":before",b),G(a,c,":after",b),E(a,HTMLTextAreaElement)&&(c.textContent=a.value),E(a,HTMLInputElement)&&c.setAttribute("value",a.value),fa(a,c));return c}).then(c=>ha(c,b)):null})};const Q=/url\((['"]?)([^'"]+?)\1\)/g,ia=/url\([^)]+\)\s*format\((["']?)([^"']+)\1\)/g,ja=/src:\s*(?:url\([^)]+\)\s*format\([^)]+\)[,;]\s*)+/g;function ka(a){const b=[];a.replace(Q,(d,c,e)=>{b.push(e);return d});return b.filter(d=>!H(d))}
function la(a,b,d,c){return t(function*(){try{const e=d?(new URL(b,d||void 0)).toString():b;let f;f=yield L(e,M[N(b).toLowerCase()]||"",c);return a.replace(new RegExp(`(url\\(['"]?)(${b.replace(/([.*+?^${}()|\[\]\/\\])/g,"\\$1")})(['"]?\\))`,"g"),`$1${f}$3`)}catch(e){}return a})}function ma(a,{I:b}){return b?a.replace(ja,d=>{for(;;){const [c,,e]=ia.exec(d)||[],f=c,g=e;if(!g)return"";if(g===b)return`src: ${f};`}}):a}
function R(a,b,d){return t(function*(){if(a.search(Q)===-1)return a;const c=ma(a,d);return ka(c).reduce((e,f)=>e.then(g=>la(g,f,b,d)),Promise.resolve(c))})};function S(a,b,d){return t(function*(){var c;const e=(c=b.style)==null?void 0:c.getPropertyValue(a);return e?(c=yield R(e,null,d),b.style.setProperty(a,c,b.style.getPropertyPriority(a)),!0):!1})}function na(a,b){return t(function*(){(yield S("background",a,b))||(yield S("background-image",a,b));(yield S("mask",a,b))||(yield S("-webkit-mask",a,b))||(yield S("mask-image",a,b))||(yield S("-webkit-mask-image",a,b))})}
function oa(a,b){return t(function*(){const d=E(a,HTMLImageElement);if(d&&!H(a.src)||E(a,SVGImageElement)&&!H(a.href.baseVal)){var c=d?a.src:a.href.baseVal,e=yield L(c,M[N(c).toLowerCase()]||"",b);yield new Promise((f,g)=>{a.onload=f;a.onerror=b.m?(...k)=>{try{f(b.m(...k))}catch(m){g(m)}}:g;a.decode&&(a.decode=f);a.loading==="lazy"&&(a.loading="eager");d?(a.srcset="",a.src=e):a.href.baseVal=e})}})}
function pa(a,b){return t(function*(){const d=w(a.childNodes).map(c=>T(c,b));yield Promise.all(d).then(()=>a)})}function T(a,b){return t(function*(){E(a,Element)&&(yield na(a,b),yield oa(a,b),yield pa(a,b))})};const U={};function V(a){return t(function*(){var b=U[a];if(b!=null)return b;b=yield(yield fetch(a)).text();b={url:a,cssText:b};return U[a]=b})}function W(a,b){return t(function*(){let d=a.cssText;const c=/url\(["']?([^"')]+)["']?\)/g,e=(d.match(/url\([^)]+\)/g)||[]).map(f=>t(function*(){let g=f.replace(c,"$1");g.startsWith("https://")||(g=(new URL(g,a.url)).href);return I(g,b.i,({result:k})=>{d=d.replace(f,`url(${k})`);return[f,k]})}));return Promise.all(e).then(()=>d)})}
function X(a){if(a==null)return[];const b=[];a=a.replace(/(\/\*[\s\S]*?\*\/)/gi,"");for(var d=RegExp("((@.*?keyframes [\\s\\S]*?){([\\s\\S]*?}\\s*?)})","gi");;){var c=d.exec(a);if(c===null)break;b.push(c[0])}a=a.replace(d,"");d=/@import[\s\S]*?url\([^)]*\)[\s\S]*?;/gi;for(c=RegExp("((\\s*?(?:\\/\\*[\\s\\S]*?\\*\\/)?\\s*?@media[\\s\\S]*?){([\\s\\S]*?)}\\s*?})|(([\\s\\S]*?){([\\s\\S]*?)})","gi");;){let e=d.exec(a);if(e===null)if(e=c.exec(a),e===null)break;else d.lastIndex=c.lastIndex;else c.lastIndex=
d.lastIndex;b.push(e[0])}return b}
function qa(a,b){return t(function*(){const d=[],c=[];a.forEach(e=>{if("cssRules"in e)try{w(e.cssRules||[]).forEach((f,g)=>{if(f.type===CSSRule.IMPORT_RULE){let k=g+1;f=V(f.href).then(m=>W(m,b)).then(m=>X(m).forEach(q=>{try{e.insertRule(q,q.startsWith("@import")?k+=1:e.cssRules.length)}catch(Da){}})).catch(()=>{});c.push(f)}})}catch(f){const g=a.find(k=>k.href==null)||document.styleSheets[0];e.href!=null&&c.push(V(e.href).then(k=>W(k,b)).then(k=>X(k).forEach(m=>{g.insertRule(m,g.cssRules.length)})).catch(()=>
{}))}});return Promise.all(c).then(()=>{a.forEach(e=>{if("cssRules"in e)try{w(e.cssRules||[]).forEach(f=>{d.push(f)})}catch(f){}});return d})})}function ra(a){return a.filter(b=>b.type===CSSRule.FONT_FACE_RULE).filter(b=>b.style.getPropertyValue("src").search(Q)!==-1)}function sa(a,b){return t(function*(){if(a.ownerDocument==null)throw Error("Provided element is not within a Document");var d=w(a.ownerDocument.styleSheets);d=yield qa(d,b);return ra(d)})}
function ta(a){function b(c){(c.style.fontFamily||getComputedStyle(c).fontFamily).split(",").forEach(e=>{d.add(e.trim().replace(/["']/g,""))});Array.from(c.children).forEach(e=>{e instanceof HTMLElement&&b(e)})}const d=new Set;b(a);return d}function ua(a,b){return t(function*(){const d=yield sa(a,b),c=ta(a);return(yield Promise.all(d.filter(e=>c.has(e.style.fontFamily.trim().replace(/["']/g,""))).map(e=>R(e.cssText,e.parentStyleSheet?e.parentStyleSheet.href:null,b)))).join("\n")})}
function va(a,b){return t(function*(){const d=b.j!=null?b.j:b.K?null:yield ua(a,b);if(d){const c=document.createElement("style");c.appendChild(document.createTextNode(d));a.firstChild?a.insertBefore(c,a.firstChild):a.appendChild(c)}})};function wa(a,b={}){return t(function*(){const {width:d,height:c}=A(a,b),e=yield P(a,b,!0);yield va(e,b);yield T(e,b);u(e,b);return yield D(e,d,c)})}
function xa(a,b={}){return t(function*(){const {width:d,height:c}=A(a,b);var e=yield wa(a,b);e=yield B(e);const f=document.createElement("canvas"),g=f.getContext("2d"),k=b.G||window.devicePixelRatio||1,m=b.h||d,q=b.g||c;f.width=m*k;f.height=q*k;!b.J&&(f.width>16384||f.height>16384)&&(f.width>16384&&f.height>16384?f.width>f.height?(f.height*=16384/f.width,f.width=16384):(f.width*=16384/f.height,f.height=16384):f.width>16384?(f.height*=16384/f.width,f.width=16384):(f.width*=16384/f.height,f.height=
16384));f.style.width=`${m}`;f.style.height=`${q}`;b.backgroundColor&&(g.fillStyle=b.backgroundColor,g.fillRect(0,0,f.width,f.height));g.drawImage(e,0,0,f.width,f.height);return f})}function ya(a,b={}){return t(function*(){return(yield xa(a,b)).toDataURL()})};const za=["gemini.google.com","corp.google.com","proxy.googlers.com"];function Y(){return document.body.querySelectorAll('[class*="animate"]').length>0}function Z(a){return t(function*(){try{return yield ya(a,{h:a.offsetWidth,g:a.offsetHeight})}catch(d){var b=a.offsetHeight;const c=document.createElement("canvas");c.width=a.offsetWidth;c.height=b;return c.toDataURL("image/png")}})}
function Aa(){return t(function*(){const a=document.body.offsetWidth,b=document.body.offsetHeight,d=document.body.cloneNode(!0);d.querySelectorAll('[class*="animate"]').forEach(c=>{c.classList.remove(...Array.from(c.classList).filter(e=>e.startsWith("animate")))});d.style.width=`${a}px`;d.style.height=`${b}px`;return d})}
function Ba(a){return t(function*(){let b=document.body;if(Y()){var d=yield Aa();b=d;document.body.appendChild(d)}d=yield Z(b);Y()&&document.body.removeChild(b);window.parent.postMessage({type:"SEND_SCREENSHOT",image:d,topOffset:document.documentElement.scrollTop},a.origin)})}function Ca(a){return t(function*(){const b={type:"SEND_SCREENSHOT_FOR_DATA_VISUALIZATION",image:yield Z(document.body),topOffset:0};window.parent.postMessage(b,a.origin)})}
window.addEventListener("message",a=>t(function*(){if(za.some(d=>a.origin.includes(d))){var b=a.data;b&&(b.type==="MAKE_SCREENSHOT"&&(yield Ba(a)),b.type==="MAKE_SCREENSHOT_FOR_DATA_VISUALIZATION"&&(yield Ca(a)))}}));
</script><script>(function() {
  // Ensure this script is executed only once
  if (window.firebaseAuthBridgeScriptLoaded) {
    return;
  }
  window.firebaseAuthBridgeScriptLoaded = true;

  let nextTokenPromiseId = 0;

  // Stores { resolve, reject } for ongoing token requests
  const pendingTokenPromises = {};

  // Listen for messages from the Host Application
  window.addEventListener('message', function(event) {

    const messageData = event.data;

  if (messageData && messageData.type === 'RESOLVE_NEW_FIREBASE_TOKEN') {
      const { success, token, error, promiseId } = messageData ?? {};
      if (pendingTokenPromises[promiseId]) {
        if (success) {
          pendingTokenPromises[promiseId].resolve(token);
        } else {
          pendingTokenPromises[promiseId].reject(new Error(error || 'Token refresh failed from host.'));
        }
        delete pendingTokenPromises[promiseId];
      }
    }
  });

  // Expose a function for the Generated App to request a new Firebase token
  window.requestNewFirebaseToken = function() {
    const currentPromiseId = nextTokenPromiseId++;
    const promise = new Promise((resolve, reject) => {
      pendingTokenPromises[currentPromiseId] = { resolve, reject };
    });
    if (window.parent && window.parent !== window) {
      window.parent.postMessage({
        type: 'REQUEST_NEW_FIREBASE_TOKEN',
        promiseId: currentPromiseId
      }, '*');
    } else {
      pendingTokenPromises[currentPromiseId].reject(new Error('No parent window to request token from.'));
      delete pendingTokenPromises[currentPromiseId];
    }
    return promise;
  };
})();</script><script>
let realOriginalGetUserMedia = null;
if (navigator.mediaDevices && navigator.mediaDevices.getUserMedia) {
  realOriginalGetUserMedia = navigator.mediaDevices.getUserMedia.bind(navigator.mediaDevices);
}

(function() {
  if (navigator.mediaDevices && navigator.mediaDevices.__proto__) {
    try {
      Object.defineProperty(navigator.mediaDevices.__proto__, 'getUserMedia', {
        get: function() {
          return undefined; // Or throw an error
        },
        configurable: false
      });
    } catch (error) {
      console.error("Error defining prototype getter:", error);
    }
  }
})();

(function() {
  const pendingMediaResolvers = {};
  let nextMediaPromiseId = 0;

  function requestMediaPermissions(constraints) {
    const mediaPromiseId = nextMediaPromiseId++;
    const promise = new Promise((resolve, reject) => {
      pendingMediaResolvers[mediaPromiseId] = (granted) => {
        delete pendingMediaResolvers[mediaPromiseId];
        resolve(granted);
      };
    });

    window.parent.postMessage({
      type: 'requestMediaPermission',
      constraints: constraints,
      promiseId: mediaPromiseId,
    }, '*');

    return promise;
  }

  let originalGetUserMedia = realOriginalGetUserMedia;

  function interceptGetUserMedia() {
    if (navigator.mediaDevices) {
      Object.defineProperty(navigator.mediaDevices, 'getUserMedia', {
        value: function(constraints) {
          return requestMediaPermissions(constraints).then((granted) => {
            if (granted) {
              if (originalGetUserMedia) {
                return originalGetUserMedia(constraints);
              } else {
                throw new Error("Original getUserMedia not available.");
              }
            } else {
              throw new DOMException('Permission denied', 'NotAllowedError');
            }
          });
        },
        writable: false,
        configurable: false
      });
    }
  }

  interceptGetUserMedia();

  const observer = new MutationObserver(function(mutationsList, observer) {
    for (const mutation of mutationsList) {
      if (mutation.type === 'reconfigured' && mutation.name === 'getUserMedia' && mutation.object === navigator.mediaDevices) {
        interceptGetUserMedia();
      } else if (mutation.type === 'attributes' && mutation.attributeName === 'getUserMedia' && mutation.target === navigator.mediaDevices) {
        interceptGetUserMedia();
      } else if (mutation.type === 'childList' && mutation.addedNodes) {
        mutation.addedNodes.forEach(node => {
          if (node === navigator.mediaDevices) {
            interceptGetUserMedia();
          }
        });
      }
    }
  });

  function interceptSpeechRecognition() {
    if (!window.SpeechRecognition && !window.webkitSpeechRecognition) {
      return;
    }

    const OriginalSpeechRecognition = window.SpeechRecognition || window.webkitSpeechRecognition;

    const SpeechRecognitionWrapper = function(...args) {
      const recognizer = new OriginalSpeechRecognition(...args);
      const originalStart = recognizer.start.bind(recognizer);

      recognizer.start = function() {
        requestMediaPermissions({ audio: true }).then(granted => {
          if (granted) {
            originalStart();
          } else {
            const errorEvent = new SpeechRecognitionErrorEvent('error');
            errorEvent.error = 'not-allowed'; // This is the standard error for permission denial.
            recognizer.dispatchEvent(errorEvent);
          }
        });
      };

      return recognizer;
    };

    SpeechRecognitionWrapper.prototype = OriginalSpeechRecognition.prototype;
    SpeechRecognitionWrapper.prototype.constructor = SpeechRecognitionWrapper;

    if (window.SpeechRecognition) {
      window.SpeechRecognition = SpeechRecognitionWrapper;
    }
    if (window.webkitSpeechRecognition) {
      window.webkitSpeechRecognition = SpeechRecognitionWrapper;
    }
  }

  interceptSpeechRecognition();

  window.addEventListener('message', function(event) {
    if (event.data) {
      if (event.data.type === 'resolveMediaPermission') {
        const { promiseId, granted } = event.data;
        if (pendingMediaResolvers[promiseId]) {
          pendingMediaResolvers[promiseId](granted);
        }
      }
    }
  });

})();</script><script>((function(modelInformation) {
  const originalFetch = window.fetch;
  // TODO: b/421908508 - Move these out of the script and match all generative AI model calls.
  let googleLlmBaseApiUrls = [
    'https://generativelanguage.googleapis.com/v1beta/models/' + modelInformation.textModelName + ':streamGenerateContent',
    'https://generativelanguage.googleapis.com/v1beta/models/' + modelInformation.textModelName + ':generateContent',
    'https://generativelanguage.googleapis.com/v1beta/models/' + modelInformation.imageModelName + ':predict',
    'https://generativelanguage.googleapis.com/v1beta/models/' + modelInformation.imageModelName + ':predictLongRunning',
    'https://generativelanguage.googleapis.com/v1beta/models/' + modelInformation.imageEditModelName + ':generateContent',
    'https://generativelanguage.googleapis.com/v1beta/models/' + modelInformation.imageTransformModelName + ':generateContent',
    'https://generativelanguage.googleapis.com/v1beta/models/' + modelInformation.videoModelName + ':predict',
    'https://generativelanguage.googleapis.com/v1beta/models/' + modelInformation.videoModelName + ':predictLongRunning',
    'https://generativelanguage.googleapis.com/v1beta/models/' + modelInformation.ttsModelName + ':generateContent',
  ];
  modelInformation.deprecatedTextModelNames.forEach((modelName) => {
    googleLlmBaseApiUrls.push(
      'https://generativelanguage.googleapis.com/v1beta/models/' + modelName + ':streamGenerateContent',
      'https://generativelanguage.googleapis.com/v1beta/models/' + modelName + ':generateContent',
    );
  });
  modelInformation.deprecatedImageModelNames.forEach((modelName) => {
    googleLlmBaseApiUrls.push(
      'https://generativelanguage.googleapis.com/v1beta/models/' + modelName + ':predict',
      'https://generativelanguage.googleapis.com/v1beta/models/' + modelName + ':predictLongRunning',
    );
  });

  const pendingFetchResolvers = {};
  let nextPromiseId = 0;

  function handleStringInput(input, optionsArgument) {
    const actualUrl = input;
    const fetchCallArgs = [actualUrl, optionsArgument];
    const effectiveOptions = optionsArgument || {};
    const bodyForApiKeyCheck = effectiveOptions.body;
    const bodyForPostMessage = effectiveOptions.body;
    return { actualUrl, fetchCallArgs, effectiveOptions, bodyForApiKeyCheck, bodyForPostMessage };
  }

  function handleRequestInput(input, optionsArgument) {
    const actualUrl = input.url;
    const fetchCallArgs = [input, optionsArgument];
    const effectiveOptions = { method: input.method, headers: new Headers(input.headers) };
    let bodyForApiKeyCheck;
    let bodyForPostMessage;

    if (optionsArgument) {
      if (optionsArgument.method) effectiveOptions.method = optionsArgument.method;
      if (optionsArgument.headers) effectiveOptions.headers = new Headers(optionsArgument.headers);
      if ('body' in optionsArgument) {
        bodyForApiKeyCheck = optionsArgument.body;
        bodyForPostMessage = optionsArgument.body;
      } else {
        bodyForApiKeyCheck = undefined;
        bodyForPostMessage = input.body;
      }
    } else {
      bodyForApiKeyCheck = undefined;
      bodyForPostMessage = input.body;
    }
    return { actualUrl, fetchCallArgs, effectiveOptions, bodyForApiKeyCheck, bodyForPostMessage };
  }

  window.fetch = function(input, optionsArgument) {
    let actualUrl;
    let fetchCallArgs;
    let effectiveOptions = {};
    let bodyForApiKeyCheck;
    let bodyForPostMessage;

    if (typeof input === 'string') {
      ({actualUrl, fetchCallArgs, effectiveOptions, bodyForApiKeyCheck, bodyForPostMessage} = handleStringInput(input, optionsArgument));
    } else if (input instanceof Request) {
      ({actualUrl, fetchCallArgs, effectiveOptions, bodyForApiKeyCheck, bodyForPostMessage} = handleRequestInput(input, optionsArgument));
    } else {
      return originalFetch.apply(window, [input, optionsArgument]);
    }

    effectiveOptions.method = effectiveOptions.method || 'GET';
    if (!effectiveOptions.headers) {
      effectiveOptions.headers = new Headers();
    }


    if (typeof actualUrl === 'string' && googleLlmBaseApiUrls.some((url) => actualUrl.startsWith(url))) {
      let apiKeyIsNull = true;

      const regex = new RegExp("models/([^:]+)");
      const modelNameMatch = actualUrl.match(regex);
      const modelName = modelNameMatch ? modelNameMatch[1] : 'unspecified';


      try {
        const urlObject = new URL(actualUrl);  // Use URL object for robust parsing
        const apiKeyParam = urlObject.searchParams.get('key');
        if (apiKeyParam) {
          apiKeyIsNull = false;
        }
      } catch (e) {
        // Continue checks even if URL parsing fails
      }

      if (apiKeyIsNull && effectiveOptions.headers) {
        const h = new Headers(effectiveOptions.headers);
        const apiKeyHeaderValue = h.get('X-API-Key') || h.get('x-api-key');
        if (apiKeyHeaderValue) {
          apiKeyIsNull = false;
          return originalFetch.apply(window, fetchCallArgs);
        }
      }

      if (apiKeyIsNull && effectiveOptions.method && ['POST', 'PUT', 'PATCH'].includes(effectiveOptions.method.toUpperCase()) && typeof bodyForApiKeyCheck === 'string') {
        try {
          const bodyData = JSON.parse(bodyForApiKeyCheck);
          if (bodyData && bodyData.apiKey) {
            apiKeyIsNull = false;
            return originalFetch.apply(window, fetchCallArgs);
          }
        } catch (e) {
          // Ignore JSON parsing errors
        }
      }

      if(apiKeyIsNull) {
        const promiseId = nextPromiseId++;
        const promise = new Promise((resolve) => {
          pendingFetchResolvers[promiseId] = (resolvedResponse) => {
            delete pendingFetchResolvers[promiseId];
            resolve(resolvedResponse);
          };
        });

        let serializedBodyForPostMessage;
        if (typeof bodyForPostMessage === 'string' || bodyForPostMessage == null) {
            serializedBodyForPostMessage = bodyForPostMessage;
        } else if (bodyForPostMessage instanceof ReadableStream) {
            serializedBodyForPostMessage = null;
        } else {
            try {
                serializedBodyForPostMessage = JSON.stringify(bodyForPostMessage);
            } catch (e) {
                serializedBodyForPostMessage = null;
            }
        }

        const messageOptions = {
            method: effectiveOptions.method,
            headers: Object.fromEntries(new Headers(effectiveOptions.headers).entries()),
            body: serializedBodyForPostMessage
        };

        window.parent.postMessage({
          type: 'requestFetch',
          url: actualUrl,
          modelName: modelName,
          options: messageOptions,
          promiseId: promiseId,
        }, '*');

        return promise;
      }
      return originalFetch.apply(window, fetchCallArgs);
    }
    return originalFetch.apply(window, fetchCallArgs);
  };

  window.addEventListener('message', function(event) {
    if (event.data && event.data.type === 'resolveFetch') {
      const { promiseId, response } = event.data;
      if (pendingFetchResolvers[promiseId]) {
        try {
          const reconstructedResponse = new Response(response.body, {
            status: response.status,
            statusText: response.statusText,
            headers: new Headers(response.headers),
          });
          pendingFetchResolvers[promiseId](reconstructedResponse);
        } catch (error) {
          pendingFetchResolvers[promiseId](new Response(null, { status: 500, statusText: "Interceptor Response Reconstruction Error" }));
        }
      }
    }
  });

}))({"textModelName":"gemini-2.5-flash-preview-09-2025","imageModelName":"imagen-4.0-generate-001","imageEditModelName":"gemini-2.5-flash-image-preview","imageTransformModelName":"gemini-3-pro-image-preview-11-2025","videoModelName":"veo-2.0-generate-001","ttsModelName":"gemini-2.5-flash-preview-tts","deprecatedTextModelNames":["gemini-2.0-flash","gemini-2.5-flash-preview-04-17","gemini-2.5-flash-preview-05-20"],"deprecatedImageModelNames":["imagen-3.0-generate-001","imagen-3.0-generate-002"]})</script><script>(function() {
  const originalConsoleLog = console.log;
  const originalConsoleError = console.error;

    /**
   * Normalizes an error event or a promise rejection reason into a structured error object.
   * @param {*} errorEventOrReason The error object or reason.
   * @return {object} Structured error data { message, name, stack }.
   */
  function getErrorObject(errorEventOrReason) {
    if (errorEventOrReason instanceof Error) {
      return {
        message: errorEventOrReason.message,
        name: errorEventOrReason.name,
        stack: errorEventOrReason.stack,
      };
    }
    // Fallback for non-Error objects.
    try {
      return {
        message: JSON.stringify(errorEventOrReason),
        name: 'UnknownErrorType',
        stack: null,
      };
    } catch (e) {
      return {
        message: String(errorEventOrReason),
        name: 'UnknownErrorTypeNonStringifiable',
        stack: null,
      };
    }
  }

  /**
   * Converts an array of arguments (from log/error) into a single string.
   * Handles Error objects specially to include their message and stack.
   * @param {Array<*>} args - Arguments passed to console methods.
   * @return {string} A string representation of the arguments.
   */
  function stringifyArgs(args) {
    return args
      .map((arg) => {
        if (arg instanceof Error) {
          const {message, stack} = arg;
          return `Error: ${message}${stack ? ('\nStack: ' + stack) : ''}`;
        }
        if (typeof arg === 'object' && arg !== null) {
          try {
            return JSON.stringify(arg);
          } catch (error) {
            return '[Circular Object]';
          }
        } else {
          return String(arg);
        }
      })
      .join(' ');
  }

  console.log = function(...args) {
    const logString = stringifyArgs(args);
    window.parent.postMessage({ type: 'log', message: logString }, '*');
    originalConsoleLog.apply(console, args);
  };

  console.error = function(...args) {
    let errorData;
    if (args.length > 0 && args[0] instanceof Error) {
      const err = args[0];
      // If the first arg is an Error, capture its details.
      errorData = {
        type: 'error',
        source: 'CONSOLE_ERROR',
        ...getErrorObject(err),
        rawArgsString: stringifyArgs(args.slice(1)),
        timestamp: new Date().toISOString(),
      };
    } else {
      // If not an Error object, treat all args as a general error message.
      errorData = {
        type: 'error',
        source: 'CONSOLE_ERROR',
        message: stringifyArgs(args),
        name: 'ConsoleLoggedError',
        stack: null,
        timestamp: new Date().toISOString(),
      };
    }
    window.parent.postMessage(errorData, '*');
    originalConsoleError.apply(console, args);
  };

  // Listen for global unhandled synchronous errors.
  window.addEventListener('error', function(event) {
    const errorDetails = event.error ? getErrorObject(event.error) : {
      message: event.message,
      name: 'GlobalError',
      stack: null,
      filename: event.filename,
      lineno: event.lineno,
      colno: event.colno,
    };

    window.parent.postMessage({
      type: 'error',
      source: 'global',
      ...errorDetails,
      message: errorDetails.message || event.message,
      timestamp: new Date().toISOString(),
    }, '*');
  });

  // Listen for unhandled promise rejections (asynchronous errors).
  window.addEventListener('unhandledrejection', function(event) {
    const errorDetails = getErrorObject(event.reason);

    window.parent.postMessage({
      type: 'error',
      source: 'unhandledrejection',
      ...errorDetails,
      message: errorDetails.message || 'Unhandled Promise Rejection',
      timestamp: new Date().toISOString(),
    }, '*');
  });

})();</script>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Global Logistics Expert Dashboard - 2026 Jan</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js" crossorigin="anonymous"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap');
        body { font-family: 'Inter', sans-serif; background-color: #f8fafc; }
        .sidebar-link:hover { background-color: rgba(255, 255, 255, 0.1); }
        .card-shadow { box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1); }
        .status-pill { padding: 2px 8px; border-radius: 9999px; font-size: 0.75rem; font-weight: 600; }
        .detail-row { display: none; background-color: #fefce8; }
        .detail-row.active { display: table-row; }
        #toast { visibility: hidden; min-width: 250px; background-color: #1e293b; color: #fff; text-align: center; border-radius: 8px; padding: 16px; position: fixed; z-index: 1000; left: 50%; bottom: 30px; transform: translateX(-50%); }
        #toast.show { visibility: visible; animation: fadein 0.5s, fadeout 0.5s 2.5s; }
        @keyframes fadein { from {bottom: 0; opacity: 0;} to {bottom: 30px; opacity: 1;} }
        @keyframes fadeout { from {bottom: 30px; opacity: 1;} to {bottom: 0; opacity: 0;} }
    </style>
<style>*, ::before, ::after{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgb(59 130 246 / 0.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgb(59 130 246 / 0.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }/* ! tailwindcss v3.4.17 | MIT License | https://tailwindcss.com */*,::after,::before{box-sizing:border-box;border-width:0;border-style:solid;border-color:#e5e7eb}::after,::before{--tw-content:''}:host,html{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;tab-size:4;font-family:ui-sans-serif, system-ui, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";font-feature-settings:normal;font-variation-settings:normal;-webkit-tap-highlight-color:transparent}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;font-feature-settings:normal;font-variation-settings:normal;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-feature-settings:inherit;font-variation-settings:inherit;font-size:100%;font-weight:inherit;line-height:inherit;letter-spacing:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0;padding:0}legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]:where(:not([hidden=until-found])){display:none}.absolute{position:absolute}.sticky{position:sticky}.bottom-0{bottom:0px}.top-0{top:0px}.mx-auto{margin-left:auto;margin-right:auto}.mb-1{margin-bottom:0.25rem}.mb-10{margin-bottom:2.5rem}.mb-2{margin-bottom:0.5rem}.mb-20{margin-bottom:5rem}.mb-6{margin-bottom:1.5rem}.mb-8{margin-bottom:2rem}.mr-2{margin-right:0.5rem}.mr-3{margin-right:0.75rem}.mt-1{margin-top:0.25rem}.mt-6{margin-top:1.5rem}.flex{display:flex}.grid{display:grid}.hidden{display:none}.h-2{height:0.5rem}.h-6{height:1.5rem}.h-full{height:100%}.h-8{height:2rem}.min-h-screen{min-height:100vh}.w-2{width:0.5rem}.w-5{width:1.25rem}.w-64{width:16rem}.w-\[80\%\]{width:80%}.w-\[90\%\]{width:90%}.w-\[98\%\]{width:98%}.w-full{width:100%}.w-8{width:2rem}.max-w-7xl{max-width:80rem}.flex-1{flex:1 1 0%}.shrink-0{flex-shrink:0}.border-collapse{border-collapse:collapse}.cursor-pointer{cursor:pointer}.grid-cols-1{grid-template-columns:repeat(1, minmax(0, 1fr))}.grid-cols-2{grid-template-columns:repeat(2, minmax(0, 1fr))}.flex-col{flex-direction:column}.flex-wrap{flex-wrap:wrap}.items-start{align-items:flex-start}.items-end{align-items:flex-end}.items-center{align-items:center}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.gap-2{gap:0.5rem}.gap-4{gap:1rem}.gap-6{gap:1.5rem}.space-x-2 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(0.5rem * var(--tw-space-x-reverse));margin-left:calc(0.5rem * calc(1 - var(--tw-space-x-reverse)))}.space-y-6 > :not([hidden]) ~ :not([hidden]){--tw-space-y-reverse:0;margin-top:calc(1.5rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(1.5rem * var(--tw-space-y-reverse))}.divide-y > :not([hidden]) ~ :not([hidden]){--tw-divide-y-reverse:0;border-top-width:calc(1px * calc(1 - var(--tw-divide-y-reverse)));border-bottom-width:calc(1px * var(--tw-divide-y-reverse))}.divide-slate-100 > :not([hidden]) ~ :not([hidden]){--tw-divide-opacity:1;border-color:rgb(241 245 249 / var(--tw-divide-opacity, 1))}.overflow-hidden{overflow:hidden}.overflow-x-auto{overflow-x:auto}.rounded-2xl{border-radius:1rem}.rounded-full{border-radius:9999px}.rounded-lg{border-radius:0.5rem}.rounded-xl{border-radius:0.75rem}.border{border-width:1px}.border-b{border-bottom-width:1px}.border-amber-100{--tw-border-opacity:1;border-color:rgb(254 243 199 / var(--tw-border-opacity, 1))}.border-red-100{--tw-border-opacity:1;border-color:rgb(254 226 226 / var(--tw-border-opacity, 1))}.border-slate-100{--tw-border-opacity:1;border-color:rgb(241 245 249 / var(--tw-border-opacity, 1))}.border-slate-200{--tw-border-opacity:1;border-color:rgb(226 232 240 / var(--tw-border-opacity, 1))}.bg-amber-400{--tw-bg-opacity:1;background-color:rgb(251 191 36 / var(--tw-bg-opacity, 1))}.bg-amber-50{--tw-bg-opacity:1;background-color:rgb(255 251 235 / var(--tw-bg-opacity, 1))}.bg-amber-500{--tw-bg-opacity:1;background-color:rgb(245 158 11 / var(--tw-bg-opacity, 1))}.bg-red-50{--tw-bg-opacity:1;background-color:rgb(254 242 242 / var(--tw-bg-opacity, 1))}.bg-red-600{--tw-bg-opacity:1;background-color:rgb(220 38 38 / var(--tw-bg-opacity, 1))}.bg-slate-400{--tw-bg-opacity:1;background-color:rgb(148 163 184 / var(--tw-bg-opacity, 1))}.bg-slate-50{--tw-bg-opacity:1;background-color:rgb(248 250 252 / var(--tw-bg-opacity, 1))}.bg-slate-800{--tw-bg-opacity:1;background-color:rgb(30 41 59 / var(--tw-bg-opacity, 1))}.bg-slate-900{--tw-bg-opacity:1;background-color:rgb(15 23 42 / var(--tw-bg-opacity, 1))}.bg-white{--tw-bg-opacity:1;background-color:rgb(255 255 255 / var(--tw-bg-opacity, 1))}.bg-amber-100{--tw-bg-opacity:1;background-color:rgb(254 243 199 / var(--tw-bg-opacity, 1))}.bg-green-100{--tw-bg-opacity:1;background-color:rgb(220 252 231 / var(--tw-bg-opacity, 1))}.bg-red-100{--tw-bg-opacity:1;background-color:rgb(254 226 226 / var(--tw-bg-opacity, 1))}.p-4{padding:1rem}.p-6{padding:1.5rem}.px-4{padding-left:1rem;padding-right:1rem}.px-6{padding-left:1.5rem;padding-right:1.5rem}.py-2{padding-top:0.5rem;padding-bottom:0.5rem}.py-3{padding-top:0.75rem;padding-bottom:0.75rem}.py-4{padding-top:1rem;padding-bottom:1rem}.px-8{padding-left:2rem;padding-right:2rem}.py-5{padding-top:1.25rem;padding-bottom:1.25rem}.text-left{text-align:left}.text-center{text-align:center}.text-2xl{font-size:1.5rem;line-height:2rem}.text-lg{font-size:1.125rem;line-height:1.75rem}.text-sm{font-size:0.875rem;line-height:1.25rem}.text-xl{font-size:1.25rem;line-height:1.75rem}.text-xs{font-size:0.75rem;line-height:1rem}.text-\[10px\]{font-size:10px}.font-bold{font-weight:700}.font-medium{font-weight:500}.uppercase{text-transform:uppercase}.leading-relaxed{line-height:1.625}.leading-tight{line-height:1.25}.tracking-wider{letter-spacing:0.05em}.text-amber-400{--tw-text-opacity:1;color:rgb(251 191 36 / var(--tw-text-opacity, 1))}.text-amber-500{--tw-text-opacity:1;color:rgb(245 158 11 / var(--tw-text-opacity, 1))}.text-amber-700{--tw-text-opacity:1;color:rgb(180 83 9 / var(--tw-text-opacity, 1))}.text-amber-800{--tw-text-opacity:1;color:rgb(146 64 14 / var(--tw-text-opacity, 1))}.text-red-400{--tw-text-opacity:1;color:rgb(248 113 113 / var(--tw-text-opacity, 1))}.text-red-500{--tw-text-opacity:1;color:rgb(239 68 68 / var(--tw-text-opacity, 1))}.text-red-600{--tw-text-opacity:1;color:rgb(220 38 38 / var(--tw-text-opacity, 1))}.text-red-700{--tw-text-opacity:1;color:rgb(185 28 28 / var(--tw-text-opacity, 1))}.text-red-800{--tw-text-opacity:1;color:rgb(153 27 27 / var(--tw-text-opacity, 1))}.text-slate-300{--tw-text-opacity:1;color:rgb(203 213 225 / var(--tw-text-opacity, 1))}.text-slate-400{--tw-text-opacity:1;color:rgb(148 163 184 / var(--tw-text-opacity, 1))}.text-slate-500{--tw-text-opacity:1;color:rgb(100 116 139 / var(--tw-text-opacity, 1))}.text-slate-600{--tw-text-opacity:1;color:rgb(71 85 105 / var(--tw-text-opacity, 1))}.text-slate-800{--tw-text-opacity:1;color:rgb(30 41 59 / var(--tw-text-opacity, 1))}.text-slate-900{--tw-text-opacity:1;color:rgb(15 23 42 / var(--tw-text-opacity, 1))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255 / var(--tw-text-opacity, 1))}.text-amber-600{--tw-text-opacity:1;color:rgb(217 119 6 / var(--tw-text-opacity, 1))}.text-green-700{--tw-text-opacity:1;color:rgb(21 128 61 / var(--tw-text-opacity, 1))}.text-slate-700{--tw-text-opacity:1;color:rgb(51 65 85 / var(--tw-text-opacity, 1))}.shadow-lg{--tw-shadow:0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.shadow-amber-200{--tw-shadow-color:#fde68a;--tw-shadow:var(--tw-shadow-colored)}.transition-colors{transition-property:color, background-color, border-color, fill, stroke, -webkit-text-decoration-color;transition-property:color, background-color, border-color, text-decoration-color, fill, stroke;transition-property:color, background-color, border-color, text-decoration-color, fill, stroke, -webkit-text-decoration-color;transition-timing-function:cubic-bezier(0.4, 0, 0.2, 1);transition-duration:150ms}.hover\:bg-amber-500:hover{--tw-bg-opacity:1;background-color:rgb(245 158 11 / var(--tw-bg-opacity, 1))}.hover\:bg-slate-50:hover{--tw-bg-opacity:1;background-color:rgb(248 250 252 / var(--tw-bg-opacity, 1))}.focus\:outline-none:focus{outline:2px solid transparent;outline-offset:2px}.focus\:ring-2:focus{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow), var(--tw-ring-shadow), var(--tw-shadow, 0 0 #0000)}.focus\:ring-amber-400:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(251 191 36 / var(--tw-ring-opacity, 1))}.group:hover .group-hover\:text-amber-500{--tw-text-opacity:1;color:rgb(245 158 11 / var(--tw-text-opacity, 1))}@media (min-width: 640px){.sm\:flex{display:flex}}@media (min-width: 768px){.md\:block{display:block}.md\:grid-cols-2{grid-template-columns:repeat(2, minmax(0, 1fr))}.md\:grid-cols-5{grid-template-columns:repeat(5, minmax(0, 1fr))}.md\:flex-row{flex-direction:row}.md\:items-center{align-items:center}.md\:p-8{padding:2rem}}@media (min-width: 1024px){.lg\:col-span-5{grid-column:span 5 / span 5}.lg\:col-span-7{grid-column:span 7 / span 7}.lg\:grid-cols-12{grid-template-columns:repeat(12, minmax(0, 1fr))}}</style></head>
<body class="flex">

    <!-- Sidebar -->
    <aside id="sidebar" class="w-64 bg-slate-900 text-white min-h-screen sticky top-0 hidden md:block">
        <div class="p-6">
            <h1 class="text-xl font-bold text-amber-400">Logistics Expert</h1>
            <p class="text-xs text-slate-400 mt-1">30 Years Experience Insights</p>
        </div>
        <nav class="mt-6">
            <a href="#summary" class="sidebar-link flex items-center px-6 py-3 text-slate-300 bg-slate-800">
                <i class="fas fa-chart-line w-5 mr-3"></i> Executive Summary
            </a>
            <a href="#metrics" class="sidebar-link flex items-center px-6 py-3 text-slate-300">
                <i class="fas fa-globe w-5 mr-3"></i> Global Indices
            </a>
            <a href="#regional" class="sidebar-link flex items-center px-6 py-3 text-slate-300">
                <i class="fas fa-map-marked-alt w-5 mr-3"></i> Regional Status
            </a>
        </nav>
        <div class="absolute bottom-0 w-full p-6 bg-slate-800">
            <p class="text-xs text-slate-500">Deep Research Mode Active</p>
        </div>
    </aside>

    <!-- Main Content -->
    <main id="reportContent" class="flex-1 p-4 md:p-8 max-w-7xl mx-auto">
        
        <!-- Header -->
        <header class="flex justify-between items-center mb-8">
            <div>
                <h2 class="text-2xl font-bold text-slate-800">2026년 1월 글로벌 물류 전략 대시보드</h2>
                <p class="text-red-600 font-bold">실무 긴급: 춘절(LNY) 전 'Red Zone' 대응 및 호주 파업 리스크 관리</p>
            </div>
            <div class="hidden sm:flex space-x-2">
                <button onclick="downloadHTML()" class="bg-amber-400 text-slate-900 px-4 py-2 rounded-lg text-sm font-bold hover:bg-amber-500 transition-colors shadow-lg shadow-amber-200">
                    <i class="fas fa-share-square mr-2"></i> 대시보드 파일 추출
                </button>
                <button onclick="downloadPDF()" class="bg-white border border-slate-200 px-4 py-2 rounded-lg text-sm font-medium hover:bg-slate-50">
                    <i class="fas fa-download mr-2 text-amber-500"></i> Report PDF
                </button>
            </div>
        </header>

        <!-- Executive Summary & Risk Heatmap -->
        <section id="summary" class="mb-10">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-6">
                <!-- Expert Insights -->
                <div class="lg:col-span-7 bg-white p-6 rounded-2xl card-shadow border border-slate-100">
                    <h3 class="text-lg font-bold text-slate-800 mb-6 flex items-center">
                        <span class="w-2 h-6 bg-red-600 mr-3 rounded-full"></span>
                        전문가 실무 총평 (Action Priorities)
                    </h3>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <div class="p-4 bg-red-50 rounded-xl border border-red-100">
                            <p class="text-sm font-bold text-red-800 mb-2"><i class="fas fa-fire-alt mr-2"></i> [Priority 1] 춘절(LNY) 골든타임</p>
                            <p class="text-xs text-red-700 leading-relaxed">1/20~1/26 선적분이 마지막 기회입니다. 이후 선복 마감 및 GRI 폭등 예상. 2월 중순 화물은 지금 즉시 부킹 확정하십시오.</p>
                        </div>
                        <div class="p-4 bg-amber-50 rounded-xl border border-amber-100">
                            <p class="text-sm font-bold text-amber-800 mb-2"><i class="fas fa-exclamation-triangle mr-2"></i> [위험] 호주 항만 파업 장기화</p>
                            <p class="text-xs text-amber-700 leading-relaxed">MELBOURNE항 DP World/Patrick 파업으로 리드타임 +7일 이상 발생. 시드니 우회 혹은 내륙운송 대안을 검토하십시오.</p>
                        </div>
                        <div class="p-4 bg-slate-50 rounded-xl border border-slate-100">
                            <p class="text-sm font-bold text-slate-800 mb-2"><i class="fas fa-snowflake mr-2"></i> 북반구 혹한기 물류 정체</p>
                            <p class="text-xs text-slate-600 leading-relaxed">밴쿠버 철송 및 북유럽 항만 겨울 폭풍으로 야드 밀도 임계치 도달. 내륙 LT에 최소 10일의 버퍼를 추가하십시오.</p>
                        </div>
                        <div class="p-4 bg-slate-50 rounded-xl border border-slate-100">
                            <p class="text-sm font-bold text-slate-800 mb-2"><i class="fas fa-shield-alt mr-2"></i> CIS 제재 및 통관 강화</p>
                            <p class="text-xs text-slate-600 leading-relaxed">러시아향 전략물자 통제 강화로 부산항 선적 전 심사 지연 빈번. HS Code 기반 Compliance 사전 체크가 필수적입니다.</p>
                        </div>
                    </div>
                </div>

                <!-- Risk Heatmap -->
                <div class="lg:col-span-5 bg-slate-900 text-white p-6 rounded-2xl card-shadow">
                    <h3 class="text-lg font-bold mb-6 flex justify-between items-center">
                        <span>리스크 히트맵 (Action Priority)</span>
                    </h3>
                    <div class="space-y-6">
                        <div>
                            <div class="flex justify-between text-xs mb-2">
                                <span class="text-red-400 font-bold">LNY 밀어내기 선복 부족 (동남아/중국)</span>
                                <span class="text-red-400 font-bold">98% Critical</span>
                            </div>
                            <div class="w-full bg-slate-800 h-2 rounded-full overflow-hidden">
                                <div class="bg-red-600 h-full w-[98%]"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between text-xs mb-2">
                                <span class="text-amber-400 font-bold">호주 항만 노조 파업 (MEL/AKL)</span>
                                <span class="text-amber-400 font-bold">90% High</span>
                            </div>
                            <div class="w-full bg-slate-800 h-2 rounded-full overflow-hidden">
                                <div class="bg-amber-500 h-full w-[90%]"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between text-xs mb-2">
                                <span class="text-slate-300">GSCPI 공급망 압력 지수 급증</span>
                                <span class="text-slate-300">80% High</span>
                            </div>
                            <div class="w-full bg-slate-800 h-2 rounded-full overflow-hidden">
                                <div class="bg-slate-400 h-full w-[80%]"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Global Indices -->
        <section id="metrics" class="mb-10">
            <h3 class="text-lg font-bold text-slate-800 mb-6 uppercase tracking-wider">주요 물류 지표 (보고서 기반 최신치)</h3>
            <div class="grid grid-cols-2 md:grid-cols-5 gap-4">
                <div class="bg-white p-4 rounded-xl card-shadow border border-slate-100">
                    <p class="text-xs text-slate-500 font-bold mb-1">SCFI</p>
                    <div class="flex items-end justify-between">
                        <span class="text-xl font-bold text-slate-800">1,574.12</span>
                        <span class="text-red-500 text-xs font-bold"><i class="fas fa-caret-up"></i> 1.37%</span>
                    </div>
                </div>
                <div class="bg-white p-4 rounded-xl card-shadow border border-slate-100">
                    <p class="text-xs text-slate-500 font-bold mb-1">GSCPI</p>
                    <div class="flex items-end justify-between">
                        <span class="text-xl font-bold text-slate-800">0.51</span>
                        <span class="text-red-500 text-xs font-bold">High</span>
                    </div>
                </div>
                <div class="bg-white p-4 rounded-xl card-shadow border border-slate-100">
                    <p class="text-xs text-slate-500 font-bold mb-1">WTI</p>
                    <div class="flex items-end justify-between">
                        <span class="text-xl font-bold text-slate-800">$59.41</span>
                        <span class="text-red-500 text-xs font-bold"><i class="fas fa-caret-up"></i> 2.4%</span>
                    </div>
                </div>
                <div class="bg-white p-4 rounded-xl card-shadow border border-slate-100">
                    <p class="text-xs text-slate-500 font-bold mb-1">BAF</p>
                    <div class="flex items-end justify-between">
                        <span class="text-xl font-bold text-slate-800">$758</span>
                        <span class="text-red-500 text-xs font-bold">Up</span>
                    </div>
                </div>
                <div class="bg-white p-4 rounded-xl card-shadow border border-slate-100">
                    <p class="text-xs text-slate-500 font-bold mb-1">ERAI</p>
                    <div class="flex items-end justify-between">
                        <span class="text-xl font-bold text-slate-800">Stable</span>
                        <span class="text-slate-400 text-xs">-</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- Regional Status -->
        <section id="regional" class="mb-10">
            <div class="flex flex-col md:flex-row justify-between items-start md:items-center mb-6 gap-4">
                <h3 class="text-lg font-bold text-slate-800 uppercase tracking-wider">권역별 상세 현황 (33개 핵심 루트)</h3>
                <div class="flex flex-wrap gap-2">
                    <input type="text" id="portSearch" placeholder="항만명 검색..." class="px-4 py-2 border border-slate-200 rounded-lg text-sm focus:outline-none focus:ring-2 focus:ring-amber-400">
                    <select id="regionFilter" class="px-4 py-2 border border-slate-200 rounded-lg text-sm focus:outline-none">
                        <option value="all">전체 구간</option>
                        <option value="sea">동남아/오세아니아</option>
                        <option value="na">북미/남미</option>
                        <option value="ea">동아시아(일/대/홍)</option>
                        <option value="eu">유럽/지중해</option>
                        <option value="cis">러시아/중앙아시아</option>
                    </select>
                </div>
            </div>

            <div class="bg-white rounded-2xl card-shadow border border-slate-100 overflow-hidden">
                <div class="overflow-x-auto">
                    <table class="w-full text-left border-collapse">
                        <thead class="bg-slate-50 border-b border-slate-200">
                            <tr>
                                <th class="px-6 py-4 text-xs font-bold text-slate-500 uppercase">Port / Route</th>
                                <th class="px-6 py-4 text-xs font-bold text-slate-500 uppercase">Status</th>
                                <th class="px-6 py-4 text-xs font-bold text-slate-500 uppercase">Lead Time</th>
                                <th class="px-6 py-4 text-xs font-bold text-slate-500 uppercase text-center">Detail</th>
                            </tr>
                        </thead>
                        <tbody id="portTableBody" class="divide-y divide-slate-100"><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">Port Kelang</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Malaysia</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-amber-100 text-amber-700">Caution</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">10-14일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p1" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 춘절 전 물량 집중으로 선복 확보 어려움. 환적 야드 밀도 높음.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">MANILA</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Philippines</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-green-100 text-green-700">Normal</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">5-9일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p2" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 마닐라 북항/남항 운영 원활. 다만 연초 통관 강화 이슈 주의.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">BANGKOK</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Thailand</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-amber-100 text-amber-700">Caution</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">12-16일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p3" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 람차방 환적 물량 증가로 인한 바지선 연결 지연 가능성.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">SIHANOUKVILLE</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Cambodia</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-amber-100 text-amber-700">Caution</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">14-18일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p4" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 직항 대비 환적 서비스 위주. 연결 지연 리스크 고려 필수.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">JAKARTA</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Indonesia</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-amber-100 text-amber-700">Caution</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">10-15일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p5" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 탄중 프리옥 항만 혼잡도 상승. 세관 'Red Line' 검사 비율 증가 시기.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">SINGAPORE</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Singapore</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-green-100 text-green-700">Normal</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">7-10일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p6" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 운영 효율은 높으나 춘절 전 환적 화물 폭증으로 야드 적체율 상승.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">MELBOURNE</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Australia</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-red-100 text-red-700">Critical</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">18-28일+</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p7" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> DP World/Patrick 파업 지속. 선박 체선 심각. 시드니 우회 회항 빈번.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">AUCKLAND</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">New Zealand</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-amber-100 text-amber-700">Caution</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">20-30일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p8" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 호주 항만 파업 여파로 인한 피더 연결 지연 직격탄.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">VANCOUVER</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Canada</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-amber-100 text-amber-700">Caution</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">14-20일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p9" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 터미널 내 철도 조차장 혼잡. Rail Dwell Time 증가 추세.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">up to MISSISSAUGA (Rail)</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Canada (Toronto)</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-red-100 text-red-700">Critical</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">35-50일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p10" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 밴쿠버발 철송 지연(평균 7.7일 체류) 및 혹한으로 인한 운행 중단 빈번.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">up to MISSISSAUGA (Truck)</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Canada (Vancouver)</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-red-100 text-red-700">Critical</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">25-35일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p11" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 로키 산맥 기상 악화로 도로 폐쇄 위험. 철송 대안이나 비용 매우 높음.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">SEATTLE</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">USA</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-green-100 text-green-700">Normal</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">12-16일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p12" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 캘리포니아 대비 혼잡도 낮음. 미 중서부 내륙 화물의 진입점으로 추천.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">LONG BEACH</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">USA</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-amber-100 text-amber-700">Caution</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">12-18일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p13" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 레일카 부족으로 컨테이너 터미널 체류 시간 5-7일로 증가.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">NEWYORK</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">USA</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-amber-100 text-amber-700">Caution</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">28-40일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p14" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 파나마 통행 제한 및 희망봉 우회 노선 고착화로 LT 편차 큼.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">SAVANNAH</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">USA</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-amber-100 text-amber-700">Caution</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">30-38일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p15" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 우회 선박 일시 유입(Vessel Bunching) 시 하역 지연 발생 가능.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">VITORIA</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Brazil</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-green-100 text-green-700">Normal</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">35-45일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p16" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 산토스 대비 혼잡도 낮으나 주로 피더 환적 서비스 위주.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">KAOHSIUNG</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Taiwan</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-green-100 text-green-700">Normal</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">3-5일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p17" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 운영 안정적. 서비스 빈도 높아 스페이스 확보 용이.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">KEELUNG</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Taiwan</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-green-100 text-green-700">Normal</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">3-5일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p18" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 대만 북부 관문. 특이사항 없이 원활한 흐름 유지.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">HONGKONG</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Hong Kong</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-green-100 text-green-700">Normal</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">3-5일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p19" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 중국 주강삼각주 피더 네트워크 지연 여부 모니터링 필요.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">YOKOHAMA</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Japan</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-green-100 text-green-700">Normal</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">2-4일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p20" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 매우 안정적. 내륙 트러킹 인력 수급 상황만 주의 요망.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">HAKATA</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Japan</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-green-100 text-green-700">Normal</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">1-2일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p21" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 최단거리 루트. 페리 서비스 이용 시 긴급 화물 처리에 최적.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">SOUTHHAMPTON</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">UK</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-amber-100 text-amber-700">Caution</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">40-50일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p22" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 겨울철 기상 악화(강풍) 및 희망봉 우회로 LT 장기화.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">ROTTERDAM</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Netherlands</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-amber-100 text-amber-700">Caution</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">38-48일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p23" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 겨울 폭풍으로 터미널 운영 효율 저하. 바지선 연결 지연 심화.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">ISTANBUL</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Turkey</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-green-100 text-green-700">Normal</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">35-45일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p24" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> Middle Corridor 종착지로서 중요성 증대. 큰 혼잡 없음.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">TOSHKENT</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Uzbekistan</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-amber-100 text-amber-700">Caution</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">30-45일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p25" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 중국 경유 TCR. 중국-카자흐 국경 화차 교환 병목 구간.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">BISHKEK (TCR)</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Kyrgyzstan</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-amber-100 text-amber-700">Caution</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">35-50일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p26" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 동절기 폭설 시 국경 폐쇄 빈번. 보수적인 LT 설정 필수.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">VLADIVOSTOK</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Russia</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-amber-100 text-amber-700">Caution</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">2-5일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p27" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 선복 제한 및 운임 높음. 한국 세관 전략물자 통제 심사 강화.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">MOSCOW (TSR)</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Russia</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-red-100 text-red-700">Critical</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">25-35일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p28" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> RZD 화차 부족 및 군수 물자 우선 배정으로 민간 화물 순위 밀림.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">NOVOSIBIRSK (TSR)</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Russia</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-red-100 text-red-700">Critical</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">20-30일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p29" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 시베리아 중심부 혹한기(-40도) 장비 고장 및 속도 저하 리스크.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">MOSCOW (Truck)</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Russia</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-red-100 text-red-700">Critical</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">18-25일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p30" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 철송 대안이나 9,000km 장거리와 도로 결빙으로 리스크 극대.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">NOVOSIBIRSK (Truck)</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Russia</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-red-100 text-red-700">Critical</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">12-18일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p31" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 동절기 화물 파손(동결) 위험 대비 보온/냉장 트럭 권장.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">ALMATY (TCR)</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Kazakhstan</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-amber-100 text-amber-700">Caution</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">25-35일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p32" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 중앙아시아 허브. 호르고스 국경 춘절 전 물량 집중 예상.</p>
                        </div>
                    </td>
                </tr><tr class="hover:bg-slate-50 transition-colors cursor-pointer group">
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">Ulaanbaatar</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">Mongolia</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill bg-amber-100 text-amber-700">Caution</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">15-25일</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                </tr><tr id="detail-p33" class="detail-row">
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> 톈진항 적체 및 얼리안 국경 환적 지연이 주된 리스크. (중앙아시아 철도 연계 루트)</p>
                        </div>
                    </td>
                </tr></tbody>
                    </table>
                </div>
            </div>
        </section>

        <footer class="mb-20 text-center text-slate-400 text-xs">
            <p>© 2026 Logistics Strategic Center. 보고서 내용 기반 33개 루트 실시간 시황 적용</p>
        </footer>

    </main>

    <div id="toast">파일 추출이 완료되었습니다.</div>

    <script>
        const portData = [
            // 동남아/오세아니아 (8)
            { id: "p1", name: "Port Kelang", country: "Malaysia", region: "sea", status: "Caution", lt: "10-14일", detail: "춘절 전 물량 집중으로 선복 확보 어려움. 환적 야드 밀도 높음." },
            { id: "p2", name: "MANILA", country: "Philippines", region: "sea", status: "Normal", lt: "5-9일", detail: "마닐라 북항/남항 운영 원활. 다만 연초 통관 강화 이슈 주의." },
            { id: "p3", name: "BANGKOK", country: "Thailand", region: "sea", status: "Caution", lt: "12-16일", detail: "람차방 환적 물량 증가로 인한 바지선 연결 지연 가능성." },
            { id: "p4", name: "SIHANOUKVILLE", country: "Cambodia", region: "sea", status: "Caution", lt: "14-18일", detail: "직항 대비 환적 서비스 위주. 연결 지연 리스크 고려 필수." },
            { id: "p5", name: "JAKARTA", country: "Indonesia", region: "sea", status: "Caution", lt: "10-15일", detail: "탄중 프리옥 항만 혼잡도 상승. 세관 'Red Line' 검사 비율 증가 시기." },
            { id: "p6", name: "SINGAPORE", country: "Singapore", region: "sea", status: "Normal", lt: "7-10일", detail: "운영 효율은 높으나 춘절 전 환적 화물 폭증으로 야드 적체율 상승." },
            { id: "p7", name: "MELBOURNE", country: "Australia", region: "sea", status: "Critical", lt: "18-28일+", detail: "DP World/Patrick 파업 지속. 선박 체선 심각. 시드니 우회 회항 빈번." },
            { id: "p8", name: "AUCKLAND", country: "New Zealand", region: "sea", status: "Caution", lt: "20-30일", detail: "호주 항만 파업 여파로 인한 피더 연결 지연 직격탄." },
            
            // 북미/남미 (7)
            { id: "p9", name: "VANCOUVER", country: "Canada", region: "na", status: "Caution", lt: "14-20일", detail: "터미널 내 철도 조차장 혼잡. Rail Dwell Time 증가 추세." },
            { id: "p10", name: "up to MISSISSAUGA (Rail)", country: "Canada (Toronto)", region: "na", status: "Critical", lt: "35-50일", detail: "밴쿠버발 철송 지연(평균 7.7일 체류) 및 혹한으로 인한 운행 중단 빈번." },
            { id: "p11", name: "up to MISSISSAUGA (Truck)", country: "Canada (Vancouver)", region: "na", status: "Critical", lt: "25-35일", detail: "로키 산맥 기상 악화로 도로 폐쇄 위험. 철송 대안이나 비용 매우 높음." },
            { id: "p12", name: "SEATTLE", country: "USA", region: "na", status: "Normal", lt: "12-16일", detail: "캘리포니아 대비 혼잡도 낮음. 미 중서부 내륙 화물의 진입점으로 추천." },
            { id: "p13", name: "LONG BEACH", country: "USA", region: "na", status: "Caution", lt: "12-18일", detail: "레일카 부족으로 컨테이너 터미널 체류 시간 5-7일로 증가." },
            { id: "p14", name: "NEWYORK", country: "USA", region: "na", status: "Caution", lt: "28-40일", detail: "파나마 통행 제한 및 희망봉 우회 노선 고착화로 LT 편차 큼." },
            { id: "p15", name: "SAVANNAH", country: "USA", region: "na", status: "Caution", lt: "30-38일", detail: "우회 선박 일시 유입(Vessel Bunching) 시 하역 지연 발생 가능." },
            { id: "p16", name: "VITORIA", country: "Brazil", region: "na", status: "Normal", lt: "35-45일", detail: "산토스 대비 혼잡도 낮으나 주로 피더 환적 서비스 위주." },

            // 동아시아 (5)
            { id: "p17", name: "KAOHSIUNG", country: "Taiwan", region: "ea", status: "Normal", lt: "3-5일", detail: "운영 안정적. 서비스 빈도 높아 스페이스 확보 용이." },
            { id: "p18", name: "KEELUNG", country: "Taiwan", region: "ea", status: "Normal", lt: "3-5일", detail: "대만 북부 관문. 특이사항 없이 원활한 흐름 유지." },
            { id: "p19", name: "HONGKONG", country: "Hong Kong", region: "ea", status: "Normal", lt: "3-5일", detail: "중국 주강삼각주 피더 네트워크 지연 여부 모니터링 필요." },
            { id: "p20", name: "YOKOHAMA", country: "Japan", region: "ea", status: "Normal", lt: "2-4일", detail: "매우 안정적. 내륙 트러킹 인력 수급 상황만 주의 요망." },
            { id: "p21", name: "HAKATA", country: "Japan", region: "ea", status: "Normal", lt: "1-2일", detail: "최단거리 루트. 페리 서비스 이용 시 긴급 화물 처리에 최적." },

            // 유럽/지중해 (3)
            { id: "p22", name: "SOUTHHAMPTON", country: "UK", region: "eu", status: "Caution", lt: "40-50일", detail: "겨울철 기상 악화(강풍) 및 희망봉 우회로 LT 장기화." },
            { id: "p23", name: "ROTTERDAM", country: "Netherlands", region: "eu", status: "Caution", lt: "38-48일", detail: "겨울 폭풍으로 터미널 운영 효율 저하. 바지선 연결 지연 심화." },
            { id: "p24", name: "ISTANBUL", country: "Turkey", region: "eu", status: "Normal", lt: "35-45일", detail: "Middle Corridor 종착지로서 중요성 증대. 큰 혼잡 없음." },

            // 러시아/중앙아시아 (10)
            { id: "p25", name: "TOSHKENT", country: "Uzbekistan", region: "cis", status: "Caution", lt: "30-45일", detail: "중국 경유 TCR. 중국-카자흐 국경 화차 교환 병목 구간." },
            { id: "p26", name: "BISHKEK (TCR)", country: "Kyrgyzstan", region: "cis", status: "Caution", lt: "35-50일", detail: "동절기 폭설 시 국경 폐쇄 빈번. 보수적인 LT 설정 필수." },
            { id: "p27", name: "VLADIVOSTOK", country: "Russia", region: "cis", status: "Caution", lt: "2-5일", detail: "선복 제한 및 운임 높음. 한국 세관 전략물자 통제 심사 강화." },
            { id: "p28", name: "MOSCOW (TSR)", country: "Russia", region: "cis", status: "Critical", lt: "25-35일", detail: "RZD 화차 부족 및 군수 물자 우선 배정으로 민간 화물 순위 밀림." },
            { id: "p29", name: "NOVOSIBIRSK (TSR)", country: "Russia", region: "cis", status: "Critical", lt: "20-30일", detail: "시베리아 중심부 혹한기(-40도) 장비 고장 및 속도 저하 리스크." },
            { id: "p30", name: "MOSCOW (Truck)", country: "Russia", region: "cis", status: "Critical", lt: "18-25일", detail: "철송 대안이나 9,000km 장거리와 도로 결빙으로 리스크 극대." },
            { id: "p31", name: "NOVOSIBIRSK (Truck)", country: "Russia", region: "cis", status: "Critical", lt: "12-18일", detail: "동절기 화물 파손(동결) 위험 대비 보온/냉장 트럭 권장." },
            { id: "p32", name: "ALMATY (TCR)", country: "Kazakhstan", region: "cis", status: "Caution", lt: "25-35일", detail: "중앙아시아 허브. 호르고스 국경 춘절 전 물량 집중 예상." },
            { id: "p33", name: "Ulaanbaatar", country: "Mongolia", region: "cis", status: "Caution", lt: "15-25일", detail: "톈진항 적체 및 얼리안 국경 환적 지연이 주된 리스크. (중앙아시아 철도 연계 루트)" }
        ];

        function renderTable(data) {
            const body = document.getElementById('portTableBody');
            body.innerHTML = '';
            data.forEach(port => {
                const tr = document.createElement('tr');
                tr.className = "hover:bg-slate-50 transition-colors cursor-pointer group";
                tr.onclick = () => toggleDetail(port.id);
                
                let statusClass = "bg-green-100 text-green-700";
                if(port.status === "Caution") statusClass = "bg-amber-100 text-amber-700";
                if(port.status === "Critical") statusClass = "bg-red-100 text-red-700";

                tr.innerHTML = `
                    <td class="px-6 py-4">
                        <div class="font-bold text-slate-800 leading-tight">${port.name}</div>
                        <div class="text-[10px] text-slate-400 mt-1 uppercase">${port.country}</div>
                    </td>
                    <td class="px-6 py-4"><span class="status-pill ${statusClass}">${port.status}</span></td>
                    <td class="px-6 py-4 text-sm text-slate-600 font-medium">${port.lt}</td>
                    <td class="px-6 py-4 text-center"><i class="fas fa-chevron-down text-slate-300 group-hover:text-amber-500"></i></td>
                `;
                
                const detailTr = document.createElement('tr');
                detailTr.id = `detail-${port.id}`;
                detailTr.className = "detail-row";
                detailTr.innerHTML = `
                    <td colspan="4" class="px-8 py-5">
                        <div class="flex items-start">
                            <div class="w-8 h-8 bg-amber-100 rounded-full flex items-center justify-center mr-3 shrink-0">
                                <i class="fas fa-lightbulb text-amber-600 text-xs"></i>
                            </div>
                            <p class="text-sm text-slate-700 leading-relaxed"><span class="font-bold text-slate-900">Insight:</span> ${port.detail}</p>
                        </div>
                    </td>
                `;
                body.appendChild(tr);
                body.appendChild(detailTr);
            });
        }

        function toggleDetail(id) {
            const row = document.getElementById(`detail-${id}`);
            const isActive = row.classList.contains('active');
            document.querySelectorAll('.detail-row').forEach(r => r.classList.remove('active'));
            if(!isActive) row.classList.add('active');
        }

        function filterData() {
            const search = document.getElementById('portSearch').value.toLowerCase();
            const region = document.getElementById('regionFilter').value;
            const filtered = portData.filter(p => {
                const matchesSearch = p.name.toLowerCase().includes(search) || p.country.toLowerCase().includes(search);
                const matchesRegion = region === 'all' || p.region === region;
                return matchesSearch && matchesRegion;
            });
            renderTable(filtered);
        }

        function downloadHTML() {
            const blob = new Blob([document.documentElement.outerHTML], { type: 'text/html' });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = 'Logistics_Dashboard_2026_Jan_Report_Fixed.html';
            a.click();
            URL.revokeObjectURL(url);
            showToast();
        }

        async function downloadPDF() {
            const opt = { margin: 10, filename: 'Logistics_Expert_Report_2026.pdf', image: { type: 'jpeg', quality: 0.98 }, html2canvas: { scale: 2 }, jsPDF: { unit: 'mm', format: 'a4', orientation: 'portrait' } };
            await html2pdf().set(opt).from(document.getElementById('reportContent')).save();
        }

        function showToast() {
            const t = document.getElementById("toast");
            t.className = "show";
            setTimeout(() => { t.className = t.className.replace("show", ""); }, 3000);
        }

        document.getElementById('portSearch').addEventListener('input', filterData);
        document.getElementById('regionFilter').addEventListener('change', filterData);
        window.onload = () => renderTable(portData);
    </script>

</body></html>
