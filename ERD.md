# 정규화 - Project 적용
### 데이터베이스 정규화란?
  - 데이터베이스의 설계를 재구성하는 테크닉이다. 정규화를 통해 불필요한 데이터중복(redundancy)를 없애는 효과가 가장 크다.(삽입, 갱신, 삭제 이상현상)
  - 데이터 저장을 논리적으로 함으로써 발생될 수 있는 삭제 이상도 제거한다
---------------
### 제 1 정규화 적용
  1. 제 1 정규화란?
      - 각 tuple마다 column의 값이 유일해야 해야 한다 - 이를 컬럼이 원자값(Atomic Value)를 갖는다 한다
      - 프로젝트를 통한 예시
          1. products 릴레이션과 products-picture릴레이션 생성
              - 상품들에 사진이 여러개 있을 수 있는데, 그 개수가 일정하지 않아서
               각 사진에 대한 컬럼을 만들 수 없다(RDBMS). 또한, 이를 products 릴레이션의 한 컬럼에
               구분자를 통한 배열(값1,값2,값3...)로 저장할 수 있는데, 이렇게 구현할 경우 데이터의
               추가, 삭제, 갱신에 대한 복잡한 문제가 발생할 수 있다(해당 컬럼의 문자열을 조작해야 하는 이슈)
              - 이에 대한 해결책으로 pictures 릴레이션을 생성한다. 그리고, pictures의 url과, products에서 참조한 product's id를 하나의 primary key로 결정하여 유일하게 만들었다.
               
                  <img src="/img/erd-1normalization-products-and-pictures.PNG" width="90%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>
                  <img src="/img/erd-1normalization-products-and-rooms.PNG" width="50%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>
      
### 제 2 정규화 적용
  2. 제 2 정규화란?
      - 완전 함수적 종속 만들기 - 기본키의 구성중 일부에만 종속적인 컬럼이 있으면 안된다.
