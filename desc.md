비즈니스 카드 CSS 스타일 설명
전체 레이아웃 (body)
```css
body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
```

flex 디스플레이를 사용하여 카드를 화면 중앙에 배치
height: 100vh로 전체 뷰포트 높이를 사용

비즈니스 카드 기본 스타일
```css
.business-card {
    background-color: white;
    width: 320px;
    padding: 40px;
    border: 2px solid #007BFF;
    transition: transform 0.3s, box-shadow 0.3s;
}
```

너비 320px의 흰색 카드
파란색(#007BFF) 테두리
애니메이션 효과를 위한 transition 설정

호버 효과
```css
.business-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 30px rgba(0, 0, 0, 0.3);
}
```

마우스 오버 시 카드가 위로 5px 이동
그림자 효과 추가로 입체감 부여

헤더 영역
```css
.header {
    display: flex;
    border-bottom: 2px solid #007BFF;
    padding-bottom: 10px;
}
```

flex로 요소들을 가로로 배치
하단에 파란색 구분선 추가

제목 스타일
```css
.header h1 {
    font-size: 24px;
    margin: 0;
    padding-right: 10px;
}


.header h2 {
    font-size: 16px;
    color: #007BFF;
    margin: 0;
}
```

h1: 24px 크기의 메인 제목
h2: 16px 크기의 파란색 부제목

연락처 정보
```css
.contact-info {
    margin-top: 15px;
    font-size: 14px;
    color: #555;
}
```

회색(#555)으로 표시되는 14px 크기의 텍스트

소셜 미디어 링크
```css
.socials {
    margin-top: 20px;
    display: flex;
    justify-content: space-between;
}
.socials a {
    color: #007BFF;
    text-decoration: none;
}
```
flex로 링크들을 균등 배치
파란색 링크, 밑줄 제거

클릭 효과
```css
.business-card:active {
    background-color: lightcoral;
}
```

카드 클릭 시 배경색이 연한 산호색으로 변경