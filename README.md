# liltools
![npm](https://img.shields.io/npm/v/liltools?style=plastic)
![npm bundle size](https://img.shields.io/bundlephobia/min/liltools?style=plastic)
![Requires.io](https://img.shields.io/requires/github/redline187/liltools?style=plastic)
![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/redline187/liltools?style=plastic)

[TOC]

### makeid()
generate random string

```js
function makeid(length) {
    var result           = '';
    var characters       = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789';
    var charactersLength = characters.length;
    for ( var i = 0; i < length; i++ ) {
      result += characters.charAt(Math.floor(Math.random() * 
 charactersLength));
   }
   return result;
}
```