# Markdown Support for Documentation based on git deployment

+ [Markdown rendering for Softreck.Dev  - md.softreck.dev](https://md.softreck.dev)
+ [Markdown rendering for Softreck.Dev  - on github](https://softreck.github.io/md/)

## How to use?
just copy [index.html](index.html), and he take  README.md and render it in your project


      <!-- Use external markdown resource, separate slides by three newlines; vertical slides by two newlines -->
      <section data-markdown="README.md" data-separator="^\n\n\n" data-separator-vertical="^\n\n"></section>





### Rozwiązania

pobieranie pliku json z URL możliwość kontroli procesu poprzez funkcję succes w przypadku poprawnego pobrania oraz error, gdy plik nie istnieje, lub nie ma odpowiedniego formatu

#### Osobne callback-i do pozytywnego i negatywnego przypadku

```php 
letJson( String  url, Function  success, Function  error)     
```

#### Metoda try - catch, bez callback, do error

```php
try{
    letJson( String  url, Function  json, Function  item)     
}catch(){

}
```   

### Przykłady użycia

#### 1. użycie z adresem url, callback: success, error

```js
letJson(
    "get.domain.com/file.json",
    function(name, value, json) {

    },
    function(error) {

    }
);
```


---  

+ [edit source](https://github.com/softreck/md/edit/main/README.md),  [README.md](https://github.com/softreck/md/blob/main/README.md)
