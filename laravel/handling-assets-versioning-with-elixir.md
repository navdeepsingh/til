# Handling assets versioning efficiently with Laravel Elixir

We understand this gulp elixir code
```
elixir(function(mix) {
    mix.version(['css/all.css', 'js/all.js']);
});
```
which generates
``` css
<link rel="stylesheet" href="/build/css/all-a2072b5556.css">
```

## Problem is :
This will not work as the browser will search for fontawesome-webfont.eot in “public/build/fonts” instead of “public/fonts” because your all-a2072b5556.css is living inside “public/build” folder instead of “public” folder!

## Solution :
Customizing “buildPath” (Laravel 5.2 only)
```
elixir(function(mix) {
    mix.version(['css/all.css', 'js/all.js'], 'public');
});
```
And
```
// Notice that we pass null as second argument 
<link rel="stylesheet" href="{{ elixir('css/all.css', null) }}">
```



