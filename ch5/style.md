# 05-1장 스타일과 스타일 시트

> css-comment.html

```html
<!doctype html>
<html lang="ko">
	<head>
		<meta charset="utf-8">
		<title>CSS 적용해 보기</title>
    <style>
      /* h2 제목과
        텍스트 단락의 
        스타일을 조절해 보자
      */
      h2{
        font-size:20px;  /* 글자 크기 20픽셀 */
        color:orange;  /* 글자색 오렌지 */
      }
      p {
        color:blue;   /* 글자색 파랑 */
      }
    </style>
	</head>
	<body>
		<h1>CSS</h1>
		<h2>웹 문서의 디자인과 내용을 분리합니다</h2>
		<p>웹 표준에 의한 웹 문서는 디자인과 내용이 분리되어 있습니다.</p>
		<p>내용은 HTML을 이용해 구성하고, 디자인은 CSS를 이용해 꾸미는 것입니다.</p>
	</body>
</html>
```

> internal.html

```html
<!DOCTYPE html>

<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>내부 스타일시트</title>
    <style>
      ul {
        color:blue; /* 목록의 글자색 */
        list-style-type:square; /* 불릿 형태 : 사각형 */
      }
    </style>
</head>
<body>
  <img src="images/sydney.png" alt="시드니 오페라 하우스">
  <h1>세계 3대 미항</h1>
  <ul>
    <li>시드니(Sydney), 호주</li>
    <li>리우데자네이루(Rio de Janeiro), 브라질</li>
    <li>나폴리(Naples), 이탈리아</li>
  </ul>
</body>
</html>
```

> external.html

```html
<!DOCTYPE html>

<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>내부 스타일시트</title>
    <link href="style.css" rel="stylesheet" type="text/css">
</head>
<body>
	<img src="images/sydney.png" alt="시드니 오페라 하우스">
  <h1>세계 3대 미항</h1>
  <ul>
    <li>시드니(Sydney), 호주</li>
    <li>리우데자네이루(Rio de Janeiro), 브라질</li>
    <li>나폴리(Naples), 이탈리아</li>
  </ul>
</body>
</html>
```

> style.css

```css
ul {
color:blue;
list-style-type:square;
}
```

> inline.html

```html
<!DOCTYPE html>

<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>인라인스타일</title>
</head>
<body>
  <h1>블루베리와 항산화 효능</h1>
  <p style="color:blue;"> 블루베리는 항산화제인 안토시아닌과 폴리페놀을 다량 포함하고 있습니다.</p>
  <p> 매사츄세츠 보스톤에 있는 USDA 노화에 관한 인류 영양 연구센터 (the USDA Human Nutrition Research Center on Aging) 의 자료에 의하면
   블루베리는 과일 중에서 가장 항산화 작용이 뛰어난 과일이라고 합니다.  </p>
</body>
</html>
```