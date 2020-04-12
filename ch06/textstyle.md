# 06-2장 텍스트 스타일

> color.html

```html
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>뉴욕타임즈 10대 식품</title>
    <style>
      h1 {
        color: rgb(0, 200, 0);
      } /* rgb 값 사용 - 녹색 계열 */
      h2 {
        color: blue;
      } /* 색상 이름 사용 - 파랑 */
      .accent {
        color: #f00;
      } /* 16진수 사용 - 빨강, #ff0000으로도 사용 */
      img {
        float: right; /* 오른쪽 정렬 */
        margin-right: 10px; /* 오른쪽 마진 여백 */
      }
    </style>
  </head>
  <body>
    <h1>세계 10대 슈퍼푸드</h1>
    <img src="images/galic.jpg" />
    <h2>마늘(Garlic)</h2>
    <p>
      일해백리(一害百利)는 마늘의 별명이다. 한가지 해가 있고 백가지 이로움이
      있다는 뜻이다. 그 한 가지 해란, 아린 맛으로 인해 위에 부담을 준다는
      것이다.
    </p>
    <p>
      마늘 특유의 아린 맛은 <span class="accent">알리신</span>이라는 성분
      때문으로, 살균 및 항균 작용을 하며 마늘에 들어 있는 아연이 피로 회복에
      도움을 준다.
    </p>
  </body>
</html>
```

> text-decoration.html

```html
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>뉴욕타임즈 10대 식품</title>
    <style>
      a {
        text-decoration: none;
      } /* 밑줄 없앰 */
      .edited {
        text-decoration: line-through;
      } /* 취소선 */
    </style>
  </head>
  <body>
    <h2>토마토(Tomato)</h2>
    <p>
      [<a href="https://www.fitbug.com/g/Superfoods-tomatoes" target="_blank"
        >외부 링크</a
      >]
    </p>
    <p>
      토마토는 비타민A, C가 풍부한 <span class="edited">과일이다.</span> 채소다.
      칼륨과 같은 각종 미네랄은 혈액의 산성도를 낮추는 역할을 해주며 혈압을
      내리고 혈관을 튼튼하게 해준다. 토마토에 들어있는 피코펜이라는 성분은
      뛰어난 항암 작용을 보이며 잘 알려져 있듯이 블루베리와 함께 대표적인 항산화
      음식이기도 하다.
    </p>
  </body>
</html>
```

> text-transform.html

```html
<!DOCTYPE html>
<li lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>text-transform</title>
    <style>
      .trans1 {
        text-transform: uppercase;
      } /* 대문자로 */
      .trans2 {
        text-transform: capitalize;
      } /* 첫글자만 대문자로 */
    </style>
  </head>
  <body>
    <h1>Have to study</h1>
    <ul>
      <li class="trans1">html</li>
      <li class="trans1">css</li>
      <li class="trans2">javascript</li>
    </ul>
  </body>
</li>
```

> text-shadow1.html

```html
<!DOCTYPE html>
<body lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>text-transform</title>
    <style>
      h1 {
        font-size: 100px; /* 글자 크기 */
        font-family: "Arial Rounded MT"; /* 글꼴 */
      }
      .shadow1 {
        color: orange; /* 글자색 */
        text-shadow: 1px 1px; /* 텍스트 그림자 */
      }
      .shadow2 {
        text-shadow: 5px 5px 3px #f00; /* 텍스트 그림자 */
      }
      .shadow3 {
        color: #fff; /* 글자색 */
        text-shadow: 7px -7px 5px #000; /* 텍스트 그림자 */
      }
    </style>
  </head>
  <body>
    <h1 class="shadow1">HTML5</h1>
    <h1 class="shadow2">HTML5</h1>
    <h1 class="shadow3">HTML5</h1>
  </body>
</body>
```

> text-shadow2.html

```html
<!DOCTYPE html>
<head lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>text-transform</title>
    <style>
      body {
        background: #222;
      } /* 문서 배경색 */
      h1 {
        font-size: 80px; /* 글자 크기 */
        font-family: "Arial Rounded MT"; /* 글꼴 */
        letter-spacing: 4px; /* 자간 */
      }
      .shadow3 {
        color: #000; /* 글자색 */
        text-shadow: 0 0 4px #ccc, 0 -5px 4px #ff3, 2px -10px 6px #fd3, -2px -15px
            11px #f80, 2px -19px 18px #f20; /* 텍스트 그림자 */
      }
    </style>
  </head>
  <body>
    <h1 class="shadow3">HTML5</h1>
  </body>
</head>
```

> letter-spacing.html

```html
<!DOCTYPE html>
<h1 lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>letter-spacing와 word-spacing</title>
    <style>
      h1 {
        font-size: 40px;
      } /* 글자 크기 */
      .letter1 {
        letter-spacing: 0.2em; /* 자간 */
      }
      .letter2 {
        letter-spacing: 0.5em; /* 자간 */
      }
    </style>
  </head>
  <body>
    <h1>HTML5</h1>
    <h1 class="letter1">HTML5</h1>
    <h1 class="letter2">HTML5</h1>
  </body>
</h1>
```
