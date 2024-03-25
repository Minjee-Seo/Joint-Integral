# Joint-Integral : 딥러닝을 이용한 관절염 진단 어플리케이션
2022-2학기 이화여자대학교 휴먼기계바이오공학부 캡스톤디자인 프로젝트

## Introduction
- 고령화 및 PC, 스마트폰 사용량 증가로 인해 어깨 관절 질환자가 급증하고 있음
- 관절 질환 진단 시 임상에서는 각도기나 육안을 통해 관절 최대 가동범위(ROM)를 측정함
- 객관성 및 재현성이 떨어지며 관절이 움직이는 속도를 고려하지 않는 평가방식
- 대형병원 쏠림 현상으로 인한 원격의료 활성화의 필요성

## Design objectives and requirements
- Keypoint Detection 기반 딥러닝 기술을 이용해 영상 기반 관절 최대 가동범위 및 각속도 측정 수행
- 새로운 관절 기능 평가 지표 제시 (static ROM, dynamic ROM)
- 측정기록을 데이터베이스화, 관절 건강 척도를 사용자 스스로 기록 및 판단할 수 있는 건강 관리 시스템을 제시
  
## Design solutions
- Pretrained lightweight-openpose 모델 파인튜닝을 통해 팔 관절 keypoint를 추론
- Flask 기반 어플리케이션을 통해 영상 업로드 및 실시간 추론, 진단결과 저장할 수 있도록 함
