# 04-2장 사용자 입력을 위한 <input> 태그

> id-pw.html

```html
<!doctype html>

<html lang="ko">
  <head>
		<meta charset="utf-8">
		<title> 웹 폼</title>
    <style>
		 label {
			font-size:14px; /* 글자 크기 */
			line-height:25px;  /* 줄 간격 */
		 }
		 label em{
			color:red;  /* 글자색 */
			font-weight:800; /* 글자 굵기 */ 
		 }
	 </style>
  </head>
  <body>
	<form>
    <fieldset>
    	<label>아이디: <input type="text" id="user_id" size="10"></label>
      <label>비밀번호: <input type="password" id="user_pw" size="10"></label>
      <input type="submit" value="로그인">
    </fieldset>
  </form>
  </body>
</html>
```

> url-email-tel.html

```html
<!doctype html>

<html lang="ko">
  <head>
		<meta charset="utf-8">
		<title> 웹 폼</title>
    <style>
		 ul {
			 list-style:none;
		 }
		 li {
			 margin:10px;
		 }
		 li label {
			 width:120px;
			float:left;
			text-align:right;
			padding-right:8px;
		 }
		 input[type="submit"] {
			 text-align:center;
			 width:100%;
			 height:30px;
			 margin-top:15px;
		 }
	 </style>
  </head>
  <body>
		<h1>회원 가입</h1>
		<form>
			<fieldset>
				<legend>로그인 정보</legend>
				<ul>
					<li>
    				<label for="user-id">아이디 </label>
						 <input type="text" id="user-id">
					</li>
					<li>
						<label for="pwd1">비밀번호 </label>
						<input type="password" id="pwd1">
					</li>
					<li>
						<label for="pwd2">비밀번호 확인 </label>
						<input type="password" id="pwd2">				
					</li>
				</ul>
			</fieldset>
			<fieldset>
				<legend>개인 정보</legend>
				<ul>
					<li>
						<label for="user-name">이름 </label>
						<input type="text" id="user-name">
					</li>
					<li>
						<label for="mail">메일 주소</label>
						<input type="email" id="mail">
					</li>
					<li>
						<label for="phone">연락처</label>
						<input type="tel" id="phone">
					</li>
					<li>
						<label for="homep">블로그/홈페이지</label>
						<input type="url" id="homep">
					</li>
				</ul>
			</fieldset>
			<input type="submit" value="가입하기">
		</form>
  </body>
</html>
```

> number-range.html

```html
<!doctype html>
<html lang="ko">
  <head>
		 <meta charset="utf-8">
     <title> 웹 폼</title>
     <style>
			 body {
				background-color:#fff; 
			 }
			 form legend{
				font-size:15px;
				font-weight:600; 
			 }
			 form label.reg {
				font-size:14px;
				width:150px;
				float:left;
			 }
			 form ul li{
				list-style:none; 
				margin: 15px 0;		
			 }
			 #member, #stuffs {
				width:50px; 
			 }
	 </style>
  </head>
  <body>
	<form>
	  <fieldset>
	    <legend> 등록 정보</legend>
    	  <ul>
	        <li>
            	   <label class="reg" for="member">참여인원<small>(최대10명)</small></label>
                <input type="number" id="member" value="1" min="0" max="10" step="1">
              </li>
              <li>
            	   <label class="reg" for="stuffs">지원물품<small>(1인당 5개)</small></label>
                <input type="number" id="stuffs" value="1" min="0" max="50" step="5" size="5">
              </li>
        	  <li>
            	   <label class="reg" for="satis">희망 단계<small>(하,중,상)</small></label>
                <input type="range" id="satis" value="1" min="1" max="3">
              </li>           
            </ul>
       </fieldset>
  </form>
  </body>
</html>
```

> radio-checkbox.html

```html
<!doctype html>
<html lang="ko">
  <head>
		<meta charset="utf-8">
     <title> 웹 폼</title>
     <style>
	 body {
		background-color:#fff; 
	 }
	 form fieldset{
		margin-bottom:25px; 
	 }	 
	 form legend{
		font-size:15px;
		font-weight:600; 
	 }
	 form label.reg {
		font-size:14px;
		color:#390;
		font-weight:bold;
		width:110px;
		float:left;
		text-align:right;
		margin-right:10px;
	 }
	 form ul li{
		list-style:none; 
		margin: 15px 0;	
		font-size:14px;	
	 }
 

	 #member, #stuffs {
		width:50px; 
	 }
	 
	 #pre {
		margin-left:15px;
	 }
	 </style>
  </head>
  <body>
	<form>
		<fieldset>
			<legend>신청 과목</legend>
			<p>이 달에 신청할 과목을 선택하세요 (1과목만 가능)</p>
			<label><input type="radio" name="subject" value="speaking">회화</label>
			<label><input type="radio" name="subject" value="grammar">문법</label>
			<label><input type="radio" name="subject" value="writing">작문</label>       
		</fieldset>
		<fieldset>
			<legend>메일링</legend>
			<p>메일로 받고 싶은 뉴스 주제를 선택해 주세요 (복수 선택 가능)</p>
			<label><input type="checkbox" name="mailing1" value="news">해외 단신</label>
			<label><input type="checkbox" name="mailing2" value="dialog">5분 회화</label>
			<label><input type="checkbox" name="mailing3" value="pops">모닝팝스</label>
		</fieldset>
  </form>
  </body>
</html>
```

> color.html

```html
<!doctype html>
<html lang="ko">
  <head>
     <meta charset="utf-8">
     <title> 웹 폼</title>
  </head>
  <body>
	<form>
		<fieldset>
			<legend>과 티셔츠 설문</legend>
			<p>올해 과 티(T)를 만들려고 합니다. 원하는 색상을 추천해 주세요.</p>
			<label>선호색상  <input type="color" value="#00ff00"> </label>
		</fieldset>

  </form>
  </body>
</html>
```

> date.html

```html
<!DOCTYPE html>

<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>date</title>
</head>
<body>
	<form>
		<h3>조회기간 선택</h3>
		<label><input type="date" id="start"></label>
		<label><input type="date" id="end"></label>
	</form>
</body>
</html>
```

> time.html

```html
<!DOCTYPE html>

<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>time 속성</title>
</head>
<body>
	<form>		
		<h3>대관시간을 선택하세요(오늘)</h3>
		<label>시작 시간<input type="time" value="09:00" id="start"></label>,
		<label>종료 시간<input type="time" value="18:00" id="end"></label>

		<h3>대관시간을 선택하세요(다른날짜)</h3>
		<label>시작 시간<input type="datetime-local" value="2016-03-02T09:00" id="start"></label>,
		<label>종료 시간<input type="datetime-local" value="2016-03-02T18:00" id="end"></label>
	</form>
</body>
</html>
```

> submit-reset.html

```html
<!DOCTYPE html>

<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>전송 - 리셋 </title>
	<style>
		body {
			padding:20px;
		}
	</style>
</head>
<body>
	<h3>메일링 리스트 등록</h3>
	<form action="register.php" method="post">
		<label> 메일 주소 <input type="text"></label>
		<input type="submit" value="제출">
		<input type="reset" value="다시입력">
	</form>
</body>
</html>
```

> submit-image.html

```html
<!DOCTYPE html>

<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>전송 - 리셋 </title>
	<style>
		body {
			padding:20px;
		}
	</style>
</head>
<body>
	<h3>메일링 리스트 등록</h3>
	<form action="register.php" method="post">
		<label> 메일 주소 <input type="text"></label>
		<input type="submit" value="제출">
		<input type="reset" value="다시입력">
	</form>
</body>
</html>
```

> button.html

```html
<!DOCTYPE html>

<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>폼 버튼 </title>
</head>
<body>
	<form>		
		<input type="button" value="새 탭 열기" onclick="window.open()">
	</form>
</body>
</html>
```

