# 2024-novel-physics

1. pc에서 ssh 클라이언트인 terminus를 사용하여 jetson 4GB에 접속함
2. 쿨링팬 동작, ros2 설치, barshrc 수정 후 ros 동작 확인
3. ROS navigation package 설치,  monicar2 code 설치, udev rule 설정
4.  micro_ros_arduino lib 및 PID lib 추가,  I2Cdev, MPU6050 lib 설치, pitches lib 추가 이후 ESP32에 코드 업로드
    코드 업로드 시 ESP32에 직결 후 업로드<br>motorEncExtraRos.ino 파일은 https://github.com/orocapangyo/monicar2/tree/main/arduino/motorEncExtraRos32 에서 다운로드 <br> **같이 위치한 songlcdled.h와 songcldled.ino 파일도 다운로드하여 동일 폴더 하에 둘것.**<br> **컴파일 과정에서 Adafruit GFX Library, Adafruit BusIO, Adafruit SSD1306 라이브러리 요구됨. 라이브러리 설치 후 진행** <br> 보드는 Node32s로 지정 -> 보드 이름을 찾을 수 없는 경우 아두이노 프로그램-파일-환경설정 이동하여 추가 보드 매니저 URL에 https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_dev_index.json 추가 후 재시도
5. micro_ros_setup을 설치 및 빌드함, micro-ROS Build 후 uros 생성 확인,
  참고(https://zeta7.notion.site/6-uROS-agent-5ccf4c0e063d45c383f5ab4de3dccb11)
  6-3장 에서 esp32를 jetson에 물린 뒤 PC에서 무선으로 원격 접속해 실행하니 문제가 해결됨.
