# 19장 정책과 수준
동일한 이유로 동일한 시점에 변경되는 정책은 동일한 수준에 위치하며, 동일한 컴포넌트에 속해야 한다.

서로 다른 이유로, 혹은 다른 시점에 변경되는 정책은 다른 수준에 위치하며, 반드시 다른 컴포넌트로 분리해야 한다. 

(= CCP: 공통 폐쇄 원칙)

아키텍처 개발은 비순환 방향 그래프여야 한다.

그래프에서 노드는 동일한 수준의 정책을 포함하는 컴포넌트를 표현하며,

방향이 있는 간선은 컴포넌트 사이의 의존성을 표현한다. 간선은 다른 수준에 있는 컴포넌트를 연결한다.

- 저수준 컴포넌트가 고수준 컴포넌트에 의존하도록 설계되어야 한다.
- 고수준 컴포넌트 (혹은 정책)은 덜 빈번하게 변경되고, 중요한 이유로 변경되는 경향이 있다.

### 참고
저수준/고수준 컴포넌트 설명 (https://kkeolmusae.tistory.com/90)