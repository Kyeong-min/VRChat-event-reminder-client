VRChat event reminder
=====================

- [다운로드 (Alpha)](https://github.com/Kyeong-min/VRChat-event-reminder-client/releases/tag/alpha)

이 프로그램은 VRChat에서 개최되는 여러 이벤트에 잊지 않고 참여할 수 있도록 도와줍니다.

지정한 이벤트가 개최되기 전에 Windows toast notification 및 VR HMD에 오버레이로 알려줍니다.

# 현재 이 프로그램은 알파테스트중입니다.

알파테스트 중에는 아래 기능을 지원하지 않습니다.
- SteamVR 기동시에 Overlay표시를 위한 어플리케이션이 자동으로 실행되지 않습니다.
  - NotificationBroker/NotificationBroker.exe를 수동으로 실행시켜야 합니다.
- 인스톨러를 이용한 설치
  - Alpha버전에서는 압축 파일 형태로 제공됩니다.
- 이벤트 목록의 정렬, 검색 등

# 이 프로그램을 사용하기 위해서는 아래의 조건을 만족햐여야 합니다.

## 필수
- 윈도우 10 64bit
- ASP .NET Core Runtime 3.1.5 [다운로드](https://download.visualstudio.microsoft.com/download/pr/6818f1f7-75de-43e5-9202-2b328ca127f7/039edc4bab29e5af63ed618e59f82fad/aspnetcore-runtime-3.1.5-win-x64.exe)

## 선택
- Valve index, HTC Vive, Oculus, Windows MR 등, SteamVR 호환 VR 하드웨어
- SteamVR

````
VR하드웨어 및 SteamVR이 설치되어 있지 않은 환경에서는 Windows toast notification을 통해서만 이벤트를 알립니다.
````

# 간단한 사용법
1. 다운로드 한 후 alpha.zip 파일의 압축을 해제합니다.
2. aspnetcore-runtime-3.1.5-win-x64.exe를 실행하여 지시에 따라 설치합니다.
   - 이미 설치되어 있다면 설치하지 않아도 됩니다.
3. VRChatEventReminder 폴더의 VRChatEventReminder.exe 파일을 실행합니다.
4. 웹 브라우저를 실행하고 http://localhost:5000 을 입력하여 접속합니다. 크롬, 파이어폭스, 엣지 등을 추천합니다.
![01](image/kr/01.jpg)
    1. 오늘 개최가 예정된 이벤트의 목록입니다.
    2. 현재 개최된 이벤트 목록입니다.
    3. 이벤트 개최 통지 체크를 한 이벤트 목록입니다.
5. 오른쪽 메뉴에서 이벤트 목록 버튼을 클릭하고 참여하고자 하는 이벤트의 첫번째 행에 있는 체크박스에 체크를 합니다.
![02](image/kr/02.JPG)
   - 종료되었거나 시작된 이벤트는 체크할 수 없습니다.
6. 이제 이벤트가 시작하기 전에 이벤트가 곧 시작한다는 알림을 받을 수 있습니다.

## VR HMD에서 알림을 받기 위해서
1. NotificationBroker/NotificationBroker.exe 파일을 실행합니다.
   - 이 때, SteamVR이 실행되어있지 않다면 자동으로 실행됩니다.
2. 이제 이벤트가 시작하기 전에 이벤트가 곧 시작한다는 알림을 VR HMD에서 확인할 수 있습니다.
3. SteamVR Dashboard에서 VRChat event reminder 대시보드를 통해 알람의 표시 방법을 설정할 수 있습니다.
![gif01](image/001.gif)
4. 오퍼레이의 표시 위치, 크기, 투명도, 표시시간을 설정하고 Show sample notification 버튼 상호작용(대부분의 경우 컨트롤러의 트리거 혹은 HMD의 선택 버튼)을 통해 테스트할 수 있습니다.
![gif02](image/002.gif)

# 프로그램을 사용함에 있어 버그 등의 문제가 발생한 경우
어떤 조작을 하여서 무슨 문제가 발생하였는지 알려주신다면 테스트 및 개발에 큰 도움이 됩니다.

아래 두가지 방법 중 한가지 방법으로 저에게 알려주세요.

- 트위터 @isHATENA 에게 DM으로 알려주세요.
- [Github repository](https://github.com/Kyeong-min/VRChat-event-reminder-client/issues)에 issue를 만들어주세요.

저게에 알려주실 때 로그 파일을 함께 제공해주시면 문제 해결에 도움이 됩니다.
- VRChatEventReminder\log\ 경로에 있는 모든 *.log 파일
- NotificationBroker\logger.log 파일

# About
개발: HATENA @isHATENA

아이콘: コールマン＆アルナイル @callman_alnair