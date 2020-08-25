# Webmethods.io
webmethods.io youtube영상을 보고 나서 내용을 정리해보자

---
## Contents
[9. Project Parameters](#9.-project-parameters)<br/>
[10. Monitor](#monitor)<br/>
[11. Mapper](#mapper)<br/>
[12. Logger](#logger)<br/>
[13. HTTP Request](#http-request)<br/>
[14. Flow Services](#flow-services)<br/>
[15. Filters](#filters)<br/>
[16. Working with Workflows](#working-with-workflows)<br/>

## 9. Project Parameters

프로젝트 수준 매개 변수 (키-값 쌍)를 정의하고 해당 프로젝트의 모든 워크 플로에 전달합니다. 프로젝트 	수준 매개 변수가 무엇인지, 설정 방법 및 프로젝트에서 삭제하는 방법을 알아 봅니다.

###1) Adding a Parameters

Parameters로  값을 특정 키 (식별자) 바인딩 할 수 있습니다.<br/> 프로젝트의 모든 워크 플로 내에서 사용할 수있는 프로젝트에 대한 사용자 지정 키-값 쌍을 추가 할 수 있습니다.<br/> 이렇게하면 특정 값을 반복해서 입력 할 필요가 없습니다.<br/>


-1) 프로젝트 매개 변수를 추가하려면 매개 변수를 추가 할 프로젝트로 이동하고 구성 , 워크 플로 를 클릭 한 다음 매개 변수 를 클릭 합니다.<br/>
![000](https://user-images.githubusercontent.com/69182192/91126538-2b7e1480-e6df-11ea-9d04-8cd13aab552f.png) <br/>
사진에서 프로젝트에 정의 된 기존 매개 변수 목록을 볼 수 있습니다. 새 parameters를 추가하려면 New Parameters 버튼을 클릭 합니다.<br/>



![001](https://user-images.githubusercontent.com/69182192/91126541-2caf4180-e6df-11ea-9e83-48b7068b549c.png)<br/>
나타나는 팝업 창에 다음 세부 정보를 입력하십시오.<br/>
Name: project parameters 적합한 이름을 제공합니다.<br/>
Value: project prameters의 값을 제공합니다.<br/>
Mark as Mandatory : 선택적으로 지정된 parameters를 필수로 표시 할 수 있습니다. <br/>이러한 parameters의 경우 webMethods.io Integration은 워크 플로 실행시 parameters 값을 사용할 수 있는지 확인합니다.<br/> 값을 사용할 수 없으면 워크 플로 실행이 성공적으로 완료되지 않습니다. <br/>따라서 parameters를 필수로 표시하면 값이 있어야합니다.<br/>
Set as Password Field : 선택적으로 지정된 매개 변수를 비밀번호 필드로 표시하여 parameters 값을 숨길 수 있습니다.<br/><br/>
이 작업이 완료되면 Create를 클릭 합니다.<br/><br/>
그러면 parameters 탭 의 프로젝트 매개 변수 목록에 새로 생성 된  parameters가 추가됩니다 .<br/>
![002](https://user-images.githubusercontent.com/69182192/91126543-2de06e80-e6df-11ea-8235-8b7d46836cab.png)<br/>


-2) Workflow settings 패널에서도 프로젝트 parameters를 추가 할 수 있습니다 .<br/>
이렇게하려면 워크 플로를 열고 캔버스의 오른쪽 상단 모서리에있는 Workflow settings 아이콘을 클릭 한 다음 parameters를 선택 합니다<br/>
![003](https://user-images.githubusercontent.com/69182192/91126546-2e790500-e6df-11ea-9dfc-fccece94fd9a.png)<br/>






Add Parameter를 클릭합니다 .<br/>
![004](https://user-images.githubusercontent.com/69182192/91126548-2faa3200-e6df-11ea-9e2d-57ec5f2d9002.png)<br/>



관련 입력을 제공하고 옵션을 선택하여 parameters를 필수로 표시하거나 비밀번호 필드로 설정하십시오. 이 작업이 완료되면 add를 클릭 합니다.<br/>

### 1) editing Parameters

정의 된 parameters를 편집 할 수 있습니다.<br/>

이렇게하려면 Projects > Configurations > Workflow > Parameters 탭으로 이동 하여 편집 할 parameters를 찾습니다.<br/>

parameters 이름에 지정된 수직 줄임표 아이콘을 클릭하고 Edit parameters를 선택 하십시오 .<br/>
![000](https://user-images.githubusercontent.com/69182192/91127027-55840680-e6e0-11ea-9554-2d049847e733.png)<br/>

표시되는 창에서 필요한 사항을 변경하고 업데이트를 클릭 합니다.<br/>
![002](https://user-images.githubusercontent.com/69182192/91127067-69c80380-e6e0-11ea-99ca-00990685c529.png)<br/>

이렇게하면 지정된 parameters가 업데이트됩니다.

### 2) Deleting Parameters

프로젝트에서 정의 된 parameters를 삭제할 수 있습니다.<br/>

이렇게하려면 Projects > Configurations > Workflow > Parameters로 이동 하여 삭제할 parameters를 찾습니다.<br/>

parameters이름에 지정된 수직 줄임표 아이콘을 클릭하고 삭제를 클릭하십시오 .<br/>
![000](https://user-images.githubusercontent.com/69182192/91127291-ece95980-e6e0-11ea-80f6-8f4b14a7eb2d.png)<br/>

선택한 parameters가 영구적으로 삭제됩니다. 삭제하려는 parameters가 모든 워크 플로에서 사용되고있는 경우 삭제 를 클릭하면 대화 상자가 표시됩니다 .<br/>
![002](https://user-images.githubusercontent.com/69182192/91127292-ed81f000-e6e0-11ea-819b-7184a0c97a85.png)<br/>
    이 경우 parameters를 영구적으로 삭제하기 전에 먼저 지정된 워크 플로에서 parameters를 제거해야합니다.


### Using Parameters


프로젝트에 대한 Parameters를 정의한 후에는 해당 프로젝트의 모든 워크 플로우에서 사용할 수 있습니다. 이렇게하려면 Parameters를 사용할 워크 플로 작업을 엽니 다. 이 예에서는 이메일 보내기 작업 에서 Parameters를 사용합니다 .

작업 구성 창을 열면 창 왼쪽에 나열된 프로젝트 Parameters를 볼 수 있습니다. 관련 필드에서 Parameters를 드래그 앤 드롭 (또는 선택)하기 만하면됩니다.
![000](https://user-images.githubusercontent.com/69182192/91127453-42be0180-e6e1-11ea-9232-32d778df5c16.png)

그런 다음 평소처럼 나머지 워크 플로를 구성하고 저장합니다.

이제이 워크 플로가 실행될 때마다 이메일 키 의 값이 이메일 보내기 작업 의받는 사람 필드에 자동으로 채워집니다 .






## Monitor
실행 상태를 추적 및 모니터링하고, 자동 경고 규칙을 설정하고, 사용자 활동을 봅니다.<br/>

모니터 탭에는 다양한 작업을 수행 할 수있는 화면 왼쪽에있는 Execution Results , Alert Rules 및 General의 세 섹션이 있습니다.

### Execution Results
Execution Results 섹션은 각 실행 로그와 함께 워크 플로 실행 및 FlowService 실행 (활성화 된 경우)과 관련된 통계에 대한 빠른 개요를 제공합니다.
### Alert Rules
webMethods.io 통합을 사용하면 워크 플로 또는 FlowService가 실패하거나 시간 초과되거나 실행이 완료 될 때 특정 사용자에게 알림을 보내도록 프로젝트에 대한 자동 경고 규칙을 설정할 수 있습니다.
### General
General 섹션에서는 감사 로그를 통해 테넌트 활동을보고 추적하고 모니터링하고 트랜잭션 기반 테넌트에 대한 이번 달의 트랜잭션 사용 통계를 볼 수 있습니다.

## Mapper
webMethods.io Integration에서 지원하는 작업으로 데이터 변환을 달성하는 방법을 이해합니다.<br/><br/>
변환 기능을 사용하면 입력 데이터에 대해 다양한 작업을 수행하여 워크 플로 출력 또는 다음 작업으로 보내는 데이터를 사용자 지정할 수 있습니다. 이 기능은 webMethods.io 통합에서 지원하는 모든 작업에서 사용할 수 있습니다.

## Logger

## HTTP Request
HTTP에 요청을합니다. 예제를 통해 워크 플로에서 HTTP 작업을 구성하는 방법과 각 작업 필드가 나타내는 내용을 알아 봅니다. 지원되는 HTTP 메소드 중 하나를 사용하여 관련 서버에 요청할 수 있습니다
## Flow Services
es를 사용하여 단일 서비스 내에서 일련의 서비스를 캡슐화하고 이들 간의 데이터 흐름을 관리하고 여러 애플리케이션 끝점을 포함하는 복잡한 고급 통합 시나리오를 만듭니다.

FlowServices는 풍부한 데이터 매핑 기능, 익숙한 디버깅 메커니즘, 다양한 기본 제공 서비스 등을 제공합니다

## Filters
워크 플로에서 조건을 설정합니다. 예제를 통해 조건이 작동하는 방식과 두 작업 사이에 조건을 설정하는 방법을 이해합니다. 또한 webMethods.io Integration에서 제공하는 기본 제공 조건 연산자와 사용 방법을 알고 있어야합니다.

## Working with Workflows
