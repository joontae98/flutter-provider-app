# Flutter Provider App
**Provider** 패턴을 이해하기 위한 **App**

### Provider
provider는 Google IO에서 추천되어 가장 큰 주목을 받는 디자인 패턴이다. 이것은 원래 구글에서 만든 것은 아니고 커뮤니티에서 만든 플러그인인데 구글에서 공식적으로 추천하였다.   
이전 Google IO에서는 BLoC 패턴 사용을 권장하였지만 단순한 로직을 구현하기 위해서도 4개 정도는 클래스를 만들어야 하므로 사람들이 어려워했다. 반면 Provider 패턴은 데이터 공유나 로직의 분리를 좀 더 간단히 할 수 있습니다.   
Provider 패턴은 한 클래스가 하나의 역할만 하도록 나누고 또한 데이터의 공유를 쉽게 할 수 있다. 여기까지는 BLoC 패턴과 유사하지만 큰 차이점은 BLoC 패턴의 경우 클래스들을 역할별로 나누는 데는 좋지만, 코드 자체가 복잡해지는 경우가 있고, Provider 패턴의 경우 좀 더 적은 코드로 깔끔하게 클래스들을 구분해서 사용할 수 있다.   
구글에서도 중소규모 프로젝트는 Provider 패턴을, 대규모 프로젝트에는 BLoC 패턴을 추천한다.   
Provider는 크게 두 가지 생산과 소비 부분으로 나눌 수 있다. 데이터를 만드는 곳과 쓰는 곳이 분리되어 있다. Provider의 값을 이용하고 싶으면, 값을 이용하고 싶은 위젯을 Provider로 감싼다. 그러면 그 밑의 위젯에서는 Provider의 값을 사용할 수 있다.
