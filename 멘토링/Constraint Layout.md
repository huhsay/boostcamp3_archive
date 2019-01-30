# Constraint Layout

**2016 google I/0 conference**



**Anchor Points**에 제약사항을 걸어서 어떻게 위치를 할 것인가.

**Center Point**

**Baseline** 텍스트뷰를 상속받은 뷰들만 보이는 제약



**Left/Start - Right/End**

Left나 Right는 국가와 상관없이 고정

Start나 End는 국가별 글자의 정렬에 따라 위치가 바뀐다.



**주의 할점**

제약 조건은 수평이나 수직은 모두 설정해 주어야한다.



## **Dimension Rules**

(차원규칙)

fixed: dp 단위로 표현 된 고정 치수

wrap_Content: 내용에 맞게

0dp(match_constraint):제약조건에 따라 뷰의 길이가 변함. 상하 또는 좌우의 앵커 포인트가 연결되어 있어야 함.



**겹치는 상황이 발생할때**

app:layout_constrainedWidth="true" - 길이가 늘어나면 줄바꿈을 한다.

- 아직 design tools에서는 사용할 수 없고 직접 코드를 작성해 주어야 한다.



## Margin

**layout_GoneMarginStart**

내가 타겟팅한 뷰가 사라졌을 때 사용한다.

target이 Gone 되면 사라지는 것이 아니라 odp의 뷰가 되는 것이다. 



## Biasing constraints



## Chains

제약조건이 없는 뷰를 선택하여, 마우스 오른쪽 버튼을 눌러 체인을 만들수 있다. 코드로 할때는 양쪽의 뷰를 모두 제약을 걸어야 한다.

- packed : 뷰들이 가운데 붙는다.
- spread_insid : 왼쪽끝과 오른쪽 끝의 마진값을 설정한 상태에서 가운데 뷰들이 spread된다.
- spread(기본값) : 전체 뷰를 균등한 값으로 마진 값이 설정된다. 



## Helper

### GuideLines



### Groups

여러개의 뷰를 하나로 묶는다.

### Barriers

그룹과 비슷하나 가상의 벽을 만든다고 생각하여 

