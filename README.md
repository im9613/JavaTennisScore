# JavaTennisScore(테니스 계수기)

## 프로젝트 개요
테니스 경기의 점수를 실시간으로 기록하고 열람할 수 있는 계수기입니다.
점수를 랜덤하게 추가 및 추적하고, 듀스, 매치포인트, 타이브레이크를 구현하여 각 세트의 승자를 자동으로 계산할 수 있습니다.

<br>

## 주요기능
- **점수 난수 입력**: 각 플레이어의 점수를 랜덤하게 부여하며 게임을 진행합니다.
- **점수 규칙 설정**: 듀스, 매치포인트, 타이브레이크를 구현하여 점수 상황에 맞는 게임 진행을 할 수 있습니다.
- **기타**: 콘솔 기반 인터페이스로 사용자에게 출력하여 보여줍니다.
  
<br>

## 기술 스택
- **언어**: Java
- **개발 환경**: Windows 10/11, Java(JDK11), Eclipse
- **기타**: 콘솔 기반 인터페이스 제공

<br>

## 담당 업무
- 포인트 게임 듀스 기능 구현
- 등록된 선수 목록 조회 구현
- 메인 메뉴 GUI, 기능 연결 구현
- 클래스 다이어 그램 작성

  <br>

## UML 클래스 다이어 그램
  ![UML](https://github.com/im9613/JavaTennisScore/blob/main/Tennis/UML.png)

  <br>
  
## 기능
- **프로그램 메인**: 실행 시, 콘솔에 출력되는 화면
  ![메인화면](https://github.com/im9613/JavaTennisScore/blob/main/Tennis/MainMenu.png)

<br>

- **경기 시작**: 등록된 선수 2명의 이름 입력 후 경기 진행
  ![경기시작](https://github.com/im9613/JavaTennisScore/blob/main/Tennis/StratGame.png)

<br>


- **점수 구현**: 포인트 40-40 도달 시, 듀스 발생. 한쪽이 2점 선 취득 시 까지 반복 진행, 게임스코어 6대6 도달 시, 타이브레이크 진행.
  ![점수구현](https://github.com/im9613/JavaTennisScore/blob/main/Tennis/DueceTie.png)

<br>


- **저장 및 메인으로 이동**: 경기가 완전히 종료 된 후 경기 결과 출력 및 BufferWriter로 저장이 이뤄지며, 메인 화면으로 이동할 수 있다.
  ![저장,이동](https://github.com/im9613/JavaTennisScore/blob/main/Tennis/SaveReturn.png)

<br>


- **경기 기록 조회**: 끝난 경기 리스트를 불러오고 해당하는 번호를 입력하여 해당 경기 결과 스코어보드를 확인할 수 있다.
  ![결과로드](https://github.com/im9613/JavaTennisScore/blob/main/Tennis/LoadGame.png)

## 느낀점
기능이 얼마 없다고 생각한 프로그램인데도 UML 다이어그램을 작성해보니 구조가 복잡하게 얽혀있었습니다. 학습 당시 메서드가 어떤식으로 호출되고 동작되는지 감이 잡히지 않았으나 직접 사용해보니, 어떤식으로 사용되는지 알게되었습니다. 기초적인 개념 정리를 해야 추후 학습할 내용 습득에 유리할 것 같습니다. 좀더 많은 메서드 구현을 못해서 아쉬웠지만 나중에 제대로 된 기능을 가진 프로그램을 만들어보고 싶습니다.

