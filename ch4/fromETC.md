# 04-5 기타 다양한 폼 요소들

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

> button-css.html

```html
<!doctype html>
<html>
<head>
	<meta charset="utf-8">
	<title>웹 폼</title>
	<style>
		.subm{  /* 버튼 스타일 */
			display:block;  /* 블록 레벨 요소 */
			background-color:#fff;  /* 배경색 */
			border:1px solid #dedede;  /* 테두리 */
			cursor:pointer;  /* 마우스 포인터 */
			padding:5px 10px 6px 7px;	/* 패딩 */
		}
		.subm img{  /* 버튼 내 왼쪽 이미지 */
			border:0;  /* 테두리 없음*/
			padding:0;  /* 패딩 없음 */
			width:16px;  /* 가로 크기 */
			height:16px;  /* 세로 크기 */	
		}
		.subm:hover{  /* 버튼 위로 마우스 포인터 올렸을 때 스타일 */
			background-color:#e6efc2;  /* 배경색 */
			border:1px solid #c6d880;  /* 테두리 */
			color:#529215; /* 글자색 */
		}
	</style>
</head>

<body>
	<form>
		<button type="submit" class="subm">
			<img src="images/tick.png" alt=""> 전송하기
		</button>
	</form>
</body>
</html>
```

> output.html

```html
<!doctype html>
<html>
<head>
	<meta charset="utf-8">
	<title>웹 폼</title>
</head>

<body>
	<form oninput="result.value=parseInt(num1.value)+parseInt(num2.value)">
		<input type="number" name="num1" value="0">
		+<input type="number" name="num2" value="0">
		=<output name="result" for="num"></output>
	</form>
</body>
</html>
```

> progress.html

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
 	 ul li{
		list-style:none; 
		margin: 15px 0;	
		font-size:14px;	
	 }		 
	 </style>
  </head>
  <body>
  	<ul>
      <li>
      	<label>10초 남음</label>
		<!-- 전체 60초 중 50초 진행 -->
		<progress value="50" max="60"> </progress>
      </li>
      <li>
      	<label>진행률 30%</label>
		<!-- 전체 100 중 30만큼 진행 -->
    	<progress value="30" max="100"></progress> 
      </li>
    </ul>
  </body>
</html>
```

> progress-js.html

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
 	 ul li{
		list-style:none; 
		margin: 15px 0;	
		font-size:14px;	
	 }
	 </style>
  </head>
  <body>
    <script>
	function dwn(){
		var bar=document.getElementById("bar"),
		progress=document.getElementById("progress"),
		loaded=0;
		var load=function(){
			loaded +=5;
			bar.value=loaded;		

			if(loaded ==100){
				clearInterval(dummyLoad);	
			}		
		};
	
		var dummyLoad = setInterval(function() {
			load()	
		}, 500);
	}
	</script>    
	<input type="button" value="다운로드 시작" onClick="dwn()">    
    <progress id="bar" value="0" max="100">
    	<span id="progress"> </span></progress>    
  </body>
</html>
```

> meter.html

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
 	 ul li{
		list-style:none; 
		margin: 15px 0;	
		font-size:14px;	
	 }
     </style>
  </head>
  <body>
  	<ul>
      <li>
      	<label>점유율 0.8 </label>
	  	<!-- 전체 크기 1을 기준으로 0.8만큼 차지합니다 -->
		<meter value="0.8"></meter>
      </li>
      <li>
      	<label>사용량 64%</label>
		<!-- 전체 100 중에서 64만큼 차지합니다  -->
		<meter min="0" max="100" value="64"></meter>
      </li>
      <li>
      	<label>트래픽 초과</label>
		<!-- 전체 크기는 1024~10240까지인데 높다고 설정한 8192보다 현재 값 9216이 더 큽니다 -->
      	<meter min="1024" max="10240" low="2048" high="8192" value="9216"></meter>        
      </li>
      <li>
      	<label>적절한 트래픽</label>
		<!-- 전체 1 중에서 현재 0.5를 차지하고 있으며 적정도를 0.8로 설정했습니다 -->
        <meter value="0.5" optimum="0.8"></meter>
      </li>
    </ul>
  </body>
</html>
```