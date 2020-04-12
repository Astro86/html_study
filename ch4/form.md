# 04-1장 폼 만들기

> form.html

```html
<!DOCTYPE html>

<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>HTML5 폼</title>
</head>
<body>
	<form action="search.php" method="post">
		<input type="text" title="검색">
		<input type="submit" value="검색">
	</form>
</body>
</html>
```

> label.html

```html
<!DOCTYPE html>

<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>label 태그 사용</title>
		<style>
			ul {
				list-style:none;  /* 불릿 없앰 */
			}
			li {
				margin:20px;  /* 각 항목간 마진 */
			}
			li label {   
				width:70px;   /* 레이블 너비 */
				float:left;  /* 왼쪽부터 시작 */
				font-size:14px;  /* 글자 크기 */
				font-weight:bold;  /* 글자 굵기 */
				line-height:25px;  /* 줄간격 */
			}
		</style>
</head>
<body>
	<form action="login.php" method="post">
		<ul>
			<li>
				<label for="id">아이디</label>
				<input type="text" id="id">
			</li>
			<li>
				<label for="pw">비밀번호</label>
				<input type="password" id="pw">
			</li>
			<li>				
				<input type="submit" title="로그인" value="로그인">
			</li>
		</ul>
	</form>
</body>
</html>
```

> withlabel.html

```html
<!DOCTYPE html>

<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>label 태그 사용</title>
		<style>
			ul {
				list-style:none;
			}
			li {
				margin:20px;
			}
		</style>
</head>
<body>
	<form>
		<h3>수강 분야(다수 선택 가능)</h3>
		<ul>
			<li>
				<input type="checkbox" value="grm">문법
			</li>
			<li>
				<input type="checkbox" value="wr">작문
			</li>
			<li>
				<input type="checkbox" value="rd">독해
			</li>
		</ul>
		<h3>수강 과목(1과목만 선택 가능)</h3>
		<ul>
			<li>
				<label><input type="radio" name="subject" value="eng">영어회화</label>
			</li>
			<li>
				<label><input type="radio" name="subject" value="ch">중국어회화</label>
			</li>
			<li>				
				<label><input type="radio" name="subject" value="jp">일어회화</label>
			</li>
		</ul>
	</form>
</body>
</html>
```

> fieldset.html

```html
<!DOCTYPE html>

<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>filedset과 legend 태그</title>
		<style>
			ul {
				list-style:none;
			}
			li {
				margin:20px;
			}
			li label {
				width:80px;
				float:left;
			}
			fieldset {
				margin:15px;
			}
		</style>
</head>
<body>
	<form>
		<fieldset>
			<legend>개인 정보</legend>
			<ul>
				<li>
					<label for="name">이름</label>
					<input type="text" id="name">
				</li>
				<li>
					<label for="mail">메일 주소</label>
					<input type="text" id="mail">
				</li>
			</ul>
		</fieldset>		
		<fieldset>
			<legend>로그인 정보</legend>
			<ul>
				<li>
					<label for="id">아이디</label>
					<input type="text" id="id">
				</li>
				<li>
					<label for="pwd">비밀번호</label>
					<input type="text" id="pwd">
				</li>
			</ul>
		</fieldset>
	</form>
</body>
</html>
```