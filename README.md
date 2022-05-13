# Bitcamp 216 Team Project

## 팀명 : BTS(BiTcampStudent)
## 프로젝트명 : YOMOJOMO
## 개발 기간 : 2022.02.18. ~ 2022.05.02.
  - 2022.02.18. ~ 2022.03.04. : 팀 선정 및 서비스 계획
  - 2022.03.04. ~ 2022.03.18. : 요구사항 정의 및 UI 설계 
  - 2022.03.18. ~ 2022.04.01. : DB 설계
  - 2022.04.01. ~ 2022.05.01. : 구현
  - 2022.05.02 : 최종 발표

## github : [TeamProejct-YOMOJOMO](https://github.com/findkh/TeamProejct-YOMOJOMO)

## 소개  
비슷한 취향을 가진 사람들을 위해 소모임 기능을 제공하고, 위드 코로나  시대에 맞춰 소모임의 활발한 활동을 지원하기 위해 비대면 뿐만 아니라, 대면 모임에도 초점을 맞추어 중간지점 찾기 기능 및 일정 관리 기능을 제공하는 차별화된 모임관리 서비스입니다.

## 제공 서비스   
회원 가입 및 로그인 : 일반, SNS 간편 로그인(카카오, 페이스북, 구글)  
관리자 페이지, 공지사항, 고객센터, 정산관리, 일정관리, 게시글 작성, 마이페이지, 중간지점찾기

## 사용기술   
서버기술 : SpringBoot, MyBatis, mariaDB  
화면기술 : HTML5, JavaScript, CSS, Jquery,  Ajax, Bootstrap, Sweetalert, Handlebars, Swiper, FullCalendar, KakaoAPI, GoogleAPI  
개발도구 : Eclipse, VScode, eXERD, Notion, KakaoOven  
형상관리 : git

## 구현한 부분
### 1. PICK ME 게시판, 모임 초대 메세지, Mypage  
- PICKME 게시판은 회원이 가입할 모임을 찾는 게시판입니다.   
  게시판 CRUD와 MyPage의 모임 초대 메세지 기능, 내가 쓴 글 모아보기를 구현하였습니다.
  - DB 설계
    <img src="https://user-images.githubusercontent.com/89373222/168266643-f11b2748-8c3e-45aa-a5b0-bb28aefbdaae.png"/>
  - UI 및 시연
    - PICKME & Mypage 게시판
      - PICKME 게시판 UI  
      <img src="https://user-images.githubusercontent.com/89373222/168283899-ceb8911d-fea4-4d0e-9041-0fb7e0dca5d5.png"/>   
      - Mypage UI
      <img src="https://user-images.githubusercontent.com/89373222/168288049-e324f1a3-6a21-423d-8ce6-0c85396dc361.png"/>
      - 게시글 페이징 처리
      <img src="https://user-images.githubusercontent.com/89373222/168312052-60411e1e-7b60-4e59-a19c-64ef88208736.gif"/>
      - 게시글 시도, 군구별로 모아보기  
      <img src="https://user-images.githubusercontent.com/89373222/168290802-ef8b1377-92da-4b4e-b0b1-a8483dbfc202.gif"/>
      - 검색 범위는 제목, 게시글의 내용, 작성자 이름이고 시별 군구별로도 모아볼 수 있게 처리하였습니다.  
      <img src="https://user-images.githubusercontent.com/89373222/168292178-63a395ae-78da-408c-8731-59635f432e60.gif"/>
      - 게시글 작성  
      <img src="https://user-images.githubusercontent.com/89373222/168286816-4e17bf3a-091e-4df0-a9c4-3468b992ddbf.gif"/>  
      - 게시글 보기 및 수정  
      <img src="https://user-images.githubusercontent.com/89373222/168287558-9211e81f-13bf-4cf3-bf69-ecc7399ef2fd.gif"/>
      - 모임 초대, 초대 메세지 읽기 전 수정, 삭제  
      <img src="https://user-images.githubusercontent.com/89373222/168293497-f50d564f-7ac1-4af1-9d70-3afc6898a77d.gif"/>  
      - 게시글 작성자의 초대 메시지 수신 후 모임 가입
      <img src="https://user-images.githubusercontent.com/89373222/168295919-be28adb5-66a5-4801-8314-d66edf0f527b.gif"/>  
      - 초대 메세지 수신 후엔 수정 삭제 불가
      <img src="https://user-images.githubusercontent.com/89373222/168296442-3ade978d-4a9e-43c2-9f22-a797b5d9d1fc.gif"/>  
      - Mypage 페이징 처리
      <img src="https://user-images.githubusercontent.com/89373222/168297196-14caa295-4132-447e-96b1-d41214bf2bc3.gif"/>  
      - Mypage에서 게시글 삭제
      <img src="https://user-images.githubusercontent.com/89373222/168298618-de5b12ae-f3c8-4a24-8dd6-af15283aa57a.gif"/>
      <img src="https://user-images.githubusercontent.com/89373222/168300382-5f8ce676-0c2d-49b9-8e2e-4a6bb21c6b17.gif"/>  
### 2. 모임 내 일정 관리
- 모임 내 일정관리를 구현하기 위해 FullCalendar API를 사용하여 CRUD를 구현하였습니다.
  - DB 설계  
    <img src="https://user-images.githubusercontent.com/89373222/168312825-65c863df-7ee0-40d4-9cce-be4c3b457434.png"/>
  - UI 및 시연
    - 일정 관리 UI
      <img src="https://user-images.githubusercontent.com/89373222/168301043-3d85d180-ee11-4b60-bc7b-417f3f15af73.png"/>
      - CRUD  
      <img src="https://user-images.githubusercontent.com/89373222/168301775-590bdb8c-46ce-4c2c-bfbe-1bf029690d20.gif"/>
      - 일반회원 Read만 가능하게 구현
      <img src="https://user-images.githubusercontent.com/89373222/168309680-26678b9b-8739-4f0e-a030-3d93b6b5b091.gif"/>
### 3. 소모임 내 회비 및 정산 관리
- 모임 내에서 발생하는 회비나 기타 비용에 대한 정산 관련 글을 작성하는 게시판으로 CRUD를 구현하였습니다.
  - DB 설계
    <img src="https://user-images.githubusercontent.com/89373222/168313458-41b4b515-4b36-46d5-a6ed-d26977469792.png"/>  
  - UI 및 시연
    <img src="https://user-images.githubusercontent.com/89373222/168304011-586c0225-3e3c-49b0-861a-6883f6a0fe2e.png"/>  
    - 페이징 처리 및 회비 유형별 모아보기
    <img src="https://user-images.githubusercontent.com/89373222/168305220-36490f0d-8a4f-4469-8897-9a07be2bb9d4.gif"/>
    - 게시글 작성  
    <img src="https://user-images.githubusercontent.com/89373222/168306200-08bca125-35fc-4147-b1cc-e66490cc21a0.gif"/>
    - 게시글 보기 및 수정  
    <img src="https://user-images.githubusercontent.com/89373222/168307472-b2cbb4c8-964a-4f80-a654-1ba620f6959c.gif"/>
    - 게시글 삭제  
    <img src="https://user-images.githubusercontent.com/89373222/168308237-f9a2e872-beac-4d61-aca1-8c2b442441c9.gif"/>
    - 일반회원 Read만 가능하게 구현  
    <img src="https://user-images.githubusercontent.com/89373222/168311348-1a045792-efe6-4c36-84a9-9f0479f3b013.gif"/>