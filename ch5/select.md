# 05-2장 주요 선택자

> tag-selector.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <title>블루베리(Blueberry)</title>
    <style>
      h2 {
        color:blue;
      }
      p{
        font-size:12px;
        margin-left:20px;
      }
    </style>
</head>
<body>
  <h1>블루베리에 관한 연구</h1>
  <h2>블루베리와 항산화 효능</h2> 
  <p>블루베리는 항산화제인 안토시아닌과 폴리페놀을 다량 포함하고 있습니다.</p>
  <p>매사츄세츠 보스톤에 있는 USDA 노화에 관한 인류 영양 연구센터 (the USDA Human Nutrition Research Center on Aging) 의 자료에 의하면
   블루베리는 과일 중에서 가장 항산화 작용이 뛰어난 과일이라고 합니다.  </p>
  <h2>블루베리와 노화</h2> 
  <p> USDA 인류 영양 연구센터(the USDA Human Nutrition Research Center) 실험실에서 신경과학자들은 쥐들에게 블루베리를 먹임으로써 
  노화에 의한 인지능력의 손실을 예방해 준다는 사실을 발견하였습니다. </p>
</body>
</html>
```

> class-selector1.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="utf-8">
  <title>블루베리(Blueberry)</title>    
  <style>
    .bluetext {
      color:blue; /* 글자색 */
    }
		p {
			font-size: 12px; /* 글자 크기 */
			margin-left: 20px; /* 왼쪽 마진 여백 */
		}
  </style>
</head>
<body>
  <h1>블루베리에 관한 연구</h1>
  <h2 class="bluetext">블루베리와 항산화 효능</h2> 
  <p class="bluetext">블루베리는 항산화제인 안토시아닌과 폴리페놀을 다량 포함하고 있습니다.</p>
  <p>매사츄세츠 보스톤에 있는 USDA 노화에 관한 인류 영양 연구센터 (the USDA Human Nutrition Research Center on Aging) 의 자료에 의하면
   블루베리는 과일 중에서 가장 항산화 작용이 뛰어난 과일이라고 합니다.  </p>
  <h2>블루베리와 노화</h2> 
  <p> USDA 인류 영양 연구센터(the USDA Human Nutrition Research Center) 실험실에서 신경과학자들은 쥐들에게 블루베리를 먹임으로써 
  노화에 의한 인지능력의 손실을 예방해 준다는 사실을 발견하였습니다. </p>
</body>
</html>
```

> class-selector2.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="utf-8">
  <title>블루베리(Blueberry)</title>
  <style>
		h2.bluetext {
			color: blue; 		/* 글자색 */;
		}
		p {
			font-size: 12px; /* 글자 크기 */
			margin-left: 20px; /* 왼쪽 마진 여백 */
		}   
  </style>
</head>
<body>
  <h1>블루베리에 관한 연구</h1>
  <h2 class="bluetext">블루베리와 항산화 효능</h2> 
  <p class="bluetext">블루베리는 항산화제인 안토시아닌과 폴리페놀을 다량 포함하고 있습니다.</p>
  <p>매사츄세츠 보스톤에 있는 USDA 노화에 관한 인류 영양 연구센터 (the USDA Human Nutrition Research Center on Aging)의 자료에 의하면
   블루베리는 과일 중에서 가장 항산화 작용이 뛰어난 과일이라고 합니다.  </p>
  <h2>블루베리와 노화</h2> 
  <p>USDA 인류 영양 연구센터(the USDA Human Nutrition Research Center)신경과학자들은 쥐들에게 블루베리를 먹임으로써 
  노화에 의한 인지능력의 손실을 예방해 준다는 사실을 발견하였습니다. </p>
</body>
</html>
```

> class-selector3.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="utf-8">
  <title>블루베리(Blueberry)</title>
  <style>
    h2.bluetext {
      color:blue; /* 글자색 */
    }
		.redtext {
			color: red; /* 글자색 */
		}
    p{
      font-size:12px; /* 글자 크기 */
      margin-left:20px; /* 왼쪽 마진 여백 */
    }
  </style>
</head>
<body>
  <h1>블루베리에 관한 연구</h1>
  <h2 class="bluetext">블루베리와 항산화 효능</h2> 
  <p class="bluetext">블루베리는 항산화제인 안토시아닌과 폴리페놀을 다량 포함하고 있습니다.</p>
  <p>매사츄세츠 보스톤에 있는 <span class="redtext">USDA 노화에 관한 인류 영양 연구센터 (the USDA Human Nutrition Research Center on Aging)</span> 의 자료에 의하면
   블루베리는 과일 중에서 가장 항산화 작용이 뛰어난 과일이라고 합니다.  </p>
  <h2>블루베리와 노화</h2> 
  <p><span class="redtext"> USDA 인류 영양 연구센터(the USDA Human Nutrition Research Center) </span> 신경과학자들은 쥐들에게 블루베리를 먹임으로써 
  노화에 의한 인지능력의 손실을 예방해 준다는 사실을 발견하였습니다. </p>
</body>
</html>
```

> id-selector.html

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="utf-8">
    <title>id 선택자</title>
	<style>
		#container {
			background: #ff6a00; /* 배경색 */
			width:400px; /* 너비 */
			height:200px; /* 높이 */
			margin:0 auto; /* 가로로 중앙에 배치 */
		}
	</style>
</head>
<body>
	<div id="container"></div>	
</body>
</html>
```