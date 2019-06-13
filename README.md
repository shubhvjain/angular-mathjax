## AngularMathjax

[Demo](https://shubhvjain.github.io/angular-mathjax/)

In this project i have implemented [Mathjax](https://www.mathjax.org) with Angular 6. 

I have created a component `mathjax` that take `content` as math input. It also allows to load (typeset) math dynamically.


This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 6.0.8.


### Process 

**Step 1** Include Mathjax CDN in index.html and store mathjax object in the `window` object. 
Make sure to do this before loading the angular app.
                                              
```
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>AngularMathjax</title>
  <base href="/">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="icon" type="image/x-icon" href="favicon.ico">
  <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.2/MathJax.js?config=TeX-MML-AM_CHTML"></script>
  <script>
    window.MathJax = MathJax;
  </script>
</head>
<body>
  <app-root></app-root>
</body>
</html>

```

**Step 2**  Create the `mathjax` component (see /src/app/mathjax). This component take `content` as input and renders it. 