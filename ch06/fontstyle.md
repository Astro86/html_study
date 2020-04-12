# 06-1장 글꼴 관련 스타일

> webfont2.html

```html
<!DOCTYPE html>

<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>웹 폰트 사용하기</title>
    <style>
      @import url(http://fonts.googleapis.com/earlyaccess/nanumgothic.css); /* 구글 웹 폰트 */
      .ng-font {
        font-family: "Nanum Gothic", 돋움; /* 웹 폰트 지정 */
      }
      p {
        font-size: 30px; /* 글자 크기 */
      }
    </style>
  </head>
  <body>
    <p>브라우저 기본 글꼴 사용</p>
    <p class="ng-font">나눔고딕 웹 폰트 사용</p>
  </body>
</html>
```

> webfont1.html

```html
<!DOCTYPE html>

<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>웹 폰트 사용하기</title>
    <style>
      @font-face {
        font-family: "trana"; /* 글꼴 */
        src: local("trana"), url("trana.eot"), url("trana.woff") format("woff"),
          url("trana.ttf") format("truetype");
      }
      .w-font {
        font-family: "trana", sans-serif; /* 웹 폰트 지정 */
      }
      p {
        font-size: 30px; /* 글자 크기 */
      }
    </style>
  </head>
  <body>
    <p>Using Default Fonts</p>
    <p class="w-font">Using Trana Fonts</p>
  </body>
</html>
```

> font-size.html

```html
<!DOCTYPE html>

<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>폰트 크기</title>
    <style>
      h1 {
        font-size: 3em; /* 글자 크기 */
      }
      p {
        font-size: 1em; /* 글자 크기 */
      }
    </style>
  </head>
  <body>
    <h1>3em의 크기를 가진 제목</h1>
    <p>1em의 크기를 가진 단락</p>
  </body>
</html>
```

> font-vary.html

```html
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>Font Variant & Weight</title>
    <style>
      .accent {
        font-variant: small-caps; /* 작은 대문자 */
        font-weight: bold; /* 굵게 */
      }
    </style>
  </head>
  <body>
    <h1>세계 3대 미항</h1>
    <p><span class="accent">시드니(Sydney)</span>, 호주</p>
    <p><span class="accent">리우데자네이루(Rio de Janeiro)</span>, 브라질</p>
    <p><span class="accent">나폴리(Naples)</span>, 이탈리아</p>
  </body>
</html>
```

> font-style.html

```html
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>폰트 스타일</title>
    <style>
      p {
        font-style: italic;
      } /* 이탤릭체로 */
      p#txt {
        font-style: normal;
      } /* p 요소 중 id=txt인 부분은 보통체로 */
    </style>
  </head>
  <body>
    <h1>세계 3대 미항</h1>
    <p>시드니(Sydney), 호주</p>
    <p>리우데자네이루(Rio de Janeiro), 브라질</p>
    <p id="txt">나폴리(Naples), 이탈리아</p>
  </body>
</html>
```

> font.html

```html
<!DOCTYPE html>

<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>글꼴 스타일</title>
    <style>
      p.txt {
        font: italic 12px/24px 돋움; /* 글꼴 스타일, 크기, 줄간격, 글꼴 */
      }
    </style>
  </head>
  <body>
    <p class="txt">
      여러 요소가 함께 사용된 웹 문서 안에서 텍스트가 눈에 띄게 하려면 내용에
      맞는 글꼴과 글자 크기, 그리고 글자색을 선택하는 것이 중요합니다.
    </p>
    <p>이럴 때 사용할 수 있는 것이 글꼴 속성입니다.</p>
    <p style="font:caption">[font:caption] 캡션에 어울리는 글꼴 스타일</p>
    <p style="font:icon">[font:icon] 아이콘에 어울리는 글꼴 스타일</p>
    <p style="font:menu">[font:menu] 드롭다운 메뉴에 어울리는 글꼴 스타일</p>
    <p style="font:message-box">
      [font:message-box] 대화 상자에 어울리는 글꼴 스타일
    </p>
    <p style="font:small-caption">
      [font:small-caption] 작은 캡션에 어울리는 글꼴 스타일
    </p>
    <p style="font:status-bar">
      [font:status-bar] 상태표시줄에 어울리는 글꼴 스타일
    </p>
  </body>
</html>
```
