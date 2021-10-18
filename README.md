## :joystick: Classic DOOM on console!

[Play it now](https://carlos18mz.github.io/classic-doom/).

<br>


![alt text](https://github.com/carlos18mz/classic-doom/blob/c1ecfa392604f4de4d7dd4ec44e9881af362b514/preview.png?raw=true)


```js
const forwardKey = (e, type) => {
  const ev = new KeyboardEvent(type, {
    key: e.key,
    keyCode: e.keyCode,
  });
  canvas.dispatchEvent(ev);
};
document.body.addEventListener("keydown", (e) => forwardKey(e, "keydown"));
document.body.addEventListener("keyup", (e) => forwardKey(e, "keyup"));
```
```js
const base64Image = canvas.toDataURL().replace(/(\r\n|\n|\r)/gm, "");
console.log(
  "%c X",
  `font-size:400px;color: transparent;background:url(${base64Image}) no-repeat; background-size: contain;margin-top: 140px;margin-left: 60px;`
);
```
```bash
python App.py
```
