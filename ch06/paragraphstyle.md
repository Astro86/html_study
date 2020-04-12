# 06-3장 문단 스타일

> text-align.html

```html
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>뉴욕타임즈 10대 식품</title>
    <style>
      p {
        border: 1px solid #ccc; /* 테두리 - 1픽셀짜리 회색 실선 */
        padding: 10px; /* 테두리와 내용 사이의 패딩 여백 */
        margin: 10px; /* 단락 주변의 마진 여백 */
      }
      .align-left {
        text-align: left;
      } /* 왼쪽 정렬 */
      .align-right {
        text-align: right;
      } /* 오른쪽 정렬 */
      .align-center {
        text-align: center;
      } /* 가운데 정렬 */
      .align-justify {
        text-align: justify;
      } /* 양쪽 정렬 */
    </style>
  </head>
  <body>
    <h1>텍스트 정렬</h1>

    <!-- 왼쪽 정렬 -->
    <p class="align-left">
      Integer elementum massa at nulla placerat varius. Suspendisse in libero
      risus, in interdum massa. Vestibulum ac leo vitae metus faucibus gravida
      ac in neque. Nullam est eros, suscipit sed dictum quis, accumsan a ligula.
    </p>

    <!-- 오른쪽 정렬 -->
    <p class="align-right">
      Integer elementum massa at nulla placerat varius. Suspendisse in libero
      risus, in interdum massa. Vestibulum ac leo vitae metus faucibus gravida
      ac in neque. Nullam est eros, suscipit sed dictum quis, accumsan a ligula.
    </p>

    <!-- 가운데 정렬 -->
    <p class="align-center">
      Integer elementum massa at nulla placerat varius. Suspendisse in libero
      risus, in interdum massa. Vestibulum ac leo vitae metus faucibus gravida
      ac in neque. Nullam est eros, suscipit sed dictum quis, accumsan a ligula.
    </p>

    <!-- 양쪽 정렬 -->
    <p class="align-justify">
      Integer elementum massa at nulla placerat varius. Suspendisse in libero
      risus, in interdum massa. Vestibulum ac leo vitae metus faucibus gravida
      ac in neque. Nullam est eros, suscipit sed dictum quis, accumsan a ligula.
    </p>
  </body>
</html>
```

> text-indent.html

```html
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>뉴욕타임즈 10대 식품</title>
    <style>
      p {
        border: 1px solid #000; /* 테두리 - 1픽셀짜리 회색 실선 */
        padding: 10px; /* 패딩 여백 */
        margin: 10px; /* 마진 여백 */
      }
      .indent1 {
        text-indent: 15px;
      } /* 15px만큼 들여쓰기 */
      .indent2 {
        text-indent: 5%;
      } /* 5%만큼 들여쓰기 */
    </style>
  </head>
  <body>
    <h1>블루베리(Blueberry)</h1>
    <p>
      블루베리는 비타민A, C, E가 풍부하고 안토니시아민, 페놀 등이 활성 산소를
      없애 노화를 억제하고 블루베리의 안토니시아민은 눈의 피로와 시력 저하를
      회복시키는 효능을 가지기도 한다.
    </p>
    <p class="indent1">
      블루베리는 비타민A, C, E가 풍부하고 안토니시아민, 페놀 등이 활성 산소를
      없애 노화를 억제하고 블루베리의 안토니시아민은 눈의 피로와 시력 저하를
      회복시키는 효능을 가지기도 한다.
    </p>
    <p class="indent2">
      블루베리는 비타민A, C, E가 풍부하고 안토니시아민, 페놀 등이 활성 산소를
      없애 노화를 억제하고 블루베리의 안토니시아민은 눈의 피로와 시력 저하를
      회복시키는 효능을 가지기도 한다.
    </p>
  </body>
</html>
```

> line-height.html

```html
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>줄 간격</title>
    <style>
      p {
        font-size: 15px;
        border: 1px solid gray;
        padding: 10px;
      }
      .big-line {
        line-height: 2; /* 글자 크기 2배만큼의 줄간격 */
      }
      .small-line {
        line-height: 0.7; /* 글자 크기 0.7배만큼의 줄간격 */
      }
    </style>
  </head>
  <body>
    <h2>블루베리(Blueberry)</h2>
    <p>
      블루베리의 대표적인 기능은 항산화로 비타민A, C, E가 풍부하고 안토니시아민,
      페놀 등이 활성 산소를 없애 노화를 억제한다. 이밖에 블루베리의
      안토니시아민은 눈의 피로와 시력 저하를 회복시키는 효능을 가지고 있다.
    </p>
    <p class="small-line">
      블루베리의 대표적인 기능은 항산화로 비타민A, C, E가 풍부하고 안토니시아민,
      페놀 등이 활성 산소를 없애 노화를 억제한다. 이밖에 블루베리의
      안토니시아민은 눈의 피로와 시력 저하를 회복시키는 효능을 가지고 있다.
    </p>
    <p class="big-line">
      블루베리의 대표적인 기능은 항산화로 비타민A, C, E가 풍부하고 안토니시아민,
      페놀 등이 활성 산소를 없애 노화를 억제한다. 이밖에 블루베리의
      안토니시아민은 눈의 피로와 시력 저하를 회복시키는 효능을 가지고 있다.
    </p>
  </body>
</html>
```

> text-overflow.html

```html
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>슈퍼푸드</title>
    <style>
      .content {
        border: 1px solid #ccc; /* 테두리 */
        width: 300px; /* 단락의 너비 */
        white-space: nowrap; /* 줄바꿈 없음 */
        overflow: hidden; /* 넘치는 부분 감춤 */
        text-overflow: ellipsis; /* 말줄임표 */
      }
      .content:hover {
        overflow: visible; /* 넘치는 부분 보여줌*/
      }
    </style>
  </head>
  <body>
    <h2>귀리(Oat)</h2>
    <p class="content">
      귀리는 베타글루칸(항암 및 면역증강작용을 가지고 있는 불소화성 다당류)
      성분을 포함하고 있다.
    </p>
  </body>
</html>
```

> market.html

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>market</title>
    <style>
      #container {
        /* 전체 콘텐츠를 감싸는 div */
        width: 650px; /* 너비 */
        margin: 0 auto; /* 가로로 중앙에 배치 */
        padding: 5px; /* 테두리와 내용 사이의 패딩 여백 */
      }
      #check {
        /* 텍스트 부분을 감싸는 div */
        width: 640px; /* 너비 - 그림 너비 값에 맞춤 */
        border: 1px solid #ccc; /* 테두리 */
      }
    </style>
  </head>

  <body>
    <div id="container">
      <img
        src="images/top.jpg"
        alt="가정용 꿀사과 - 흠집이 있고 약간은 못생겼지만 맛과 영양은 그대로입니다. 질좋은 사과를 저렴하게 즐겨보세요"
      />
      <div id="check">
        <h1>확인하세요</h1>
        <h2>주문 및 배송</h2>
        <p>
          오후 2시 이전 주문건은 당일 발송합니다<br />
          2시 이후 주문건은 다음날 발송합니다(주말 제외)
        </p>
        <hr />
        <h2>교환 및 환불</h2>
        <p>
          불만족시 100% 환불해 드립니다<br />
          고객센터로 전화주세요
        </p>
        <hr />
        <h2>고객센터</h2>
        <p>
          0000-0000<br />
          상담시간 : 오전 9시 ~ 오후 6시 (토/일, 공휴일 휴무)
        </p>
      </div>
    </div>
  </body>
</html>
```

> market-result.html

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>market</title>
    <style>
      #container {
        /* 전체 콘텐츠를 감싸는 div */
        width: 650px; /* 너비 */
        margin: 0 auto; /* 가로로 중앙에 배치 */
        padding: 5px; /* 테두리와 내용 사이의 패딩 여백 */
      }
      #check {
        /* 텍스트 부분을 감싸는 div */
        width: 640px; /* 너비 - 그림 너비 값에 맞춤 */
        border: 1px solid #ccc; /* 테두리 */
      }
      h1 {
        color: white; /* 글자색 */
        font-size: 1em; /* 글자 크기 */
        background: #222; /* 배경색 */
        margin: 0; /* 제목과 다른 요소 간의 마진 여백 */
        padding: 10px; /* 테두리와 제목 텍스트 사이의 패딩 여백 */
      }
      h2 {
        color: #ff0000; /* 글자색 */
        font-size: 1.2em; /* 글자 크기 */
        text-align: center; /* 가운데 정렬 */
      }
      p {
        font-size: 1.5em; /* 글자 크기 */
        line-height: 2em; /* 줄간격 */
        font-weight: bold; /* 굵게 */
        text-align: center; /* 가운데 정렬 */
      }
      .accent {
        color: blue; /* 글자색 */
      }
      .smalltext {
        font-size: 0.7em; /* 글자 크기 */
      }
    </style>
  </head>

  <body>
    <div id="container">
      <img
        src="images/top.jpg"
        alt="가정용 꿀사과 - 흠집이 있고 약간은 못생겼지만 맛과 영양은 그대로입니다. 질좋은 사과를 저렴하게 즐겨보세요"
      />
      <div id="check">
        <h1>확인하세요</h1>
        <h2>주문 및 배송</h2>
        <p>
          <span class="accent">오후 2시 이전</span> 주문건은 당일 발송합니다<br />
          2시 이후 주문건은 다음날 발송합니다(주말 제외)
        </p>
        <hr />
        <h2>교환 및 환불</h2>
        <p>
          불만족시 <span class="accent">100% 환불</span>해 드립니다<br />
          고객센터로 전화주세요
        </p>
        <hr />
        <h2>고객센터</h2>
        <p>
          0000-0000<br />
          <span class="smalltext"
            >상담시간 : 오전 9시 ~ 오후 6시 (토/일, 공휴일 휴무)</span
          >
        </p>
      </div>
    </div>
  </body>
</html>
```
