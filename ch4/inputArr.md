# 04-4장 여러 데이터 나열해 보여 주기

> select1.html

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
			.reg {
				font-size:14px;
				width:110px;
				color:#390;
				font-weight:bold;		
				float:left;
				text-align:right;
				margin-right:10px;
			 }	 
			 form ul li{
				list-style:none; 
				margin: 15px 0;	
				font-size:14px;	
			 }
	 </style>
  </head>
  <body>
  <h1> 여름방학 특강 신청</h1>
	<form>
    <fieldset>
    <legend>수강 신청인</legend>
    <ul>
    	<li>
	    	<label class="reg" for="id">학번</label>
        	<input type="text" id="id" autofocus> 
        </li>
        <li>       	
	    	<label class="reg" for="name">이름</label>
        	<input type="text" id="name">               
      </li>
    	<li>
            <label class="reg" for="class">학과</label>
            <select id="class">
            	<option value="archi">건축공학과</option>
                <option value="mechanic">기계공학과</option>
                <option value="indust">산업공학과</option>
                <option value="elec">전기전자공학과</option>
            	<option value="computer" selected>컴퓨터공학과</option>
                <option value="chemical">화학공학과</option>
            </select>
      </li>
     </ul>
    </fieldset>
  </form>
  </body>
</html>
```

> select2.html

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
			.reg {
				font-size:14px;
				width:110px;
				color:#390;
				font-weight:bold;		
				float:left;
				text-align:right;
				margin-right:10px;
			 }	 
			 form ul li{
				list-style:none; 
				margin: 15px 0;	
				font-size:14px;	
			 }
	 </style>
  </head>
  <body>
  <h1> 여름방학 특강 신청</h1>
	<form>
    <fieldset>
    <legend>수강 신청인</legend>
    <ul>
    	<li>
	    	<label class="reg" for="id">학번</label>
        	<input type="text" id="id" autofocus> 
        </li>
        <li>       	
	    	<label class="reg" for="name">이름</label>
        	<input type="text" id="name">               
      </li>
    	<li>
            <label class="reg" for="class">학과</label>
			<select size="5" id="class" multiple>
				<option value="archi">건축공학과</option>
				<option value="mechanic">기계공학과</option>
				<option value="indust">산업공학과</option>
				<option value="elec">전기전자공학과</option>
				<option value="computer" selected>컴퓨터공학과</option>
				<option value="chemical">화학공학과</option>
			</select>
      </li>
     </ul>
    </fieldset>
  </form>
  </body>
</html>
```

> select3.html

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
			.reg {
				font-size:14px;
				width:110px;
				color:#390;
				font-weight:bold;		
				float:left;
				text-align:right;
				margin-right:10px;
			 }	 
			 form ul li{
				list-style:none; 
				margin: 15px 0;	
				font-size:14px;	
			 }
	 </style>
  </head>
  <body>
  <h1> 여름방학 특강 신청</h1>
	<form>
    <fieldset>
    <legend>수강 신청인</legend>
    <ul>
    	<li>
	    	<label class="reg" for="id">학번</label>
        <input type="text" id="id" autofocus> 
       </li>
       <li>       	
	    	<label class="reg" for="name">이름</label>
        <input type="text" id="name">               
      </li>
    	<li>
        <label class="reg" for="class">학과</label>
				<select id="class">
					<optgroup label="공과대학">
						<option value="archi">건축공학과</option>
						<option value="mechanic">기계공학과</option>
						<option value="indust">산업공학과</option>
						<option value="elec">전기전자공학과</option>
						<option value="computer">컴퓨터공학과</option>
						<option value="chemical">화학공학과</option>
					</optgroup>
					<optgroup label="인문대학">
						<option value="history">사학과</option>
						<option value="lang">어문학부</option>
						<option value="philo">철학</option>
					</optgroup>
				</select>
      </li>
     </ul>
    </fieldset>
  </form>
  </body>
</html>
```

> datalist.html

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
			.reg {
				font-size:14px;
				width:110px;
				color:#390;
				font-weight:bold;		
				float:left;
				text-align:right;
				margin-right:10px;
			 }	 
			 form ul li{
				list-style:none; 
				margin: 15px 0;	
				font-size:14px;	
			 }
	 </style>
  </head>
  <body>
  <h1> 여름방학 특강 신청</h1>
	<form>
    <fieldset>
    <legend>수강 신청인</legend>
    <ul>
    	<li>
	    	<label class="reg" for="id">학번</label>
        <input type="text" id="id" autofocus> 
       </li>
       <li>       	
	    	<label class="reg" for="name">이름</label>
        <input type="text" id="name">               
      </li>
    	<li>
        <label class="reg" for="class">학과</label>
				<select id="class">
					<optgroup label="공과대학">
						<option value="archi">건축공학과</option>
						<option value="mechanic">기계공학과</option>
						<option value="indust">산업공학과</option>
						<option value="elec">전기전자공학과</option>
						<option value="computer">컴퓨터공학과</option>
						<option value="chemical">화학공학과</option>
					</optgroup>
					<optgroup label="인문대학">
						<option value="history">사학과</option>
						<option value="lang">어문학부</option>
						<option value="philo">철학</option>
					</optgroup>
				</select>
      </li>
     </ul>
    </fieldset>
		<fieldset>
			<legend>수강 과목을 선택하세요</legend>
			<ul>
				<li>
					<span class="reg">관심분야</span>
					<label for="interest"></label>
					<input type="text" id="interest" list="choices">
					<datalist id="choices">
						<option value="grammar" label="문법"></option>
						<option value="voca" label="어휘"></option>
						<option value="speaking" label="회화"></option>
						<option value="listening" label="리스닝"></option>
						<option value="news" label="뉴스청취"></option>
					</datalist>
				</li>
			</ul>
		</fieldset>
  </form>
  </body>
</html>
```

> textarea.html

```html
<!doctype html>
<html lang="ko">
<head>
	<meta charset="utf-8">
	<title> 웹 폼</title>
	<style>
		form fieldset {
			margin: 10px 0;
		}

		form legend {
			font-size: 18px;
			color: #0066FF;
			font-weight: 600;
		}

		form label.reg {
			font-size: 14px;
			width: 120px;
			float: left;
		}

		form label em {
			font-size: 15px;
			color: red;
			font-weight: 800;
		}

		form ul li {
			list-style: none;
			margin: 10px 0;
		}

		form .easys {
			text-align: left;
			font-size: 12px;
			color: blue;
		}

		form fieldset.sendform {
			text-align: center;
		}
	</style>
</head>
<body>
	<form>
		<fieldset class="login">
			<legend>로그인</legend>
			<label for="user_id">아이디 </label>
			<input type="text" id="user_id" size="10" autofocus>
			<label for="user_pw">비밀번호 </label>
			<input type="password" id="user_pw" size="10">
			<input type="submit" value="로그인">
		</fieldset>
		<fieldset class="register">
			<legend>가입하기</legend>
			<ul>
				<li>
					<label class="reg" for="user_name">아이디 <em>*</em></label>
					<input type="text" id="new_id" size="20" autocomplete="on" required>
				</li>
				<li>
					<label class="reg" for="new_pw1">비밀번호 <em>*</em></label>
					<input type="password" id="new_pw1" size="20" required>
				</li>
				<li>
					<label class="reg" for="new_pw2">비밀번호 확인 <em>*</em></label>
					<input type="password" id="new_pw2" size="20" required>
				</li>
				<li>
					<label class="reg" for="user_name">이름 <em>*</em></label>
					<input type="text" id="user_name" size="20" required>
				</li>
				<li>
					<label class="reg" for="user_mail">메일 주소 <em>*</em></label>
					<input type="email" id="user_mail" size="20" required>
				</li>
				<li>
					<label class="reg" for="user_tel">전화번호 </label>
					<input type="tel" id="user_tel" size="20">
				</li>
			</ul>
		</fieldset>
		<fieldset class="easys">
			<legend>이지스퍼블리싱</legend>
			<textarea name="intro" cols="60" rows="5">
열심히 사는 사람들의 손을 잡아주는 곳 - 이지스 퍼블리싱

우리는 책을 내기 전에 다시 한번 물어봅니다
"이 책이 사람들에게 도움이 되는가?"

더 쉽게, 더 빠르게 지식을 전달하고 싶습니다.
이지스퍼블리싱의 책과 앱을 만나보세요.
			</textarea>
		</fieldset>
		<fieldset class="sendform">
			<input type="submit" value="가입하기">
			<input type="reset" value="다시쓰기">
		</fieldset>
	</form>
</body>
</html>
```