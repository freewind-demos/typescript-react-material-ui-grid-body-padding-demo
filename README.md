TypeScript React "material-ui" Grid Body Padding Demo
=========================================

一个Grid container如果设置了`spacing={1}`，它的width会被设置为`calc(100% + 16)`，所以有可能超出外层的区域。

如果放在一个body中，则可能右侧有一部分会跑到屏幕外，不太好。

我目前找到的做法是，手动给外层body的width设置为:

```
width: calc(100% - 16)
```

让它们互相抵消。

```
npm install
npm run demo
```

