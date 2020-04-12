# 04-3장 <input> 태그의 다양한 속성

> attribute.html

```html
<!doctype html>
<html lang="ko">
  <head>
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

				#member, #stuffs {
					width:50px; 
				}
	 		</style>
  </head>
  <body>
    <h1> 여름방학 특강 신청</h1>
  	<form>
  		<fieldset id="subject">
  			<legend>수강과목</legend>
  			<ul>
  				<li>
  					<label class="reg" for="subj">영어회화(초급)</label>
  					<input type="text" id="subj" value="오전 9:00~11:00" readonly>
  				</li>
  			</ul>
  		</fieldset>
  		<fieldset id="register">
  			<legend> 신청자</legend>
  			<ul>
  				<li>
  					<label class="reg" for="uname">이름</label>
  					<input type="text" id="uname" autofocus required>
  				</li>
  				<li>
  					<label class="reg" for="uid">학번</label>
  					<input type="text" id="uid" placeholder="하이픈없이 입력" maxlength="8" required>
  				</li>
  				<li>
  					<label class="reg" for="uclass">학과</label>
  					<select id="uclass">
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
  		<fieldset>
  			<legend>교재 주문</legend>
  			<ul>
  				<li>
  					<label class="reg" for="book">교재</label>
  					<input type="number" id="book" value="1" min="1" max="3">
  				</li>
  				<li>
  					<label class="reg" for="wsheet">워크시트</label>
  					<input type="number" id="wsheet" value="1" min="1" max="3">
  				</li>
  				<li>
  					<label class="reg" for="group">단체주문</label>
  					<input type="number" id="group" value="10" min="10" max="100" step="10">
  				</li>
  			</ul>
  		</fieldset>
  		<fieldset>
  			<button type="submit" value="submit">신청하기</button>
  			<button type="reset" value="reset">다시쓰기</button>
  		</fieldset>


  	</form>
  </body>
</html>
```

> join.html

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
	 </style>
  </head>
  <body>
		<h1>회원 가입을 환영합니다</h1>
		<form>
			<ul>
    		<li><label>아이디: <input type="text" id="user_id" size="10" minlength="4" maxlength="15"></label><small style="color:red;"> 4~15자리 이내의 영문과 숫자</small></li>
				<li><label>이메일: <input type="email" id="user_email"></label></li>
				<li><label>비밀번호: <input type="password" id="user_pwd"></label></li>
				<li><label>비밀번호 확인: <input type="password" id="check_pwd"></label></li>
				<li><input type="submit" value="회원가입"></li>
			</ul>
  </form>
  </body>
</html>
```

> order.html

```html
<!doctype html>
<html>
<head>
	<meta charset="utf-8">
	<title> 주문서 작성하기</title>
</head>
<body>
	<div class="container">
		<h1>상품 주문서</h1>
		
	</div>
</body>
</html>
```


> order-result.html

```html
<!doctype html>
<html>
<head>
	<meta charset="utf-8">
	<title> 주문서 작성하기</title>
	<style>
		.container {
			width:600px;
			margin:0 auto;
		}
		ul { /* 순서없는 목록에 적용할 스타일 */
			list-style-type: none; /* 불릿 없앰 */
		}

		label.title { /* class=title인 label에 적용할 스타일 */
			font-weight: bold; /* 굵은 글자 */
			width: 80px; /* 너비 80px */
			float: left; /* 왼쪽부터 배치 */
		}

		div.centered { /* class=centered인 div에 적용할 스타일 */
			text-align: center; /* 가운데 정렬 */
		}

		fieldset { /* 필드셋에 적용할 스타일*/
			margin: 15px 10px; /* 상하 마진 15xp, 좌우 마진 10px */
		}

			fieldset legend { /* 필드셋의 제목 */
				font-weight: bold; /* 굵은 글자 */
				font-size: 18px; /* 글자 크기 18px */
				color: purple; /* 글자색 자주 */
			}

		ul li { /* 목록의 각 항목 */
			margin-bottom: 10px; /* 아래 마진 10px */
		}
	</style>	
</head>
<body>
	<div class="container">
		<h1>상품 주문서</h1>
		<form>
			<fieldset>
				<legend>개인 정보</legend>
				<ul>
					<li>
						<label for="uname" class="title">이름</label>
						<input type="text" id="uname" placeholder="여백없이 입력" required>
					</li>
					<li>
						<label for="tel1" class="title">연락처</label>
						<input type="tel" id="tel1" placeholder="연락가능한 번호">
					</li>
				</ul>
			</fieldset>
			<fieldset>
				<legend>배송지 정보</legend>
				<ul>
					<li>
						<label for="addr" class="title">주소</label>
						<input type="text" size="40" id="addr" required>
					</li>
					<li>
						<label for="tel2" class="title">전화번호</label>
						<input type="tel" id="tel2" required>
					</li>
					<li>
						<label for="comment" class="title">메 모</label>
						<textarea cols="40" rows="3" id="comment"></textarea>
					</li>
				</ul>
			</fieldset>
			<fieldset>
				<legend>주문 정보</legend>
				<ul>
					<li>
						<label><input type="checkbox">과테말라 안티구아 (100g) </label>
						<label><input type="number" value="0" min="0" max="5">개 </label>
					</li>
					<li>
						<label><input type="checkbox">인도네시아 만델링 (100g) </label>
						<label><input type="number" value="0" min="0" max="5">개 </label>
					</li>
					<li>
						<label><input type="checkbox">탐라는도다(블렌딩) (100g) </label>
						<label><input type="number" value="0" min="0" max="5">개 </label>
					</li>
				</ul>
			</fieldset>
			<div class="centered">
				<input type="submit" value="주문하기">
				<input type="reset" value="다시 작성">
			</div>
		</form>
	</div>
</body>
</html>
```

