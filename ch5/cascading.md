# 05-3장 캐스캐이딩 스타일 시트

> cascading1.html

```html
<!DOCTYPE html>

<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>캐스캐이딩 - 중요성</title>
    <style>
      p {
        font-style:italic;  /* 글자 스타일 */
        color:blue; /* 글자색 */
      }
      p {
        color:red !important; /* 글자색, 우선 적용 */
      }
    </style>
</head>
<body> 
  <h1>세계 3대 미항</h1>
  <img src="images/rio.png" alt="브라질 리우데자네이루">
  <p>시드니(Sydney), 호주</p>  
  <p>리우데자네이루(Rio de Janeiro), 브라질</p>
  <p>나폴리(Naples), 이탈리아</p>
</body>
</html>
```

> cascading2.html

```html
<!DOCTYPE html>

<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>캐스캐이딩</title>
    <style>
      h1 {
        color:blue;  /* 글자색 */
      }
      #habor{
        border:1px solid gray;  /* 테두리 - 1픽셀짜리 회색 실선 */
        padding:10px; /* 패딩 여백 - 테두리와 내용 사이의 여백 */
        color:green; /* 글자색 */
      }
      .heading {
        color:red; /* 글자색 */
      }
    </style>
</head>
<body> 
  <h1 class="heading" id="habor">세계 3대 미항</h1>
	<img src="images/rio.png" alt="브라질 리우데자네이루">
  <p>시드니(Sydney), 호주</p>  
  <p>리우데자네이루(Rio de Janeiro), 브라질</p>
  <p>나폴리(Naples), 이탈리아</p>
</body>
</html>
```

> inherit.html

```html
<!DOCTYPE html>

<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>뉴욕타임즈 10대 식품</title>
    <style>
      body {
        font-family:"돋움"; /* 글꼴 */
        color:darkgreen; /* 글자색 */
      }
    </style>
</head>
<body>
  <h1>뉴욕 타임즈에서 발표한 세계 10대 슈퍼푸드</h1>
  <ul>
    <li>블루베리</li>
    <li>귀리</li>
    <li>토마토</li>
    <li>시금치</li>
    <li>적포도주</li>
    <li>견과류</li>
    <li>브로콜리</li>
    <li>연어</li>
    <li>마늘</li>
    <li>녹차</li>
  </ul>
</body>
</html>
```