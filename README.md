# 여행복행
#### 우리나라 대표 휴양지인 제주도에 대한 다양한 정보를 제공하고 많은 사람들의 방문을 유도할 수 있는 프로젝트

## [Project-study][project-study-link]

[project-study-link]: https://github.com/JaeHyukSim/project-study/blob/master/README.md "Go project-study!"

-----------

### 나의 담당 부분과 기능
+ ERD 설계
    - [ERD 보러가기][erd-link]
    
    [erd-link]: /ERD.md "Go ERD!"
+ 호텔 리스트
    - [perfect-sliding 보러가기!][perfect-sliding-link]
    
    [perfect-sliding-link]: https://github.com/JaeHyukSim/perfect-sliding "Go perpect-sliding!"
    
    - [검색 기능 보러가기][search-link]
    
    [search-link]: /Search.md "Go Search function!"
    - [더보기 기능 보러가기][more-link]
    
    [more-link]: /more.md "Go more function!"
+ 호텔 디테일
    - modal 기능
        + 모달 창 띄우기 / 밖 클릭 시 꺼짐.
	    + 모달 창 드래그하기 - 모달의 위치를 바꿀 수 있다
	    + 모달 스크롤 - 모달을 띄우면, 원본 스크롤이 없어지고, 모달의 스크롤만 제어 가능하다
    - tab UI 기능
        + 텝 유아이는 클릭을 통해, 여러 메뉴를 선택할 수 있다
	+ 메뉴는 상세정보, 이용정보, 카카오 api를 사용한 지도(반경 1km내의 시설 안내), 댓글 작성이 있다.

### 축적한 지식
+ Back End : Spring의 Dispatcher Servlet 동작 방식에 대한 이해
    - 프론트 서블릿과 연계하는 핸들러 매핑, 뷰 리졸버를 스트링 파싱을 통해 패키지에서 찾고, url을 매핑시킨다.
    - db 동작을 위해 mybatis를 활용하여 SQL문장을 따로 분리시켜서 가독성을 높인다.
    - MVC 패턴에 대해 명확히 이해한다
+ Front End : javascript에 대한 이해
    - templating 기법으로 html 문장을 미리 만들고, 데이터를 대입하여 재활용할 수 있는 코드를 제작하였다
    - evemt delegating, bubbling 등을 활용하여, 리스트에서 특정 부분을 클릭했을 때 적절히 동작하도록 하였다.
    - CSS를 활용하여, slider와 같은 애니메이션을 구현하였다 : 다음에 더 공부해야 할 목록 - GUI 가속
+ 정규화에 대한 이해
    - 프로젝트를 진행하면서, 데이터 중복을 방지하기 위해 정규화 시키려고 노력하였다
    - 삭제이상을 방지하기 위해 원본 데이터를 유지하는 릴레이션을 제작하고, 이 릴레이션의 관계도 테이블로 만들었다
### 개발 기간
+ #### 2020-03-16 ~ 2020-04-29
### 팀원 
+ 심재혁 김유진 김학민 신승호 조성빈

-----------

### 사용한 기술및 도구
- Java JSP Vanilla Javascript HTML CSS
- STS(Spring-Tool-Suite)

---------

### 실행 방법
- [happy-travel url][happy-travel-link]

[happy-travel-link]: URL "Go happy-travel!"

-----------

### 시연 영상 - 1차
[시연 영상 보러가기][desc-link]

[desc-link]: https://www.youtube.com/watch?v=Ts9go0W2r6c&feature=youtu.be "Go desc link!"
