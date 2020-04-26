**소형 가구를 위한 원격 스마트 락 서비스**
=============

- 1, 2인 가구가 늘어남에 따라 개인 공간 방범에 대한 관심이 높아졌습니다. 이를 해결하기 위해 사용자 로그인과 모바일 앱을 통한 원격 잠금 및 해제를 제공하여 높은 보안성을 유지하며 거수자에 대한 데이터를 수집하여 사용자에게 더욱 강력한 보안을 제공하는 스마트 락 서비스입니다.

**해결 방법**
------------
1. 모바일 앱을 통한 원격 제어
- 모바일 앱에 사용자 로그인 시스템을 도입하여 해당 계정에 연결된 디바이스에 대해서만 잠금 및 해제를 할 수 있도록 합니다.
- 모바일 앱에서 잠금 및 해제 버튼을 이용하여 소켓을 통해서 서버, 아두이노 디바이스와 실시간 통신을 가능케하여 실시간으로 잠금 및 해제를 할 수 있게 합니다.
- 잠금 해제 이후 일반 도어락과 동일하게 자동으로 눌리는 물리적 센서에 의해 잠금이 이뤄질 수 있도록 합니다.

2. 거수자 확인
- 초음파 센서를 이용하여 실제 거주자가 잠금을 해제하고 문을 열기까지 걸리는 시간 동안 거리 데이터를 수집합니다.
- 이러한 데이터를 이용 및 분석하여 실제 거주자가 잠금을 해제하는 데 걸리는 시간을 초과하거나 측정되는 거리가 상당히 가까운 경우 등의 상황을 가정하여 실제 거주자와 거수자를 구분하여 이를 모바일 앱을 통해 알려줄 수 있도록 합니다.

**예상 시스템 구성도**
---------------
![시스템 구성도](https://user-images.githubusercontent.com/49565544/80301903-be667b00-87e1-11ea-986d-67a12196e141.png)

**개발 내용 및 순서**
```
1. React-Native를 이용하여 계정 및 잠금 해제 관련 UI 구현
2. 앱 - 서버 - 아두이노 소켓 통신 구현
3. 데이터 저장용 DB 테이블 구성
4. 서버 API 구현(라우터 구현)
5. 아두이노 회로 설계
6. 아두이노 코드 구현
7. 3D 프린터를 이용한 하드웨어 설계 및 제작
```
**기대 성과**
---------------
1. 보안성  
- 스마트 락과 모바일 앱간 통신을 통해 원격으로 잠금/잠금 해제를 제어할 수 있습니다. 이를 통해 사용자만이 스마트 락을 이용할 수 있는 철저한 보안을 제공합니다.

2. 편리성  
- 모바일 앱을 이용한 스마트 락으로써 잠금의 기능 외에 잠금 해제 기록, 범죄 행각 측정과 같은 여러 기능을 제공받을 수 있습니다. 또한 기존 물리적인 잠금장치에서 우려되었던 열쇠와 비밀번호의 분실에 대한 문제에서 자유로워질 수 있습니다.

**팀원**
--------
![준서사진](https://user-images.githubusercontent.com/49565544/79038549-15caef80-7c15-11ea-86c8-3a50f6775fc7.jpg)


### 박준서 (Leader)
```
■ 역할

1) 시스템 기획
2) 제품 하드웨어 디자인 개발
3) 프로젝트 관련 판넬제작 및 발표 
4) 수익모델 구조 구상
5) 회의 자료 정리 및 서기

```
![귬니 민증사진](https://user-images.githubusercontent.com/49565544/79038580-4874e800-7c15-11ea-987f-52f195b15403.jpg)

### 최규민 (Committer)
```
■ 역할

1) Github Committer
2) React-Native를 이용한 모바일 앱 프론트 엔드 구현
3) 모바일 앱 - 서버 - 아두이노 소켓 통신 구현
4) 모바일 앱 배포 및 관리
5) 아두이노를 이용한 잠금 장치 회로 설계 및 코드 구현

```
<img width="100" alt="정재 사진" src="https://user-images.githubusercontent.com/49565544/79038452-5413df00-7c14-11ea-84e7-2b5edcd0ba07.png">

### 오정재 (Developer)
```
■ 역할 

1) AWS 서버 관리
2) Nodejs 서버 구축
3) Express 프레임워크를 이용하여 라우터 처리
4) Mysql DB 구축
5) 계정, 잠금 해제 기록, 초음파 데이터 저장용 DB 테이블 설계
```

**개발 환경**
-------
개발 툴 : 
* Github, Slack, Arduino IDE, VS Code

개발 환경 :
* 언어 : JavaScript
* 백엔드 : Node.js
* 프론트엔드 : React-Native
* 데이터베이스 : MySQL

개발 방식 :
* Github Pull Request를 통한 Agile 방식의 프로젝트 구현

**개발 계획**
--------
* 개발환경 구축 및 기획 (2020.04.13 ~ 2020.04.20) - 완료

* 데이터베이스 구성 (2020.04.21 ~ 2020.04.24) - 완료

* 프론트 / 백엔드 및 아두이노 제품 개발 (2020.04.25 ~ 2020.06.01)

* 프로젝트 수정 및 완정 + 발표 준비 (2020.06.02 ~ 2020.06.07)





