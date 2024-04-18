# Today I Learned

## 날짜: 2024-04-18

### 스크럼

- 학습 목표 1: 카카오 클라우드 스쿨 in JEJU 2주차 과제 2-2, 정리 및 리팩토링

### 새로 배운 내용

#### 주제 1: 자바스크립트 DOM 탐색 최소화

자바스크립트에서 DOM 탐색을 최소화하면 성능 향상에 도움을 줄 수 있다.

Before

```js
document.getElementById('button').addEventListener('click', () => {
  document.getElementById('button').innerText = document.getElementById('button').innerText === '버튼' ? '클릭' : '버튼';
});
```

After

```js
const button = document.getElementById('button');

button.addEventListener('click', () => {
  button.innerText = button.innerText === '버튼' ? '클릭' : '버튼';
});
```

### 오늘의 도전 과제와 해결 방법

- 도전 과제 1: 카카오 클라우드 스쿨 in JEJU 2주차 과제 2-2, 정리 및 리팩토링

### 오늘의 회고

- CSS 또는 자바스크립트에서 HTML의 태그를 사용하기 위해 class, id를 사용했지만, 혼용되는 경우가 많았음
- 차후 재사용을 위해 일관성을 유지하고, 유의미한 이름을 사용하도록 노력해야 함

### 참고 자료 및 링크
