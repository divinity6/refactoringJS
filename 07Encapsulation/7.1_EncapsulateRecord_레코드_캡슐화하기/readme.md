## 레코드 캡슐화하기
### Encapsulate Record

---

레코드( Record ) : 하나로 취급되는 자료의 집합

- 레코드는 데이터를 직관적으로 묶을 수 있어서 의미있는 단위로 전달할 수 있다


- 그러나, 레코드는 **계산할 값**과 **저장할 값**을 명확히 구분해야함
- 예) 범위
  - { start : 1 , end : 5 }
  - { start : 1 , length : 5 }
  - { end : 5 , length : 5 }
  - 등으로 범위 데이터를 저장가능


- 따라서, 가변데이터는 레코드보단 객체가 좋다

---

객체를 사용하면, 무슨 값을 저장했는지 숨긴채 **각각의 값을 메서드로 전달**할 수 있다

( 저장된 값인지, 계산할 값인지 구분하지 않아도 된다 )

---

- 코드를 작성하면, 중첩리스트 or 해시맵을 JSON , XML 포맷으로 직렬화 시켜야할 경우가 있다
  - 해당 구조를 캡슐화하면 포맷을 바꾸거나, 추적하기 어려운 데이터를 수정하기 수월해진다


- 만약 해당 레코드를 캡슐화 할때, 해당 레코드 필드가 중첩된 구조라면
  - **레코드 캡슐화하기( 7.1 )**
  - **컬렉션 캡슐화하기( 7.2 )**
  - 를 재귀적으로 사용한다

---

#### 재귀적으로 레코드를 클래스화해서 , 캡슐화시키는 방법이 가장확실하다!!