# falko(무단 착석 감지 시스템)


falko 사용법<br/><br/>
-------------
[주요 기능]


<br/>
<img src="https://github.com/eane13/falko/assets/133244019/9f5e8cb8-5d5c-4236-a103-1de473d27fc6.png"/><br/><br/>
① 좌석 위치 정보 생성<br/>
: 각 상영관 A, B, C, D에 연결된 카메라를 통해 하나의 frame을 캡쳐한 후, 해당 frame 내의 좌석을 인식한다. 그와 동시에, 인식된 좌석을 A1부터 열대로 라벨링하며 좌석 번호를 자동으로 부여하고, 이를 ‘좌석번호 : [좌석이 위치한 좌표 값]’의 형태로 좌석 위치 정보 텍스트 파일을 생성한다.<br/><br/>
<img src ="https://github.com/eane13/falko/assets/133244019/150662c4-0a2a-4fbb-a703-5b6b4adc7257.png" width=300" height="250"/>
<img src ="https://github.com/eane13/falko/assets/133244019/ff81935e-bca1-4a2f-8b7a-02ab3fd41b38.png" width=300" height="250"/>
<img src ="https://github.com/eane13/falko/assets/133244019/7b848fa4-f9c3-4852-90f7-c8a5019a0cc6.png" width=300" height="250"/><br/><br/>
② 좌석 위치 정보 설정<br/>
: 사용자는 ①에서 생성한 좌석 위치 정보 파일을 시스템에 설정한다.<br/><br/>
<img src ="https://github.com/eane13/falko/assets/133244019/171d2643-290f-4752-8677-add362e53515.png" width=300" height="250"/>
<img src ="https://github.com/eane13/falko/assets/133244019/bb15a31b-b35d-42de-9653-888e07e1fa7d.png" width=300" height="250"/>
<img src ="https://github.com/eane13/falko/assets/133244019/c4aef8a2-3f65-4de8-86e7-a2a515e4d772.png" width=300" height="250"/><br/><br/>


③ 카메라 ON/OFF <br/>
: ON 버튼을 누르면 무단 착석 감지를 시작한다. 이때 ON 버튼은 비활성화되며, OFF 버튼이 활성화된다.<br/>
: OFF 버튼을 누르면 무단 착석 감지를 종료한다. 이때 OFF 버튼은 비활성화되고, 다시 ON 버튼이 활성화된다.<br/><br/>
![카메라1](https://github.com/eane13/falko/assets/133244019/4fe9529c-af39-4acb-a251-659081c84ae1)
![카메라2](https://github.com/eane13/falko/assets/133244019/6b8792da-4f74-4755-87bd-8cb1e5e2d4f1)<br/><br/>

④ 무단 착석 감지<br/>
: 시스템에 미리 설정한 좌석 좌표를 기준으로, 예매되지 않은 좌석 좌표와 실시간으로 인식 중인 사람 객체의 좌표가 일정 비율로 10 frame 이상 겹치면 해당 좌석 영역에 빨간 박스를 그린다.<br/><br/>

⑤ 무단 착석 정보 제공<br/>
: 무단 착석한 사람이 앉아있는 좌석 번호를 띄운다.<br/><br/>

⑥ 예약된 좌석 수 & 인식된 사람 수 정보 제공<br/>
: 영화 사이트를 통해 각 A, B, C, D 상영관에 예약된 좌석 수와, 각 상영관에 현재 인식중인 사람 수 정보를 제공한다.<br/><br/>

⑦ 저장 & 종료<br/>
  -1) 저장 : 사용자가 Save 버튼을 누른 시점의 무단 착석 좌석 정보가 텍스트 파일로 저장된다. 이때, 사용자는 파일이 저장될 경로 및 이름을 설정할 수 있다.<br/>
  -2) 종료 : Quit 버튼 및 Esc 버튼을 누르면 프로그램이 종료된다.<br/><br/>


[기타 기능]<br/><br/>

1. GUI 크기 자동 설정 <br/>
: 사용자의 화면 크기에 맞게 GUI 크기가 자동으로 조정된다. <br/><br/>

2. 경고창<br/>
![경고창](https://github.com/eane13/falko/assets/133244019/99cba71c-d84c-427c-a1d3-2b1a65985c67)<br/>
 : ②에서 좌석 위치 정보를 설정하지 않은 상태에서 카메라 ON 버튼을 누르면 좌석 위치 정보를 설정하라는 경고창이 뜬다.<br/><br/>

