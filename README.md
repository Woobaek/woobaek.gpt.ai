# 화염 감지 AI 시스템

## 소개

이 프로젝트는 OpenMV 카메라와 TensorFlow Lite(TFLite) 모델을 활용하여 화재 및 연기를 실시간으로 감지하는 AI 기반 화재 감지 시스템입니다.

카메라 영상에서 화재(Fire), 연기(Smoke), 정상(Normal) 상태를 분류하며, 화재가 감지되면 UART 통신을 통해 아두이노 등 외부 장치에 신호를 전송할 수 있습니다.

## 주요 기능

* 실시간 화재(Fire) 감지
* 실시간 연기(Smoke) 감지
* 정상 상태(Normal) 분류
* TensorFlow Lite AI 모델 사용
* UART 통신을 통한 외부 장치 제어
* OpenMV 카메라 기반 임베디드 AI 구현

## 사용 방법

1. 프로젝트 파일을 OpenMV IDE에 업로드합니다.
2. `fire_model.tflite` 모델 파일을 OpenMV 보드에 저장합니다.
3. 카메라를 연결한 후 프로그램을 실행합니다.
4. AI 모델이 영상을 분석하여 화재, 연기, 정상 상태를 실시간으로 판별합니다.
5. 화재가 감지되면 UART를 통해 `"1"` 신호를 전송하고, 그렇지 않으면 `"0"` 신호를 전송합니다.

## 개발 환경

* OpenMV
* Python (MicroPython)
* TensorFlow Lite
* Arduino (UART 연동)

## 라이선스

MIT License
