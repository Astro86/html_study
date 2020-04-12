# 02 - 2장 텍스트를 한 줄로 표시하는 태그

> text-3.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>제주 이색 여행지</title>
    <style>
        p { 
            font-size:16px;  /* 글자 크기 */  
            line-height:25px;  /* 줄 간격 */
        }
    </style>
</head>
<body>
    <h2>제주 이색 여행지 - 이중섭 거리</h2>
    <p><strong>주말</strong>마다 <b>'서귀포문화예술디자인시장'</b>이 열립니다.</p>
    <p><em>'아트마켓'</em>이라고도 부르는데, <i>문화예술체험</i>이나 <i>공연관람</i>을 할 수도 있고 <br>
     작가들이 직접 만든 창작예술품 등을 판매하기도 합니다.</p>
</body>
</html>
```

> text-4.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
	<meta charset="utf-8">
	<title>웹 접근성(Web Accessibility)</title>
</head>
<body>
	<h1>웹 접근성</h1>
	<p>웹의 창시자인 팀 버너스 리 (Tim Berners-Lee)의 
        <q cite="http://www.w3.org/standards/webdesign/accessibility">웹의 힘은 보편성에 있다. 
        장애에 구애없이 모든 사람이 접근할 수 있는 것이 필수적인 요소이다.</q>
        라는 말로 웹 접근성을 설명한다. 
    </p>
</body>
</html>
```

> text-5.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>제주 이색 여행지</title>
</head>
<body>
    <h2>야외 텐트를 닮은 건축물 <mark>"테쉬폰"</mark></h2>
    <p>아일랜드 출신 임피제 신부가 1954년 제주에 오면서 목장 숙소로 짓기 시작한 후 사료공장, 성당으로 활용됐습니다. 
        제주에서 점차 다른 지방으로 보급됐지만 현재 제주에만 건축물이 남아있으며, 
        <span style="color:blue;">국내 근현대 건축사의 한 페이지를 보여주는 가치를 지닌다</span>
        고 전문가들은 평가합니다.</p>
</body>
</html>
```

> text-6.html

```html
<!doctype html>
<html lang="ko">
	<head>
		<meta charset="utf-8">
		<title>Ruby</title>
	</head>
	<body>
		<p>루비(Ruby)는 1995년, 일본의 프로그래머인 마츠모토 유키히로 
            (<ruby>松本行弘<rt>まつもとゆきひろ</rt>)</ruby>
            가 만든 프로그래밍 언어입니다.</p>
	</body>	
</html>
```