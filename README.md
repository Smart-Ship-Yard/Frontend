# Frontend - 3D 디지털 트윈 관제 대시보드

## 개요
스마트 조선소 프로젝트에서 관리자가 보는 '모니터 화면' 역할을 함. 백엔드에서 전송한 실시간 AI 분석 데이터를 수신하여, 웹 브라우저상의 3D 조선소 모델(Digital Twin) 위에 위험 위치를 렌더링하고 즉각적인 알림을 표출함.

## 주요 기능
- 3D 디지털 트윈 렌더링: Three.js 및 WebGL을 활용한 선박 블록(glTF) 및 조선소 환경 3D 시각화
- 실시간 Red Alert: WebSocket 데이터를 수신하여 위험 위치에 핑(Ping) 점멸 효과 적용 및 공정률 시각화
- Click & View 팝업: 위험 알림 클릭 시 WebRTC 기반으로 딜레이 없이 현장 실제 CCTV 영상 팝업 표출
- 이벤트 통계: Chart.js 기반 누적 위험 이벤트 데이터 통계 대시보드 제공

## 사용 기술
- 언어: TypeScript
- 프레임워크: React.js
- 3D 렌더링: Three.js (@react-three/fiber)
- 시각화 및 통신: WebRTC, WebSocket, Chart.js

## 실행 방법
1. 레포지토리 클론 및 폴더 이동
`git clone https://github.com/조직명/Smart-Shipyard-Frontend.git`
`cd Smart-Shipyard-Frontend`
2. 패키지 설치
`npm install`
3. 개발 서버 실행
`npm start` (또는 `npm run dev`)
