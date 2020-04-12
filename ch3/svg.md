# 03 - 3장 SVG 이미지

> insert-svg.html

```html
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>Insert SVG</title>
  </head>
  <body>
    <h1>SVG 이미지 삽입하기</h1>
    <img src="images/muffin.svg" />
  </body>
</html>
```

> check-svg.html

```html
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>Insert SVG</title>
    <script src="modernizr-custom.js"></script>
  </head>
  <body>
    <h1>SVG 이미지 삽입하기</h1>
    <img src="images/muffin.svg" />
    <script>
      if (!modernizr.svg) {
        $("img").attr("src", "images/muffin.png");
      }
    </script>
  </body>
</html>
```
