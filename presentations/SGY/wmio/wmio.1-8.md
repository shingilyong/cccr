
# Webmethods.io
webmethods.io youtube영상을 보고 나서 내용을 정리해보자

---
## Contents
[1회](#1회)
[2회](#2회)
[3회](#3회)
[4회](#4회)<br/>
[5회](#5회)
[6회](#6회)
[7회](#7회)
[8회](#8회)<br/>
## 1회
WebMethods.io 계정을 생성하고 로그인하는 방법을 알려줌 <br/>
       1. 홈페이지 접속<br/><br/>
       <img src = "https://user-images.githubusercontent.com/69182192/91125229-31bec180-e6dc-11ea-8b6b-12d354f5b8fa.png" width="250px"> <br/><br/>
       2. 홈페이지 우측 상단에 Login 클릭 <br/><br/>
       <img src = "https://user-images.githubusercontent.com/69182192/91125232-34b9b200-e6dc-11ea-8ed4-e3b817b2b504.png" width="250px"> <br/><br/>
       3. 회원가입 화면 접속<br/><br/>
       <img src = "https://user-images.githubusercontent.com/69182192/91125404-a265de00-e6dc-11ea-8431-e6b1b98395ab.png" width="250px"> <br/> <br/>
       4. 회원가입 후 로그인<br/><br/>
       <img src = "https://user-images.githubusercontent.com/69182192/91125408-a42fa180-e6dc-11ea-8671-c4f5e2837749.png" width="250px"> <br/> <br/>
       5. 로그인 후 접속화면<br/><br/>
       <img src = "https://user-images.githubusercontent.com/69182192/91125412-a4c83800-e6dc-11ea-939a-95bf5bf8b4eb.png" width="250px"> <br/> <br/>
## 2회
새 프로젝트와 워크플로우를 만들고 트리거와 커넥터를 사용해서 트위터와 슬랙을 연결함<br/>
1.프로젝트 화면으로 접속<br/><br/>

2.새 프로젝트 생성<br/><br/>

    3. 워크플로우 생성<br/><br/>

    4. 워크플로우 접속<br/><br/>

    5. 트리거 선택<br/><br/>

       6. 트리거에 대한 인증<br/><br/>

       7. 트리거 설정화면<br/><br/>

       8. 액션, 트리거 연결<br/><br/>

       9. 연결 확인<br/><br/>

 

## 3회
프로젝트 섹션들에 대해서 설명함<br/>
workflow : 새 워크 플로를 만들거나 레시피 에서 워크 플로를 가져올 수 있습니다 .<br/>
FlowServices : 단일 서비스 내에서 일련의 서비스를 캡슐화하고 이들 간의 데이터 흐름을 관리하고 여러 애플리케이션 끝점을 포함하는 복잡한 고급 통합 시나리오를 만들 수 있습니다<br/>
APIs : REST API 및 SOAP API를 사용하여 외부 세계에 노출 될 수 있습니다 .<br/>
configuration : 워크 플로 및 FlowService 구성을 관리 할 수 있습니다<br/>

## 4회
1.트리거의 정의<br/>

트리거 는 정의 된 이벤트가 발생하면 자동으로 워크 플로를 시작하는 강력한 도구입니다<br/>
2.트리거의 타입<br/>

외부 앱 또는 서비스에서 이벤트가 발생하면 트리거가 워크 플로를 시작합니다<br/>
정기적으로 (예 : 5 분마다) 변경 사항을 확인합니다. 이러한 유형의 트리거를 폴링 트리거 라고 합니다<br/>
실시간으로 webMethods.io Integration에 데이터를 전송하여 외부 앱 또는 서비스에서 지정된 이벤트가 발생하는 즉시 워크 플로를 실행할 수 있습니다.<br/> 이러한 종류의 트리거를 웹훅 트리거라고 합니다<br/>
3.트리거에 트위터를 연결하여 테스트함<br/>

    4. 트위터 연동 계정에 새로운 글을 올리지 않았을경우 error<br/>

    5. 트위터 연동 계정에 새로운 글이 게시되었을 경우<br/>

## 5회
1.액션의 정의<br/>
Actions은 트리거 될 때 워크 플로가 자동으로 수행하는 작업입니다<br/>

    2. 액션의 타입<br/>
services<br/>	unity<br/>	IOT<br/>



custom

## 6회
커넥터의 정의<br/>
    • 커넥터는 작업을 자동화하기 위해 워크 플로에서 사용할 수있는 여러 작업을 제공합니다.<br/>
커넥터의 유형<br/>
    • 서비스 : 서비스 범주에는 webMethods.io 통합에서 지원하는 모든 외부 웹 서비스 (커넥터라고 함)가 포함됩니다 (IoT 커넥터 제외).<br/>
    • 유틸리티 : 유틸리티 카테고리 아래에 나열된 것은 webMethods.io 통합 팀에서 만든 개발자 친화적 인 사용자 지정 응용 프로그램입니다.<br/> 이러한 애플리케이션 및 관련 작업을 사용하여 HTTP 요청을 보내고 복잡한 파일 작업을 수행하고 데이터를 변환 할 수 있습니다.<br/>
    • IoT : IoT 범주에는 webMethods.io Integration에서 지원하는 모든 IoT 기반 애플리케이션이 포함됩니다.<br/> 이러한 애플리케이션을 사용하여 다양한 IoT 장치를 webMethods.io Integration과 쉽게 통합하고 일상적인 활동을 단순화 할 수 있습니다.<br/>
    • 사용자 지정 : webMethods.io 통합을 사용하면 사용자 지정 코드를 추가하여 자신의 응용 프로그램과 작업을 만들 수 있습니다.<br/> 이러한 작업은 사용자 지정 범주에 나열됩니다 .<br/>
## 7회
트리거,커넥터의 계정 연동하는법을 알려줌<br/>
1. 키를 생성하여 계정 생성<br/>

    2. 기존 키를 사용하여 계정 생성<br/>

3. 연결 기반 커넥터에 대한 계정 만들기<br/>

## 8회
레시피에서 워크 플로를 가져 오거나 내 보냅니다.<br/>
레시피에서 계정으로 웹 서비스 별 워크 플로를 가져오고 사용자 지정 워크 플로를 레시피로 내보내는 방법을 알아 봅니다<br/>
Recipes import<br/>

Recipes export<br/>

My Recipes<br/>

