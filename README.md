# 임베디드 시스템 설계 및 실험

## 프로젝트 개요
이 프로젝트는 수업시간에 배운 다양한 센서와 보드의 기능을 활용하여 **앰플 제조기**를 개발하는 것입니다. 주요 목표는 다음과 같습니다.

### 1. 블루투스 연동
- 스마트폰과 블루투스를 연결하여 **레시피 및 설정값을 전송**
- 사용자 정의 레시피 선택 가능

### 2. 인터럽트 활용
- **압력 센서**: 앰플이 설정된 양에 도달하면 자동으로 제조 중지
- **수위 센서**: 원재료 부족 시 즉시 사용자에게 알림

### 3. 센서 간 의존성 활용
- **블루투스 연결 후 솔레노이드 밸브 및 센서 활성화**
- **압력 센서가 설정 값 도달 시 솔레노이드 밸브 자동 제어**

## 제조 과정 시나리오
1. **사용자 시작**
   - 스마트폰과 블루투스 연결 후 레시피 선택
   - 선택한 레시피 정보를 보드로 전송

2. **제조기 준비**
   - 제조기가 재료 리스트 준비
   - 원재료 부족 시 사용자에게 알림
   - 용기를 올려두면 감지 후 제조 시작

3. **재료 분배 및 감지**
   - 솔레노이드 밸브 개방 후 재료 투입
   - 압력 센서가 설정 값 도달 시 밸브 닫힘
   - 원재료 부족 시 사용자에게 알림

4. **제조 완료 및 알림**
   - 마지막 재료 투입 후 제조 완료
   - 스마트폰을 통해 사용자에게 알림

## 레포지토리 내용
이 레포지토리에는 위와 같은 프로젝트 및 실습 코드가 포함되어 있습니다.  
각 폴더에는 관련된 코드와 보고서가 정리되어 있습니다.
