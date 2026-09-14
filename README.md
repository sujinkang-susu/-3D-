# -3D-# 생산·품질 보고서 및 3D 검사·이송 설비 웹 서비스

**날짜:** 09월 14일

## 사용 라이브러리

* Python
* Flask
* Werkzeug
* Three.js
* OrbitControls
* HTML5
* CSS3
* JavaScript
* JSON
* Cloudflared
* asyncio
* threading
* urllib
* pathlib

## 설명

생산·품질 데이터를 조회하고 설비 상태와 관련 기록을 확인하여 업무 보고서를 작성할 수 있도록 구현한 교육용 웹 서비스입니다.

사용자는 조회할 날짜와 생산 라인을 선택하여 생산량, 목표 생산량, 생산 달성률, 검사 수량, 불량 수량 및 불량률을 확인할 수 있습니다.

주요 기능은 다음과 같습니다.

* 날짜 및 생산 라인별 생산·품질 데이터 조회
* 생산량 / 목표 생산량 표시
* 생산 달성률 계산 및 표시
* 검사 수량 / 불량 수량 표시
* 불량률 계산 및 표시
* LOT별 생산·검사 기록 조회
* 일자별 불량률 시각화
* 설비 사건 및 상태 이력 확인
* Three.js를 활용한 패널 검사·이송 설비 3D 시각화
* 마우스를 이용한 3D 설비 회전 및 확대/축소
* 생산·품질 데이터를 기반으로 업무 보고서 초안 생성
* 보고서 본문 수정 및 검토 상태 저장
* 보고서 TXT 파일 다운로드
* 보고서 근거 데이터 JSON 파일 다운로드
* Flask 기반 웹 서버 실행
* Cloudflared를 이용한 외부 접속 주소 생성

생산 달성률은 다음과 같이 계산합니다.

`생산 달성률 = 생산 합계 ÷ 목표 합계 × 100`

불량률은 다음과 같이 계산합니다.

`불량률 = 불량 합계 ÷ 검사 합계 × 100`

Three.js로 검사·이송 설비의 프레임, 컨베이어 롤러, 검사 구역, 검사 카메라, 디스플레이 패널, 조작부 및 타워 램프 등을 3D 형태로 표현했습니다.

본 프로젝트에서 사용하는 생산량, 검사량, 불량 수량, 설비 상태 및 사건 기록은 실제 생산 데이터가 아닌 **교육 및 실습 목적의 가상 데이터**입니다.

## 참고 문헌들

* Three.js Documentation
  https://threejs.org/docs/

* Three.js OrbitControls Documentation
  https://threejs.org/docs/#examples/en/controls/OrbitControls

* Flask Documentation
  https://flask.palletsprojects.com/

* Werkzeug Documentation
  https://werkzeug.palletsprojects.com/

* Cloudflare Tunnel Documentation
  https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/

* Python Documentation
  https://docs.python.org/3/

* MDN Web Docs – HTML / CSS / JavaScript
  https://developer.mozilla.org/
