# toonflix

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.


## Reuserable Widgets
- Error Lens : 뭐 대충 vscode에 에러내용 바로 표시해주는 확장익스텐션
- mainAxisAlignment.between : 두 버튼 사이에 최대치로 떨어뜨릴때 사용
- 재사용 가능한 부분을 위젯으로 만드는 방법
- code Action 버튼을 통해서 자동완성 기능이 유용함

## Transform
- Transform은 어떤 위젯에 대해서만 주위에 영향을 주지 않고 사이즈를 키우거나 변형,위치이동 등에 사용됨
- clipBegavior : overflow되는 부분 어떻게 처리할건지

## FutuerBuilder
- API를 가져와서 그려줄때 await나 state를 사용하지 않고 가능하게 해줌
- Stateless에서는 프로퍼티를 API를 사용하는데 사용할 수 없음 
  - 그래서 Stateful로 변경
  - stateless를 steteful로 바꾸면 title -> widget.title로 변경됨
  - widget은 부모한테 가라는 의미, widget을 사용하는 이유는 별개의 클래스로 작업되기 때문
  - Constructor에서 불가능한 API fetch작업은 initState()에서 해야함

- ListView는 많은 값들을 보여줄때 주로 사용 (ListView의 단점은 모든 데이터가 로딩되고 뜸. 즉 모든 데이터가 메모리에 상주함)
- ListView.builder -> 리스트 빌더의 옵션을 선택해서 만들수잇음
- ListView.separated -> 리스트 빌더 아이템 사이사이에 빌드되는 것

## DetailScreen
- GesturDetector : 사용자의 조작을 감지 (탭, 탭다운 탭업 등)
- Navigator.push : 애니메이션 효과로 다른페이지로 이동한것처럼 보이게 해줌
- navigator.route -> MaterialPageRotue -> DetailScreen

## Hero
- Hero 위젯을 통해서 tag를 달아주면 동일한 이미지를 이동시켜서 사용하는 애니메이션 효과를 줄 수 있음

## FLutter에서 URL열기
- url_launcher 설치 (pub.dev)
- 해당 패키지 doc에 따라 configuration 파일 손봐야함

## 사용자 데이터를 저장하는 방법
- shared_preferences 라는 패키지를 사용
- 이것도 document 참고하면 될듯