# Android Unit Test 활용법

**20190211**



## 컴파일, 빌드 , CI

컴파일 : 기계어로 번역 .java -> .class

CI : 젠킨스 같은거?

빌드는 컴파일이 아니다.

빌드는 전처리 컴파일 패키징 테스팅 배포를 포함하는 것이다.

빌드 툴은 gradle maven이 있다. 

안드로이드는 maven을 쓰다가 gradle로 



### Maven



### Gradle

Groovy 언어 기반이다.

균일한 빌드 환경을 만들어줌 -> 여러 사람이 같은 환경에서 빌드할수있게 해준다.

의존성 관리의 다양한 방법 제공



### Gradle Wrapper

gradlew -> local에 gradle을 다운 받아야 하는데 설치파일이 안에 제공되는 것.

gradlew.bat



### 안드로이드 gradle 빌드 시스템

Myapp

 \- build.gradle

 \- settings.gradle

 \- app

 \-\- build.gradle



### build.gradle: Project

### build.gradle: app

- 프로가드 -> 난독화 하는 것?
- 린트? 문법검사?  -> 정적검사 툴이라 보면 공부가 된다.



## Unit test

android unit test

- local unit test - jvm
- instumented test - 앱에서 돌아감



###  local unit test

- Mockito

- 안드로이드 의존성이 없는 테스트 (계산기를 만들어서 계산 로직이 맞냐?)

  

### instrumented test

- context를 사용할 수 있다. 의존성이 있다는 의미