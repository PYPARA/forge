## update
直接使用 jsencrypt , 他本身支持生成密钥
```js
var crypt = new JSEncrypt({ default_key_size: 2048 }); 
var keypair = {
  PublicKey: crypt.getPublicKey(), 
  PrivateKey: crypt.getPrivateKey()
};
```

## log
使用 github上 jsencrypt 和 forge 库
原版 jsencrypt 不兼容 IE
forge 兼容IE

## jsencrypt 有京东使用的 IE 兼容版本
jdJsencrypt.min.js
https://passport.jd.com/new/js/jdJsencrypt.min.js

## 兼容 Promise
es6-promise.min.js

```js
if (!("Promise" in window)) {
  Promise = ES6Promise
}
```

