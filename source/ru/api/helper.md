---
title: Помощник
---
Помощник позволяет легко и быстро добавлять фрагменты кода в шаблоны. Мы рекомендуем использовать помощников в шаблонах, когда вы имеете дело со сложным кодом.

## Краткий обзор

``` js
hexo.extend.helper.register(name, function(){
  // ...
});
```

## Пример

``` js
hexo.extend.helper.register('js', function(path){
  return '<script src="' + path + '"></script>';
});
```

``` js
<%- js('script.js') %>
// <script src="script.js"></script>
```
