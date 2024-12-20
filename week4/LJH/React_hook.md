# React Hook

React 16.8 버전에서 도입된 기능으로, 클래스형 컴포넌트에서만 가능했던 상태 관리와 라이프 사이클 기능 등을 `함수형 컴포넌트`에서도 사용할 수 있게 해주는 기능입니다.

## 주요 Hook

* `useState` : 컴포넌트의 상태를 관리
* `useEffect` : 컴포넌트가 렌더링될 때마다 특정 작업(Side Effect)을 실행
* `useContext` : 전역에서 사용할 수 있는 context를 가져옴
* `useReducer` : 여러 개의 상태 관리를 할 때 사용되는 Hook. 컴포넌트의 상태 업데이트 로직을 따로 분리할 수 있음
* `useRef` : ref 객체를 생성하고, 특정 DOM에 접근하여 DOM 조작을 진행

<br/>

---

### 예상 꼬리 질문

* `useEffect`에서 두 번째 파라미터의 역할이 무엇인가요?

  ```javascript
  useEffect(() => {
    console.log(name);
  }, [name])
  ```

  두 번째 파라미터로 전달되는 배열 내에 존재하는 값이 변경될 때에만 useEffect를 호출하여 작업을 실행합니다. 두 번째 파라미터가 빈 배열일 경우에는 컴포넌트가 처음 마운트 될 때만 실행되고 이 후에는 실행되지 않습니다. 두 번째 파라미터를 아예 넣지 않은 경우에는 컴포넌트가 렌더링될 때마다 실행되기 때문에 상태나 props가 변경될 때마다 호출이 되어 불필요한 렌더링이 발생할 수 있습니다.

<br/>

---

### 참고 자료

[리액트의 Hooks 완벽 정복하기](https://velog.io/@velopert/react-hooks)
