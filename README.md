# Read-PDF-in-Dark-mode-on-Microsoft-edge

## Process
1. Open PDF in MS-edge
2. Go to ` inspect -> console ` and past bellow code and last hit `enter`


```bash
 var cover = document.createElement("div"); 
 let css = ` 
 position: fixed; 
 pointer-events: none;
 top: 0; 
 left: 0; 
 width: 100vw; 
 height: 100vh; 
 background-color: white; 
 mix-blend-mode: difference; 
 z-index: 1; 
 ` 
 cover.setAttribute("style", css);
 document.body.appendChild(cover);
```
