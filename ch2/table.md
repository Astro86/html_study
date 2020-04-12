# 02 - 4장 표를 만드는 태그

> table-1.html
```html
<!DOCTYPE html>
<html lang="ko">
<head>
	<meta charset="utf-8">
	<title>표 만들기</title>
	<style>
		td {
			padding:5px;  /* 셀 테두리와 내용 사이의 간격(패딩) */
		}
	</style>
</head>
<body>
	<table border="1">
		<tr>
			<th> 제목 셀 </th>
			<td> 1행 2열 </td>
			<td> 1행 3열 </td>
		</tr>
		<tr>
			<th> 제목 셀 </th>
			<td> 2행 2열 </td>
			<td> 2행 3열 </td>
		</tr>
	</table>

</body>
</html>
```

> table-2.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>표 만들기</title>
	<style>
		th {
			padding:15px;   /* 셀 테두리와 내용 사이의 간격(패딩) */
		}
	</style>
</head>
<body>
	<table border="1">
		<colgroup>
			<col style="width:100px;">
			<col style="width:300px;">
			<col style="width:100px;">
			<col style="width:300px;">
		</colgroup>
		<tr>
			<th>이름</th>
			<td></td>
			<th>연락처</th>
			<td></td>
		</tr>
		<tr>
			<th>주소</th>
			<td colspan="3"></td>
		</tr>		
		<tr>
			<th>자기소개</th>
			<td colspan="3"></td>
		</tr>
	</table>
</body>
</html>
```

> table-3.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
	<meta charset="utf-8">
	<title>표 만들기</title>
	<style>
		td, th {
			padding:10px;   /* 셀 테두리와 내용 사이의 간격(패딩) */
		}
	</style>
</head>
<body>	
	<table border="1">
		<caption>
			<strong>Modern Browser</strong>
			<p>국내에서 자주 사용하는 모던 브라우저</p>
		</caption>
		<tr>
			<th>브라우저</th>
			<th>제조업체</th>
			<th>다운로드</th>
		</tr>
		<tr>
			<th>크롬(Chrome)</th>
			<td>Google</td>
			<td>https://www.google.com/chrome/ </td>
		</tr>
		<tr>
			<th>파이어폭스(Firfox)</th>
			<td>Mozilla</td>
			<td>https://www.mozilla.org/ko/firefox/</td>
		</tr>
		<tr>
			<th> 엣지(Edge) </th>
			<td> Microsoft </td>
			<td>https://www.microsoft.com/ko-kr/windows/microsoft-edge</td>
		</tr>
	</table>

</body>
</html>
```

> table-4.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
	<meta charset="utf-8">
	<title>표 만들기</title>
	<style>
		td, th {
			padding:10px;   /* 셀 테두리와 내용 사이의 간격(패딩) */
		}
	</style>
</head>
<body>	
	<figure>
		<figcaption>
			<p>국내에서 자주 사용하는 <b>모던 브라우저</b></p>
		</figcaption>
		<table border="1">
			<tr>
				<th>브라우저</th>
				<th>제조업체</th>
				<th>다운로드</th>
			</tr>
			<tr>
				<th>크롬(Chrome)</th>
				<td>Google</td>
				<td>https://www.google.com/chrome/ </td>
			</tr>
			<tr>
				<th>파이어폭스(Firfox)</th>
				<td>Mozilla</td>
				<td>https://www.mozilla.org/ko/firefox/</td>
			</tr>
			<tr>
				<th> 엣지(Edge) </th>
				<td> Microsoft </td>
				<td>https://www.microsoft.com/ko-kr/windows/microsoft-edge</td>
			</tr>
		</table>
	</figure>
</body>
</html>
```

> html-5.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
	<meta charset="utf-8">
	<title>표 만들기</title>
	<style>
		td, th {
			padding:10px;  /* 셀 테두리와 내용 사이의 간격(패딩) */
		}
	</style>
</head>
<body>	
	<p id="summary">다음 표는 HTMl5를 지원하는 모던(Modern Browser)를 정리한 것입니다. 최신 버전일수록 HTML5를 좀더 많이 지원하기 때문에 최신 버전을 다운로드하는 것이 좋습니다. </p>
	<table border="1" aria-describedby="summary">
		<caption>Modern Browser</caption>
		<tr>
			<th>브라우저</th>
			<th>제조업체</th>
			<th>다운로드</th>
		</tr>
		<tr>
			<th>크롬(Chrome)</th>
			<td>Google</td>
			<td>https://www.google.com/chrome/ </td>
		</tr>
		<tr>
			<th>파이어폭스(Firfox)</th>
			<td>Mozilla</td>
			<td>https://www.mozilla.org/ko/firefox/</td>
		</tr>
		<tr>
			<th> 엣지(Edge) </th>
			<td> Microsoft </td>
			<td>https://www.microsoft.com/ko-kr/windows/microsoft-edge</td>
		</tr>
	</table>
</body>
</html>
```

> table-6.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>표 만들기</title>
	<style>
		th, td {
			width:80px;  /* 셀의 너비 */
			padding:10px; /* 셀 테두리와 내용 사이의 간격(패딩) */
		}
		thead, tfoot { 
			background : #eeeeee;  /* thead와 tfoot의 배경 색 */
		}
	</style>
</head>
<body>
	<table border="1">
		<caption>제주특별자치도 학교현황(2015.4.1 기준)</caption>
		<thead>
			<tr>
				<th>구분</th>
				<th>학교수</th>
				<th>학급수</th>
				<th>학생수</th>
				<th>교원수</th>
			</tr>
		</thead>
		<tbody>
			<tr>
				<th>유치원</th>
				<td>117</td>
				<td>252</td>
				<td>5,547</td>
				<td>474</td>
			</tr>
			<tr>
				<th>초등학교</th>
				<td>111</td>
				<td>1,720</td>
				<td>37,686</td>
				<td>2,632</td>
			</tr>
			<tr>
				<th>중학교</th>
				<td>44</td>
				<td>699</td>
				<td>21,274</td>
				<td>1,412</td>
			</tr>
			<tr>
				<th>고등학교</th>
				<td>29</td>
				<td>676</td>
				<td>22,019</td>
				<td>1,433</td>
			</tr>
			<tr>
				<th>특수학교</th>
				<td>3</td>
				<td>90</td>
				<td>428</td>
				<td>160</td>
			</tr>
		</tbody>
		<tfoot>
			<tr>
				<th>합계</th>
				<td>300</td>
				<td>3,437</td>
				<td>86,954</td>
				<td>6,111</td>
			</tr>
		</tfoot>
	</table>
</body>
</html>
```

> colgroup.html
```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>표 만들기</title>
	<style>
		td {
			width:100px;  /* 셀 너비 */
			height:30px;  /* 셀 높이 */
		}

	</style>
</head>
<body>
	<table border="1">
		<caption>colgroup 연습</caption>
		<colgroup>
			<col>
			<col span="2" style="background-color:blue;">
			<col style="background-color:yellow">
		</colgroup>
		<tr>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td></td>
			<td></td>
			<td></td>
			<td></td>
		</tr>
	</table>
</body>
</html>
```