# 03 - 2장 링크

> link.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>링크 만들기</title>
</head>
<body>
	<h1>텍스트 링크 만들기</h1>
	<a href="http://www.easyspub.com">이지스퍼블리싱 홈페이지</a>
	<h1>이미지 링크 만들기</h1>
	<a href="http://www.easyspub.com">
		<img src="images/easyspub.jpg" alt="이지스퍼블리싱 홈페이지로 가기">
	</a>
</body>
</html>
```

> target.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>텍스트 링크</title>
	<style>
		a {
			text-decoration:none;
			color:black;
		}
	</style>
</head>
<body>
	<h1>텍스트 링크 만들기</h1>
	<p><a href="http://www.easyspub.com">이지스퍼블리싱 홈페이지(현재 화면)</a></p>
	<p><a href="http://www.easyspub.com" target="_blank">이지스퍼블리싱 홈페이지(새 창 또는 새 탭)</a></p>
</body>
</html>
```

> parent.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>프런트엔드 웹 디자인 입문</title>
	<style>
		body {
			text-align:center;
		}
		iframe {
			border:1px dotted gray;
		}
	</style>
</head>
<body>
	<h1>Do it! 프런트엔드 웹 디자인 입문 </h1>	
	<p>아래 화면은 iframe 태그를 이용해 외부 문서를 현재 문서에 삽입한 것입니다.</p>
	<br><br>
	<iframe src="child.html" width="600" height="400"></iframe>
</body>
</html>
```

> child.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>프런트엔드 웹 디자인 입문</title>
	<style>
		body {
			background-color:#ffffff  /* 문서 전체 배경색 */
		}
		img {
			float:left;  /* 왼쪽으로 배치 */
			margin-right:20px;  /* 이미지의 오른쪽 여백*/
		}
	</style>
</head>
<body>
	<img src="images\webd.png" alt="두잇, 프런트엔드 웹 디자인 입문">
	<br><br>
	<h2>코딩으로 만드는 웹 디자인</h2>	
	<p>HTML5 ․ CSS3 ․ jQuery로 웹 디자인 트렌드를 따라잡는 비법 대공개</p>
	<p>취업용 포트폴리오에 바로 써먹을 수 있는<br> 실전 웹 디자인 예제 수록</p>
	<p><a href="http://easyspub.co.kr/20_Menu/BookView/65">도서 상세 보기(현재 화면에)</a></p>
	<p><a href="http://easyspub.co.kr/20_Menu/BookView/65" target="_top">도서 상세 보기(전체 화면에)</a></p>
</body>
</html>
```

> anchor.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>링크 만들기</title>
</head>
<body>
	<h1>앵커 만들기</h1>
	<p>웹 문서가 너무 길 경우 필요한 곳마다 문서 안에 이름을 붙여놓고 그 위치로 한번에 이동하는 링크를 만들 수 있는데, 이 기능을 앵커(anchor)라고 합니다. </p>
	<ul id="menu">
		<li><a href="#content1">메뉴1</a></li>
		<li><a href="#content2">메뉴2</a></li>
		<li><a href="#content3">메뉴3</a></li>
	</ul>
	<h2 id="content1">내용1</h2>
	<p>웹 문서가 너무 길 경우 필요한 곳마다 문서 안에 이름을 붙여놓고 그 위치로 한번에 이동하는 링크를 만들 수 있는데, 이 기능을 앵커(anchor)라고 합니다. </p>
	<p>웹 문서가 너무 길 경우 필요한 곳마다 문서 안에 이름을 붙여놓고 그 위치로 한번에 이동하는 링크를 만들 수 있는데, 이 기능을 앵커(anchor)라고 합니다. </p>
	<p>웹 문서가 너무 길 경우 필요한 곳마다 문서 안에 이름을 붙여놓고 그 위치로 한번에 이동하는 링크를 만들 수 있는데, 이 기능을 앵커(anchor)라고 합니다. </p>
	<p><a href="#menu">[메뉴로]</a></p>
	<h2 id="content2">내용2</h2>
	<p>웹 문서가 너무 길 경우 필요한 곳마다 문서 안에 이름을 붙여놓고 그 위치로 한번에 이동하는 링크를 만들 수 있는데, 이 기능을 앵커(anchor)라고 합니다. </p>
	<p>웹 문서가 너무 길 경우 필요한 곳마다 문서 안에 이름을 붙여놓고 그 위치로 한번에 이동하는 링크를 만들 수 있는데, 이 기능을 앵커(anchor)라고 합니다. </p>
	<p>웹 문서가 너무 길 경우 필요한 곳마다 문서 안에 이름을 붙여놓고 그 위치로 한번에 이동하는 링크를 만들 수 있는데, 이 기능을 앵커(anchor)라고 합니다. </p>
	<p><a href="#menu">[메뉴로]</a></p>
	<h2 id="content3">내용3</h2>
	<p>웹 문서가 너무 길 경우 필요한 곳마다 문서 안에 이름을 붙여놓고 그 위치로 한번에 이동하는 링크를 만들 수 있는데, 이 기능을 앵커(anchor)라고 합니다. </p>
	<p>웹 문서가 너무 길 경우 필요한 곳마다 문서 안에 이름을 붙여놓고 그 위치로 한번에 이동하는 링크를 만들 수 있는데, 이 기능을 앵커(anchor)라고 합니다. </p>
	<p>웹 문서가 너무 길 경우 필요한 곳마다 문서 안에 이름을 붙여놓고 그 위치로 한번에 이동하는 링크를 만들 수 있는데, 이 기능을 앵커(anchor)라고 합니다. </p>
	<p><a href="#menu">[메뉴로]</a></p>
</body>
</html>
```

>map.html

```html
<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>이미지맵</title>
	<style>
		a {
			text-decoration:none
		}
	</style>
</head>

<body>
<img src="images/kids.jpg"  alt="" usemap="#favorites">
<map name="favorites">
  <area shape="rect" coords="10,10,160,200" href="http://cafe.naver.com/doithtml5" target="_blank" alt="do it html5 네이버 카페로 가기">
  <area shape="rect" coords="220,10,380,200" href="http://www.facebook.com/do.it.html5" target="_blank" alt="do it html5 페이스북 페이지로 가기">
</map>
</body>
</html>
```

> index-link-result.html

```html
<!doctype html>
<html lang="ko">

<head>
	<title>온라인 프로필</title>
	<meta charset="utf-8">
	<style>
		table,th,td {
			border: 1px solid black; 
			border-collapse: collapse; 
		}		
		th,td {
			padding: 15px; 
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
	<h2>Who I am?</h2>
	<p>프런트엔드 웹 기술(Front-end Web Tech.)에 관심을 가지고 있습니다.<br> 현재 마이크로소프트 공인 최고기술전문가(Most Valuable Professional)로 활동 중이며,<br> 제주의 한
		시골 마을에서 코딩 중입니다.</p>
	<h2>SNS</h2>
	<ul>
		<li><a href="https://www.facebook.com/funnycom" target="_blank">facebook</a></li>
		<li><a href="https://www.twitter.com/funnycom" target="_blank">twitter</a></li>
	</ul>
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