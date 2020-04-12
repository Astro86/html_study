# 03-1장 이미지

> img-1.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>추천 관광지</title>
</head>
<body>
	<h1>사려니 숲길</h1>
	<img src="images/road.jpg" alt=""> 
</body>
</html>
```

> img-2.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>추천 관광지</title>
</head>
<body>
	<h1>사려니 숲길</h1>
	<img src="images/road.jpg" alt="사려니 숲길">
	<img src="images/road.jpg" width="250" height="90" alt="사려니 숲길">	
</body>
</html>
```

> figcaption.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>추천 관광지</title>
</head>
<body>
	<h1>제주의 오름</h1>
	<p>거인 설문대할망이 제주도와 육지 사이에 다리를 놓으려고 치마폭에 흙을 담아 나를 때 치마 틈새로 한줌씩 떨어진 흙덩이들이 오름이 되었다는 전설이 있다. </p>
	<figure>
		<img src="images/oreum-1.jpg" alt="용눈이 오름">
		<figcaption>완만하고 부드러운 용눈이 오름</figcaption>
	</figure>
</body>
</html>
```

> index-img-result

```html
<!doctype html>
<html lang="ko">

<head>
	<title>온라인 프로필</title>
	<meta charset="utf-8">
	<style>
		table,th,td {
			border: 1px solid black; /* 표의 테두리 - 1px 회색 실선 */
			border-collapse: collapse;  /* 표 테두리와 셀 테두리 합치기 */
		}		
		th,td {
			padding: 15px; /* 셀 패딩(테두리와 내용 사이의 여백) */
		}
	</style>
</head>

<body>
	<figure>
		<img src="images/pf.png" alt="">
		<figcaption>오늘은 남은 인생이 시작되는 첫째날</figcaption>
	</figure>
	<h1>Kyunghee Ko</h1>
	<p>이메일 : funcom@gmail.com</p>
	<br><br>
	<h2>Who I am?</h2>
	<p>프런트엔드 웹 기술(Front-end Web Tech.)에 관심을 가지고 있습니다.<br> 현재 마이크로소프트 공인 최고기술전문가(Most Valuable Professional)로 활동 중이며,<br> 제주의 한
		시골 마을에서 코딩 중입니다.</p>
	<hr>
	<h2>Skills</h2>
	<ul>
		<li>
			사용 언어
			<ul>
				<li><mark>HTML</mark></li>
				<li><mark>CSS</mark></li>
				<li>Javascript</li>
				<li>AngularJS</li>
			</ul>
		</li>
		<li>
			사용 툴
			<ul>
				<li>Photoshop(12years)</li>
				<li>Dreamweaver(19years)</li>
				<li><b>Visual Studio(5years)></b></li>
			</ul>
		</li>
	</ul>
	<h2>Academic</h2>
	<table>
		<caption>학력 사항</caption>
		<thead>
			<tr>
				<th>출신학교</th>
				<th>전공</th>
				<th>기간</th>
				<th>졸업구분</th>
			</tr>
		</thead>
		<tbody>
			<tr>
				<td>ㅇㅇㅇ고등학교</td>
				<td> (해당사항 없음)</td>
				<td>2001.3 ~ 2004.2</td>
				<td>졸업</td>
			</tr>
			<tr>
				<td>ㅁㅁ대학교</td>
				<td>컴퓨터공학</td>
				<td>2004.3 ~ 2008.2</td>
				<td>졸업</td>
			</tr>
		</tbody>
	</table>
</body>

</html>
```