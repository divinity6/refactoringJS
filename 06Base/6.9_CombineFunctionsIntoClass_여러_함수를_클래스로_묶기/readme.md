## 여러 함수를 클래스로 묶기
### Combine Functions into Class

---

사람들이 잘 모르는 클래스의 장점 : **데이터와 함수를 하나의 환경으로 묶을 수 있다는 것**

- 신호 :
  - 함수에 전달되는 파라미터들이 공통적일 경우,
  - 데이터를 처리하는 로직들이 함수로 분산되어 있을 경우,


- 클래스로 묶으면 해당 데이터에 관한 동작들을 일관되게 관리할 수 있다
  -( 클래스 대신 **중첩함수** 를 이용해도 된다 : 클래스를 지원하지 않을 경우 )


- 그러나 이 작업을 하려면 먼저,
  - **레코드 캡슐화하기( 7.1 )**


- 공통 레코드를 사용하는 함수를,
  - **함수 옮기기( 8.1 )**


- 데이터를 조작하는 로직들일 경우,
  - **함수 추출하기( 6.1 )**

----

**데이터를 처리하는 코드( 보통 함수 )** 와 **데이터 코드**는 가까이 두는 것이 좋다

뿔변 데이터가 좋지만, 가변 데이터를 사용해야할 경우가 많다면 클래스로 묶어두는 것이 큰 도움이된다!!