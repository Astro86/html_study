# 02 - 3장 목록을 만드는 태그

> ul.html

```html
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>제주 관광 안내</title>
  </head>
  <body>
    <h1>관광 안내 전화</h1>
    <p>
      한국관광공사에서는 전국의 관광안내소와 공동으로 여러분의 여행편의를 위해
      관광안내전화 1330 서비스를 연중무휴 실시하고 있습니다.
    </p>
    <p>
      1330에는 해당 지역의 지도와 관광 가이드북, 관광안내소를 대신할 수 있을
      정도의 다양한 정보가 있습니다. 원하는 관광지는 물론이며 숙박, 교통, 음식점
      등의 자세한 정보를 한국어를 비롯한 영어, 중국어, 일어의 3개 국어로도 이용
      가능합니다.
    </p>
    <ul>
      <li>일반 전화 : (국번없이) 1330</li>
      <li>휴대 전화 : 064-1330</li>
    </ul>
  </body>
</html>
```

> ol.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
	<meta charset="utf-8">
	<title>1박 2일 가족 여행 코스</title>
</head>
<body>
	<h1>1박 2일 가족 여행 코스</h1>
	<ul>
		<li>1일차
			<ol type="a">
				<li>해녀박물관</li>
				<li>낚시체험</li>
			</ol>
		</li>
		<li>2일차
			<ol type="a" start ="3">
				<li>용눈이오름</li>
				<li>만장굴</li>
				<li>카약체험</li>
			</ol start>
		</li>
	</ul>

</body>
</html>
```

> dl.html

```html
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>제주 올레</title>
    <style>
      dl {
        line-height: 25px; /* 줄 간격 */
      }
    </style>
  </head>
  <body>
    <h1>제주 올레</h1>
    <dl>
      <dt>올레 1코스</dt>
      <dd>코스 : 시흥 초등학교 옆 - 광치기 해변</dd>
      <dd>거리 : 14.6km(4~5시간)</dd>
      <dd>난이도 : 중</dd>
      <dt>올레 2코스</dt>
      <dd>코스 : 광치기 해변 - 온평 포구</dd>
      <dd>거리 : 14.5km(4~5시간)</dd>
      <dd>난이도 : 중</dd>
    </dl>
  </body>
</html>
```
