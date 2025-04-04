# 태그 총정리

## 태그 분류와 종류



### 1. 기본 구조 태그
웹 문서의 기본적인 구조를 정의하는 태그.
```html
<!DOCTYPE html> <!-- HTML 문서 유형 선언 -->
<html lang="ko">
<head>
    <meta charset="UTF-8"> <!-- 문자 인코딩 설정 -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>문서 제목</title> <!-- 브라우저 탭에 표시될 제목 -->
</head>
<body>
    <!-- 본문 내용 -->
</body>
</html>
```
- `<html>` : HTML 문서의 루트 요소
- `<head>` : 문서의 메타데이터(설정, 제목 등)를 포함
- `<title>` : 문서의 제목을 설정
- `<meta>` : 문서 정보(인코딩, 뷰포트 등)를 지정
- `<body>` : 실제 화면에 보이는 내용을 포함


---


### 2. 텍스트 관련 태그
웹페이지에 텍스트를 표시하는 태그.

```html
<h1>제목 1</h1>
<h2>제목 2</h2>
<p>이것은 문단입니다.</p>
<strong>강조된 텍스트</strong>
<em>기울임 텍스트</em>
```
- `<h1> ~ <h6>` : 제목을 나타내는 태그 (h1이 가장 크고, h6이 가장 작음)

- `<p>` : 단락(문단)을 나타내는 태그

- `<strong>` : 중요(강조) 표시(굵은 글씨)

- `<em>` : 기울임꼴 텍스트(강조)

---

### 3. 레이아웃 관련 태그
구조와 스타일링을 위해 자주 쓰이는 태그.
```html
<div style="background-color: lightgray; padding: 10px;">
    <h2>이것은 div입니다.</h2>
    <p>div는 여러 요소를 그룹화할 때 사용됩니다.</p>
</div>

<p>이 문장에서 <span style="color: red;">이 부분</span>만 강조할 수 있습니다.</p>
```

- `<div>` : 블록 요소로, 여러 요소를 그룹화하는 데 사용됨.
		

- `<span>` : 인라인 요소로, 텍스트의 특정 부분을 감싸 스타일링할 때 사용됨.

---

### 4. 목록 관련 태그
목록을 만들 때 사용하는 태그.

```html
<ul> <!-- 순서 없는 목록 -->
    <li>항목 1</li>
    <li>항목 2</li>
</ul>

<ol> <!-- 순서 있는 목록 -->
    <li>첫 번째</li>
    <li>두 번째</li>
</ol>
```

- `<ul>` : 순서 없는 목록 (●, ○, ■ 등으로 표시)

- `<ol>` : 순서 있는 목록 (1, 2, 3 순서로 표시)

- `<li>` : 목록 항목을 정의

---

### 5. 링크 및 이미지 태그
웹페이지에서 링크와 이미지를 추가하는 태그.

```html
<a href="https://www.google.com">Google로 이동</a>
<img src="image.jpg" alt="설명 텍스트">
```
- `<a href="URL">` : 하이퍼링크를 생성 (다른 페이지나 사이트로 이동)

- `<img src="경로" alt="대체 텍스트">` : 이미지를 삽입하는 태그

---

### 6. 테이블 태그
표를 만들 때 사용하는 태그.

```html
<table border="1">
    <tr>
        <th>이름</th>
        <th>나이</th>
    </tr>
    <tr>
        <td>홍길동</td>
        <td>25</td>
    </tr>
</table>
```
- `<table>` : 표(table)를 정의

- `<tr>` : 표의 행(row)을 정의

- `<th>` : 표의 제목(굵은 글씨)

- `<td>` : 표의 셀(cell)

---

### 7. 폼(form) 태그
사용자로부터 입력을 받을 때 사용하는 태그.
```html
<form action="submit.php" method="POST">
    <label for="name">이름:</label>
    <input type="text" id="name" name="name">
    
    <label for="email">이메일:</label>
    <input type="email" id="email" name="email">
    
    <button type="submit">제출</button>
</form>
```

- `<form>` : 입력 폼을 정의

- `<input type="text">` : 텍스트 입력란

- `<input type="email">` : 이메일 입력란

- `<button>` : 버튼 추가

### 8. fieldset 태그
form 내부에서 또 하나의 소그룹으로 묶을 때 사용하는 태그
속성으로 disabled를 적용하면 input이 노출되기는 하지만 입력을 막을 수 있다.
```html
<form>
  <fieldset disabled>
    <legend>반장</legend>
    <label for="name_1">이름 : </label>
    <input id="name_1" type="text" name="name_1">
    <br><br>
    <label for="age_1">나이 : </label>
    <input type="number" id="age_1" name="age_1">
  </fieldset>
</form>
```

### 9. input 태그

```html
<body bgcolor="5f5f5f">
  <h1>03_textinput</h1>
  <form action="#">
    <label for="txtIp">text</label>
    <br>
    <input 
    id="txtIp"
    type="text"
    placeholder="5자 이하"
    maxlength="5"
    >
    <br><br>
    <label for="pwdIp">password</label>
    <br>
    <input 
    id="pwdIp"
    type="password"
    placeholder="4자 이상"
    minlength="4"
    >
    <br><br>
    <label for="srcIp">search</label>
    <br>
    <input id="srcIp" type="search">
    <br><br>
    <label for="tlIp">tel</label>
    <br>
    <input id="tlIp" type="tlIp">
    <br><br>
    <button type="submit">제출</button>
  </form>
</body>
```

1. input 태그에 type을 설정하지 않으면 default text
2. minlength / maxlength / placeholder
  - 최소 길이 / 최대 길이 / 기본 안내 문구
3. password : 입력 내용 안 보임
4. search : 텍스트 입력 시 X 표시가 보임, 클릭 시 내용 삭제
5. tel : 전화번호 입력 폼, 모바일에서 넘버패드 표시

### 숫자 관련 input 태그

04_numberinput.html

```html
  <form action="#">
    <label for="numIp">number</label>
    <input 
    id="numIp"
    type="number"
    min="0" 
    max="10"
    >
    <!-- 0이상 10이하 -->
    <br><br>
    <label for="rgIp">range</label>
    <input 
    id="rgIp"
    type="range"
    min="0" 
    max="100"
    step="20"
    >
    <br><br>
    <label for="dtIp">date</label>
    <input 
    id="dtIp"
    type="date"
    min="2020-01-01"
    max="2025-12-31"
    >
  </form>
```

number 관련 input 태그
1. number
2. range
3. date -> 예약 관련 서비스 구현에 필요할 수 있다

-> live server 확인 필수

05_checkinput.html

```html
<form action="#">
  <h2>checkbox</h2>
  <input 
  id="cbIp" 
  type="checkbox"
  checked
  >
  <label for="cgIp">유기농</label>
  <br>
  <h2>radio</h2>
  <input 
  id="f_apple"
  type="radio"
  name="fruit"
  value="apple"
  checked
  >
  <label for="f_apple">사과</label>

  <input 
  id="f_grape"
  type="radio"
  name="fruit"
  value="grape"
  >
  <label for="f_orange">포도</label>

  <input 
  id="f_orange"
  type="radio"
  name="fruit"
  value="orange"
  >
  <label for="f_orange">오렌지</label>

  <br><br>

  <input 
  id="f_carrot"
  type="radio"
  name="vege"
  value="carrot"
  checked
  >
  <label for="f_carrot">당근</label>

  <input 
  id="f_cabbage"
  type="radio"
  name="vege"
  value="f_cabbage"
  >
  <label for="f_cabbage">배추</label>

  <input 
  id="f_onion"
  type="radio"
  name="vege"
  value="onion"
  >
  <label for="f_onion">양파</label>
</form>
```

1. checkbox
  - label 요소의 for 속성을 input의 id와 일치시킴. -> 그래서 유기농을 클릭해도 체크 설정 가능.
  - checked 속성 : default로 표시될 체크를 설정할 수 있음

2. radio
  - 라디오 버튼으로 그룹을 설정할 때
  - name 속성을 기준으로 그룹 중 하나의 옵션을 선택할 수 있습니다.

3. value
  - 결과를 서버로 넘기는 실제 데이터.
  - label에서는 유기농, 사과, 포도, 오렌지와 같은 방식으로 알아보기 쉽게 작성했는데, 실제 값은 프로그래밍 언어에 적합하게 영문이나 코드 형식으로 보내야합니다. 그래서 각 imput의 value에 영어로 작성했습니다.

### 기타 input 태그

06_ercinput.html

```html
  <form action="#">
    <label for="fileIp">file</label>
    <br>
    <input 
    id="fileIp"
    type="file"
    accept="image/png, image/jpeg"
    multiple
    >
    <br><br>
    <label for="hdnIp">hidden</label>
    <input
    id="hdnIp" 
    type="hidden"
    >
  </form>
  <br>
  <hr>
  <br>
  <form action="#">
    <label for="emailIp">email</label>
    <input 
    id="emailIp"
    type="email"
    >
    <br><br>
    <button type="submit">제출</button>
  </form>
```

1. file
  - 파일 첨부
  - accept 속성 지정하면 지정된 유형의 파일만 업로드 가능
  - multiple
    - 여러 개의 파일을 한 번에 올릴 수 있도록 지정
    - 설정하지 않을 경우 한 번에 하나의 파일만 가능

2. hidden
  - 사용자로부터 받은 개인 정보나 사용자 본인이 알아서는 안 되는 등급의 정보 때문에 굳이 input 창을 만들어놓고 hidden으로 가려둡니다.
  - 예를 들어 JS 코드로 변환된 값을 input 창에 집어넣고, 이를 제출했을 때 값은 서버로 이동하겠지만 사용자는 이를 인지할 수 없습니다.

3. email

### 10. textarea 태그

긴 분량의 텍스트, 즉 입력이 여러줄을 차지할 때 사용하는 태그

- 내부 속성으로 cols(너비) / rows(줄 수)

- textarea에 기본 입력값을 넣으려면?

    value 속성이 없기 때문에 

```html 
<textarea>이 사이에 값을 넣어야합니다.</textarea>
```

- 브라우저에서 오른쪽 아래에 보면 textarea 크기 조절이 가능한데 이를 막으려면  (style="resize: none;:") css에서 resize: none;으로 설정 해주면 된다

### 11. iframe
페이지 내에 유튜브 영상 링크를 가지고 와서 보여주는 형태

### 12. span / div 태그 : 아무것도 하지 않는 태그 - 가장 중요 
1. span
  - 기능은 딱히 뭐 없음
  - 텍스트의 영역 만큼만 자리 차지
  - 인라인(inline)
2. div
  - 마찬가지로 기능은 딱히 없음
  - 한 줄 전체 차지
  - 블록(block)

- css 설정할 때 class에 따른 style 적용을 잘 하고 싶으면 (display, align-items, justify-content, position 등 너무 많다) 반드시 
```html
<div class="board_warp">
  <div class="btn_warp">
    <button class="close_btn">닫기</button>
  </div>
</div>
```
과 같이 각 요소 요소 마다 상세히 지정해주는 것이 좋다.

또한 초심자라면 css에서 각 요소의 style에 대해 설정할 때 괜히 직접 손으로 치다가 오타 내지 말고(내가 클론 코딩 하면서 그랬음) ctrl + c, ctrl + v를 적극 활용하도록 하자!!!!


