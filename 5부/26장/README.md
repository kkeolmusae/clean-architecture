# 26장 메인 컴포넌트
모든 시스템에는 메인(Main) 컴포넌트가 존재한다. 이 컴포넌트는 나머지 컴포넌트를 생성, 조정, 관리하는 역할을 한다.

메인 컴포넌트는 궁극적인 세부사항으로, 가장 낮은 수준의 정책이다. (시스템의 초기 진입점)

의존성 주입 프레임워크를 이용해 의존성을 주입하는 일은 바로 이 "메인 컴포넌트"에서 이루어져야 한다. 메인 컴포넌트에 의존성이 일단 주입되고 나면, 메인 컴포넌트는 의존성 주입 프레임워크를 사용하지 않고도 일반적인 방식으로 의존성을 분배할 수 있어야 한다. 

(tsed 프레임워크에서는 Server.ts가 메인 컴포넌트 역할을 하는 건가..?)

메인 컴포넌트는 고수준의 시스템을 위한 모든 것을 로드한 후, 제어권을 고수준의 시스템에 넘긴다. (메인 컴포넌트는 초기 조건과 설정을 구성하고 외부 자원을 모두 수집한다.)