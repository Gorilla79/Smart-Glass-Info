# 🧠 Smart Glass Module Overview

본 프로젝트는 **Smart Glass 모듈**을 구성하는 하드웨어 요소들을 정리하고, 각 구성요소에 대한 3D 모델 파일 정보를 제공하기 위한 문서입니다.

---

## 📦 1. 전체 구성도

Smart Glass는 다음과 같은 구성 요소들로 이루어져 있습니다:

- **Raspberry Pi Zero 2W**
- **ReSpeaker 2-Mics Pi HAT**
- **Bone Conductor Transducer (골전도 트랜스듀서)**
- **Camera (IMX219-77)**
- **Laser Neopixel LED**
- **Battery**

---

## 🔍 2. 모듈별 상세 정보

### 📷 2.1. 카메라 (Camera)

- **모델명**: IMX219-77 (Raspberry Pi Camera)
- **파일명**:
  - `카메라 모듈.step` *(obj, f3d 사용 가능)*
  - `IMX219-77 카메라 모듈.step` *(obj, f3d 사용 가능)*
- **원본**: `raspberry-pi-camera-4.snapshot.1`

---

### 🔴 2.2. 레이저 모듈 (Laser)

- **모델명**: [LB laser] RED 8x20 (10)
- **파일명**: `레이저 모듈.step` *(obj, f3d 사용 가능)*
- **특이사항**:
  - 기존 모델링 모듈과 다름
  - **기존 모델 직경**: 약 4.5mm → **현재 모듈 직경**: 약 8mm로 확장 필요

---

### 💡 2.3. Pixel LED (NeoPixel)

- **모델명**: WS2812B LED 네오픽셀 스트립 DM2036
- **파일명**: `DM2036_Pixel_LED.step` *(obj, f3d 사용 가능)*
- **특이사항**:
  - 단일 모듈 모델링 → 실제 사용 시 4개 연결 필요
- **원본**: `ws2812-60leds-m-5v-black-pbc-1.snapshot.4`

---

### 🔊 2.4. 골전도 모듈 (Bone Conduction)

- **모델명**: Bone conduction transducer 21×14mm
- **파일명**: `Bone Conducting Transducer.SLDRT` *(obj, step, f3d 변환 실패)*
- **특이사항**: Fusion 360에서 확인 불가 → **원본 모델만 참조 가능**
- **원본**: `adafruit-bone-conducting-transducer-1.snapshot.1`

---

### 🍓 2.5. Raspberry Pi Zero 2W

- **파일명**: `Raspberry Pi Zero 2 W.step` *(obj, f3d 사용 가능)*
- **원본**: `raspberry-pi-zero-2-w-1.snapshot.3`
- **사용 시 참고**: ReSpeaker 2-Mics Pi HAT와 **납땜하여 최소 높이로 사용**

---

### 🎙 2.6. ReSpeaker 2-Mics Pi HAT

- **파일명**: `Respeaker2MicPiHat.step` *(obj, f3d 사용 가능)*
- **원본**: `respeaker-2mic-pi-hat-1.snapshot.2`
- **사용 시 참고**: Raspberry Pi Zero 2W와 **납땜하여 사용**

---

### 🧩 2.7. Raspberry Pi Zero 2W + ReSpeaker HAT 결합

- **연결 방법**: 납땜
- **파일명**: `Raspberry Pi Zero 2 W & Respeaker2MicPiHat.step` *(obj 사용 가능)*
- **특이사항**: 실제 높이 미반영, 형태 참고용 모델링

---

### 🔧 2.8. PCB 및 프레임

- **PCB 파일**: `PCB.step` *(obj, f3d 사용 가능)*
- **안경 프레임 파일**: `Glasses.step` *(obj, f3d 사용 가능)*

---

## 📁 모델링 파일 요약

| 모듈             | 파일명                                     | 형식 지원                   |
|------------------|--------------------------------------------|-----------------------------|
| Camera           | 카메라 모듈.step / IMX219-77.step          | `.step`, `.obj`, `.f3d`     |
| Laser            | 레이저 모듈.step                           | `.step`, `.obj`, `.f3d`     |
| Pixel LED        | DM2036_Pixel_LED.step                      | `.step`, `.obj`, `.f3d`     |
| Bone Conduction  | Bone Conducting Transducer.SLDRT           | `.sldrt` only (변환 실패)   |
| Raspberry Pi     | Raspberry Pi Zero 2 W.step                 | `.step`, `.obj`, `.f3d`     |
| ReSpeaker HAT    | Respeaker2MicPiHat.step                    | `.step`, `.obj`, `.f3d`     |
| 결합 모델        | Raspberry Pi + Respeaker.step              | `.step`, `.obj`             |
| PCB              | PCB.step                                   | `.step`, `.obj`, `.f3d`     |
| Glass Frame      | Glasses.step                               | `.step`, `.obj`, `.f3d`     |

---

## 📌 참고 사항

- 모든 모델은 **Fusion 360** 기준 설계되었습니다.
- `.SLDRT` 형식은 **SolidWorks 전용**이며, 변환이 어려울 수 있습니다.
- 실제 제작 시 치수 및 형태를 기반으로 일부 모델 수정이 필요할 수 있습니다.

---
