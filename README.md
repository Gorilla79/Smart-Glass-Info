# Smart-Glass-Info

--------------------------------------------------------------------------------
## Smart Glass Module 정리
1. 전체 구성도 </br>
Smart Glass 모듈은 다음 핵심 구성 요소들로 이루어져 있습니다:</br>
• Raspberry Pi zero 2W</br>
• ReSpeaker 2-Mics Pi HAT</br>
• Bone Conductor Transducer (골전도 트랜스듀서)</br>
• Camera (카메라)</br>
• Laser neopixel led (레이저 네오픽셀 LED)</br>
• Battery (배터리)</br>

--------------------------------------------------------------------------------
2. 모듈별 상세 정보
</br>
2.1. 카메라</br>
• 모델명: IMX219-77 (라즈베리파이 카메라)</br>
• 카메라 모듈 파일명: 카메라 모듈.step (obj, f3d 파일 사용 가능)</br>
• 카메라 파일명: IMX219-77 카메라 모듈.step (obj, f3d 파일 사용 가능)</br>
• 원본 파일명: raspberry-pi-camera-4.snapshot.1</br>
</br>
2.2. 레이저</br>
• 모델명: [LB laser] 레이저 모듈 (RED 8x20)-(10)</br>
레이저 모듈 파일명: 레이저 모듈.step (obj, f3d 사용 가능)</br>
• 특이사항: 이 모듈은 실제 모델링 할 때 사용된 모듈과 다르므로, 기존 모델링의 레이저 모듈 부분을 확장해야 합니다. 기존 모듈의 직경은 약 4.5mm였으나, 현재 모듈의 직경은 약 8mm입니다.</br>
</br>
2.3. Pixel LED</br>
• 모델명: WS2812B LED 네오픽셀 스트립 DM2036</br>
• LED 모듈 파일명: DM2036_Pixel_LED.step (obj, f3d 사용 가능)</br>
• 특이사항: 본 모델링 파일은 모듈 1개만 모델링되어 있으므로, 실제 사용된 모듈과 같은 형태를 나타내기 위해서는 4개의 모듈을 연결하여 사용해야 합니다.</br>
• 원본 파일명: ws2812-60leds-m-5v-black-pbc-1.snapshot.4</br>
</br>
2.4. 골전도 모듈</br>
• 모델명: Bone conduction transducer 21*14mm</br>
• 골전도 모듈 파일명: Bone Conducting Transducer.SLDRT (obj, step, f3d 파일 변환 실패)</br>
• 특이사항: 본 모델링 파일은 퓨전 360에서 확인이 불가능하여 원본 모델링 파일만 참조해야 합니다.</br>
• 원본 파일: adafruit-bone-conducting-transducer-1.snapshot.1</br>
</br>
2.5. Raspberry Pi Zero 2W</br>
• 라즈베리파이 보드 파일명: Raspberry Pi Zero 2 W.step (obj, f3d 사용 가능)</br>
• 원본 파일명: raspberry-pi-zero-2-w-1.snapshot.3</br>
• 실제 사용 시: ReSpeaker 2-Mics Pi HAT와 납땜하여 최소한의 높이로 사용해야 합니다.</br>
</br>
2.6. ReSpeaker 2-Mics Pi HAT</br>
• 오디오 확장 보드 파일명: Respeaker2MicPiHat.step (obj, f3d 사용 가능)</br>
• 원본 파일명: respeaker-2mic-pi-hat-1.snapshot.2</br>
• 실제 사용 시: Raspberry Pi zero 2W와 납땜하여 최소한의 높이로 사용해야 합니다.</br>
</br>
2.7. Raspberry Pi Zero 2W & ReSpeaker 2-Mics Pi HAT 결합</br>
• 연결 방법: 납땜을 하여 연결합니다.</br>
• 모델링 특이사항: 본 모델링은 정확한 높이를 반영하지 않았으나, 형태를 예상하기 위해 제작되었습니다.</br>
• 결합된 형태 파일명: Raspberry Pi Zero 2 W & Respeaker2MicPiHat.step (obj 사용 가능)</br>
</br>
2.8. PCB</br>
• 스마트 글래스 PCB 파일명: PCB.step (obj, f3d 사용 가능)</br>
• 글래스 파일명: Glasses.step (obj, f3d 사용 가능)</br>

--------------------------------------------------------------------------------
