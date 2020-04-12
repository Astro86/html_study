# 06-4장 목록 스타일

> bullet.html

```html
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>불릿 바꾸기</title>
    <style>
      .sqbullet {
        list-style-type: square; /* 채운 사각형 */
      }
      .nobullet {
        list-style-type: none; /* 불릿 없애기 */
      }
    </style>
  </head>
  <body>
    <h1>이지스퍼블리싱</h1>
    <!-- 채운 사각형으로 불릿 바꾸기 -->
    <ul class="sqbullet">
      <li>회사소개</li>
      <li>도서</li>
      <li>자료실</li>
      <li>질문답변</li>
      <li>동영상강의</li>
    </ul>

    <!-- 불릿 없애기 -->
    <ul class="nobullet">
      <li>회사소개</li>
      <li>도서</li>
      <li>자료실</li>
      <li>질문답변</li>
      <li>동영상강의</li>
    </ul>
  </body>
</html>
```

> ordered.html

```html
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>불릿 바꾸기</title>
    <style>
      .book1 {
        list-style-type: lower-alpha; /* 소문자 알파벳 */
      }
      .book2 {
        list-style-type: upper-roman; /* 대문자 로마 숫자 */
      }
    </style>
  </head>
  <body>
    <h1>도서 시리즈</h1>
    <ol class="book1">
      <li>Do it! 시리즈</li>
      <li>된다 시리즈</li>
      <li>DCM 프로 사진가</li>
      <li>데이터과학 시리즈</li>
    </ol>

    <ol class="book2">
      <li>Do it! 시리즈</li>
      <li>된다 시리즈</li>
      <li>DCM 프로 사진가</li>
      <li>데이터과학 시리즈</li>
    </ol>
  </body>
</html>
```

> image-bullet.html

```html
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>불릿 바꾸기</title>
    <style>
      ul {
        list-style-image: url("images/dot.png"); /* 불릿으로 사용할 이미지 */
      }
    </style>
  </head>
  <body>
    <h1>이지스퍼블리싱</h1>
    <ul>
      <li>회사소개</li>
      <li>도서</li>
      <li>자료실</li>
      <li>질문답변</li>
      <li>동영상강의</li>
    </ul>
  </body>
</html>
```

> list-position.html

```html
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>불릿 바꾸기</title>
    <style>
      .inside {
        list-style-position: inside;
      }
    </style>
  </head>
  <body>
    <h3>list-style-position을 지정하지 않음</h3>
    <ul>
      <li>회사소개</li>
      <li>도서</li>
      <li>자료실</li>
      <li>질문답변</li>
      <li>동영상강의</li>
    </ul>
    <h3>list-style-position : inside</h3>
    <ul class="inside">
      <li>회사소개</li>
      <li>도서</li>
      <li>자료실</li>
      <li>질문답변</li>
      <li>동영상강의</li>
    </ul>
  </body>
</html>
```
