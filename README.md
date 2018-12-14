# osagai-simple-router
A simple and tiny (520 Byte) router implemented with Osagai

## Install

```
npm install osagai osagai-simple-router
```

or import directly in your html using [unpkg.com](http://unpkg.com)

```html
<script src="//unpkg.com/osagai/osagai.umd.js"></script>
<script src="//unpkg.com/osagai-simple-router/dist/index.umd.js"></script>
```


## Usage

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width">
  <title>Osagai Simple Router</title>
</head>
<body>
  <div class="current-route"></div>
  <a href="/next">Go to next</a>

  <simple-router></simple-router>

  <script src="//unpkg.com/osagai/osagai.umd.js"></script>
  <script src="//unpkg.com/osagai-simple-router/dist/index.umd.js"></script>

  <script>
    const router = document.querySelector('simple-router')
    const currentRoute = document.querySelector('.current-route')

    router.addListener(route => {
      currentRoute.innerText = route
    });
  </script>
</body>
</html>
```
