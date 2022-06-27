# 타이포라 사용 방법

[타이포라 사용방법 ](https://green-study.tistory.com/3523)



모든 명령 표시(에디터의 모든 명령에 접근)

- 맥 : cmd + shift + p

- 윈도우 : ctrl + s + p

  > 설정 :  **tab size** (공백 4 -> 2로 만드는 방법) 숫자 4를 2로 바꿔주기



css 링크 거는 법

- link rel="stylesheet" href="./main.css"



**기타**

- www.lipsum.com : 별 의미 없는 긴 문장이 필요할 때 사용하는 사이트



**text-decoration : none; 글자 밑 줄 없애기**



브라우저 초기화 방법

link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/reset-css@5.0.1/reset.min.css"



# css초기화 방법

- **reste.css cdn**

- <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/reset-css@5.0.1/reset.min.css">

#### *속성 죽이기*

*list-style:none; 으로 하면 앞에 아이템들의 점들이 없어진다.

*text-decoration:none 색상 밑줄 없애는 것.

*boreder-collapse:collapse 테이블에 선을 다 따로 떨어져있는 것을 붙여주는 기능.

*기본적으로 숨겨져있는 padding:0; / margin:0px; 죽여주기.





# 용어 저리 및 단위

1em = 10px "em의 기준은 글꼴 크기"

Rem =  "html 요소의 글꼴 크기 기준"

Vw = 

- "뷰포트는 브라우저 출력되는 페이지의 전체 영역 w는 가로 너비"
- 1vw 는 가로너비의 백분의 1너비

vh = "세로 너비 백분의 1너비"



Margin = 음수를 사용할 수 있음 / 단축속성 

- margin auto는 가운데 정렬에 활용함

- 외부 여백. 

  **Margin : top , right, bottom, left**

  **Margin : top, bottom / left,right**

  **Margin : top / left, right / bottom**

  **margin : top / right / bottom / left** 



padding = 내부의 여백 / 요소의 크기가 커짐



border = 요소의 테두리 선을 지정하는 단축 속성

- border-width "선-두께"
- Border-style "선-종류"
- Broder-color "선-색상"
  - 두께/종류/색상 순으로 작성하면 좋음.

none = 선 없음

Solid = 실선 (일반 선)

dotted = 점선

dashed = 파선

Double = 두줄 선

groove = 홈이 파여 있는 모양

Ridge = 솟은 모양 (groove의 반대 )

inset = 요소 전체가 들어간 모양

outset = 요소 전체가 나온 모양



border-color = transparent 투명색



**색상표현**

hex 색상코드 

- 16진수 색상 #000 / #FFFFFF

rgba

- 빛의 삼원색 + 투명도  rgba(0. 0. 0. 0.5) 0~1 투명도

hsl 

- 색상, 채도, 명도 hsl(120,100%, 50%)

hsla

- 색상, 채도, 명도 + 투명도 hsla (120, 100%, 50%, 0.3)



border-top : 두께 종류 색상 ;

Border-top-width : 두께 ;

Border-top-style : 종류 ;

Border-top-color : 색상 ;

나머지 속성 똑같음.





Border-radius : 테두리의 라운드

Box-sizing: border-box; 

- 요소의 내용 + padding + border로 크기 계산

Box-sizing :  content-box 

- 요소의 내용 (content)으로 크기 계산





# 포지션 : position

<포지션 정리>

position : relative 를 쓰면 원래 있는 그 자리에서 움직이는 것.

Position: absolute 내 아이템이  담겨있는 상자 안에서 옮겨지는 것. 
예를 들면 큰 상자속의 작은상자가  큰상자의 영역에 맞추어서 옮겨지는 것

Position:fixed는 큰상자안에서 작은상자가 완전히 벗어나서 웹페이지 상에서 옮겨지는 것

Position : sticky 는 원래의 자리에 있으면서 스크롤을 내릴때, 그 자리에서 고정되는 것.





# 선택자 갯수 늘리기

- .hero*15(늘리고싶은 갯수)>.image 하고 탭 

![image-20220519150657880](C:\Users\PublicAI\AppData\Roaming\Typora\typora-user-images\image-20220519150657880.png)





### background-attachment: fixed;

- 백그라운드 이미지가 고정이 된다.스크롤 할때!

### margin(외부여백)

- auto라는 속성을 쓸수 있다.
- 가로 사이즈가 있는 요소 있어야하고, block요소여야 / margin : auto를 쓰면 센터로온다.



### padding(내부여백)

- 



emmet ( 에밋 )

**input  사용자가 데이터를 입력하는 요소**

- 어떤 데이터 타입을 입력 받을 거지?

**Inline  글자를 만들기 위한 요소들**

**Block 상자(레이아웃)를 만들기 위한 요소들**

**span 콘텐츠 영역을 설정하는 용도. 본질적으로 아무 것도 나타내지 않음.(인라인 요소)**

- 요소가 수평으로 쌓임.
- <span> hello</span> <span>world</span>

**인라인 요소**(글자 요소)

- 포함한 콘텐츠 크기만큼 자동으로 줄어듬**
- 가로/세로 사이즈를 지정 할 수 없다.
- 마진/ 패딩은 위 아래 여백은 추가 할 수 없다. 좌/우는 여백을 할 수 있다.
- 인라인(글자)요소는 자식요소를 Block(상자)를 사용 할 수 없다.

**margin은 요소의 외부 여백을 지정하는 css속성**

**padding은 요소의 내부 여백을 지정하는 css 속성**

<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220504122253894.png" alt="image-20220504122253894" style="zoom:50%;" />

**div요소는 대표적인 Block 요소 본직적으로 아무것도 나타내지 않는 콘텐츠 영역을 설정하는 용도.**

- 포함한 콘텐츠 크기만큼 자동으로 줄어듬.
- 가로 넓이가 늘어남
- 가로/세로 넓이의 css 내부/외부 여백을 지정 할 수 있다.
- Block 요소는 자식요소로 Block 요소를 넣을 수 있고, 인라인 요소도 가능하다.

<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220504122624843.png" alt="image-20220504122624843" style="zoom:50%;" />

***Block 요소들***

- h1 : 제목을 의미하는 요소 (h6까지있음.)
- p :  문장을 구분하는 요소.

- ul : 순서가 필요 없는 목록의 집합을 의미
- li : 목록 내 각 항목 리스트



***Inline 요소들***

- img : 이미지를 삽입하는 요소
- a : 다른 / 같은 페이지로 이동하는 하이퍼링크를 지정하는 요소. (링크를 건다라는 의미)
  <a href="사이트 주소"> 텍스트 </a>
  <a href="사이트 주소" target="_blank"> 텍스트 </a>
- _blank : 링크 url을 페이지가 따로 생기는 것

- br  :  줄바꿈 요소 

- label  <input type = "checkbox"/>  : 라벨링이 가능한 요소의 제목
- label <input type = "radio" name="fruits"/ > : 사용자에게 체크여부를 그륩에서 1개만 입력 받음! 

<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220504125229352.png" alt="image-20220504125229352" style="zoom:50%;" />

<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220504125101441.png" alt="image-20220504125101441" style="zoom:50%;" />



**span 테그를 쓰면 동해물 이라는 글자만 따로 색상이나 크기를 변경할 때 영역을 구분지어서 사용 할 수 있다.** **글자들의 범위를 잡아낼 때 쓴다.**

<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220504124041660.png" alt="image-20220504124041660" style="zoom:50%;" />

<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220504124125157.png" alt="image-20220504124125157" style="zoom:50%;" />



**br/ : 줄 바꿈 할 때 사용**

<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220504124302081.png" alt="image-20220504124302081" style="zoom:50%;" />





***lnline-block 요소들***

- input : 사용자가 데이터를 입력하는 요소

<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220504124519374.png" alt="image-20220504124519374" style="zoom:50%;" />

<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220504124650902.png" alt="image-20220504124650902" style="zoom:50%;" />

<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220504124737677.png" alt="image-20220504124737677" style="zoom:50%;" />





<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220504124806343.png" alt="image-20220504124806343" style="zoom:50%;" />

<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220504124915604.png" alt="image-20220504124915604" style="zoom:50%;" />



***table 요소들***  (하나의 block 요소)

- 표 요소, 행과 열의 집합

- 표를 만들 땐 행을 먼저 한다.

- tr : 행 요소 / td : 열의 요소

  tr 

  td > 텍스트 </td

  /tr



<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220504125613193.png" alt="image-20220504125613193" style="zoom:50%;" />

전환효과 :  transition : 1s  

***a:hover 효과***



<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220509093038834.png" alt="image-20220509093038834" style="zoom:50%;" />



**a** 테그를 **active**(클릭하는 동안에만) 빨간색이 적용 되도록 하는 것.



**focus**

focus가 될 수 있는 요소는 **HTML 대화형 콘텐츠가** 해당 됨.

요소는  **INPUT / A / BUTTON / LABEL / SELECT** 등 여러 요소가 있다.

그리고 HTML 대화형 콘텐츠 요소가 아니더라도, tabindex 속성을 사용한 요소도 focus가 될 수 있다.

- 구글검색 : HTML 대화형 콘텐츠 mdn

- focus가 되지 않는 속성에 focus속성을 사용할려면, HTML에 tabindex 속성을 통해서 만들수 가 있다.

  순서(값)로 -1이 아닌 다른 값을 넣는 것은 논리적 흐름을 방해하기 때문에 권장하지 않는다.

  **( 예시  div class="box" tabinde="-1"></div>)**

  포커스라는 것은 하나의 페이지에서 한 요소만 가능 하기 때문에. 다른 포커스를 쓰면 다른 요소의 포커스는

  해제 된다.

빈 테그는 / 를 붙여주는게 좋다.





***first-child  요소 중 첫째라면 선택.***



<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220509094733021.png" alt="image-20220509094733021" style="zoom:50%;" />

***몇 번째 요소 라면 선택***

<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220509095127071.png" alt="image-20220509095127071" style="zoom:50%;" />

<*****> 하의 요소의 모든 요소를 선택

**(2) 두번 째 요소를 선택.** 

**(2n) n은 0부터 시작.( *일반적으로 1부터 시작한다.) - 자바에서 기본적인 내용**

- 0x2 = 0 

- 1x2 = 2

- 2x2 = 4

- 3x2 = 6

- 4x2 = 8 

  인데, 0은 곱해도 0이여서 없는 요소가 되어 2부터 시작한다. 그래서 수박 (2번째) / 망고(4번째) 

  가 선택이 된다.

**(2n+1)은 홀수 요소를 선택한다.**

- 0x2 = 0 + 1 = 1

- 1x2 = 2 + 1 = 3

- 2x2 = 4 + 1 = 5

- 3x2 = 6 + 1 = 7

- 4x2 = 8 + 1= 9

  마찬 가지로 +1이 되어 홀수가 되므로 0부터 시작한다. 

# :nth-child()

**(n+2)** n+ 숫자

<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220509100015459.png" alt="image-20220509100015459" style="zoom:50%;" />



***부정 선택자 not***

<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220509100254852.png" alt="image-20220509100254852" style="zoom:50%;" />

span테그가 아닌 요소를 선택하는 것!



***:before (인라인 요소)***

내부의 앞 쪽에 삽입하는 요소

***:after (인라인 요소)***

내부의 뒤쪽에 삽입하는 요소

css :  content를 꼭 사용해야됨.

예시

.box**::before** {

​	content: " before";

}

**inline 요소를 블록요소를 바꿀수 있는 요소는**

***display: block;*** 



속성 선택자 [ ] 대괄호

속성 선택자 포함하고 값이 요소 선택 [ ]

<img src="C:\Users\PublicAI\Desktop\github_jin\_posts\image\image-20220510101631306.png" alt="image-20220510101631306" style="zoom:50%;" />

스타일 상속

***inherit; (부모요소로 부터 값을 강제 상속 받는 것.)***



**overflow** 

visible : 넘친 내용을 그대로 보여줌

hidden : 넘친 내용을 잘라냄

scroll : 넘친 내용을 잘라냄, 스크롤바

**auto : 넘친내용이 있는 경우에만 잘라내고 스크롤바 생성**



**display** : 요소의 화면 출력(보여짐) 특성

**block : 상자(레이아웃)요소**

**inline : 글자 요소**

**inline-block : 글자 +상자요소**

*flex : 플렉스 박스 (1차원 레이아웃)*

*grid : 그리드 (2차원 레이아웃)*

*none : 보여짐 특성 없음, 화면에서 사라짐*

기타 : table, table-row, table-cell 등..



# **글꼴**

***serif : 바탕체***

***italic : 이텔릭체***

***sans-serif : 고딕체***

***cursive : 필기체***

***fantasy : 장식 글꼴***

***monospace : 고정너비 (가로, 폭 등)***

normal : 기울기 없음



**line-height : 한 줄에 대한 높이. 행간과 유사함.**

- 요소의 글꼴 크기의 배수로 지정

- 배수의 개념을 사용하는게 좋음.

**font-style : none ;  [기울기 없음]**

**font-weight : bold; / 700; [ 두껍게 ]**

- 100~ 900 : 100단위의 숫자 9개 normal 과 bold 이외 두께

- bolder 상위(부모) 요소보다 더 두껍게

- lighter 상위(부모) 요소보다 더 얇기

**font-size**

- 16px : 기본크기

 font-family : 글꼴1, "글꼴2",

**폰트의 띄어쓰기가 있으면  따옴표로 묶어야됨.**



# **문자속성**

**text-align : center ;  [ left, right, center, justify ]**

- text-decoration : none ; [ 장식없음 ]
- text-decoration : underline ; [ 밑 줄 ]
- text-decoration : overline ; [ 윗 줄 ]
- text-decoration : line-through [ 중앙 선 ] 

**text-indent : 들여쓰기** [음수로 쓰면 내여쓰기감]





# 배경

**background-color :** 컬러색상 ;

- transparent : 투명함 

**backgroubd-image:** url("경로");

**backgroud-size: **@@px ;****

- 요소의 사이즈에 맞게 조절 하면됨.
- auto : 이미지의 실제 크기 [기본 값]
- cover : 비율을 유지, 요소의 더 넓은 너비에 맞춤 
- contain : 비율을 유지, 요소의 더 짧은 너비에 맞춤 

**background-repeat** 

- no-repeat ; [반복하지 않고싶다.]
- repeat-x : [ 이미지를 수평 반복 ] 
- repeat-y : [ 이미지를 수직 반복 ]

**background-position** 

- center ; [중앙배치]

- top / bottom / left / right / center  방향

**background-position** : 100px 30px ; [ X축 / Y축 ]

**background-attachment :** 배경 이미지 스크롤 특성

- scroll : 이미지가 요소를 따라서 같이 스크롤
- fixed : 이미지가 뷰포트에 고정, 스크롤 X



# 배치

**position : 요소의 위치 지정 기준**

- absolute : 위치 상 부모 요소를 기준
  - *위치 상 부모 요소를 꼭 확인 해야됨.*
- relative :  요소 자신을 기준
- fixed : 뷰포트(브라우저) 기준
  - *top / bottom / left / right / zi-index*
  - *포지션과 같이 사용하는 css속성들은 모두 음수를 사용할 수 있음.*

- sticky : 스크롤 영역 기준 [배치와는 거리가 있음]



- [x] #### 중요

포지션이라는 속성을 쓰면 display:block 이라는 속성이 자동으로 들어가짐.

그래서 display:block을 사용할 필요가 없음.

예) span 테그는 인라인 요소이기 때문에, 가로/세로 값을 얻기 위해 display:block을 사용하면 가로/세로 값을 가질 수 있기 때문에 사용을 해야되지만,

position:absolute;를 쓰면 자동으로 block으로 바뀌어서 따로 block값을 따로 명시할 필요가 없다.

[position:absolute / fixed] 두 종류만 가능.

relative는 해당이 안됨.





## CSS의 배치 조건

1. 포지션의 값이 있는 경우.
2. z-index의 속성의 값이 더 크면 위에 쌓인다.
3. html 구조가 나중에 작성 된 것이 더 위에 쌓인다.



## flex 플렉스(정렬)

### **display:flex**

- 수평 정렬

display:flex 는 2가지 개념으로 나뉜다. **[flex-container / items]**

가 지정된 요소의 자식요소를 flex-itmes이라고 부른다.

### **display: inline-flex**

- 인라인 요소와 같이 flex container 를 사용할 수 있다.

- 블록 요소와 인라인 요소로 구분된다.

- 인라인 요소가 있어서 가로너비가 최소로 보여질려고 한다.

### **flex-direction** 행은 수평정렬

- 주 축을 설정
- 기본값은 row ( 행 축 좌->우 )
- row-reverse ( 행 축 우->좌 )
- column ( 열 축 위->아래 )
- column-reverse ( 열 축 아래->위)

### **flex-wrap** **: wrap**

- 기본 값은 nowrap

- flex items 묶음(줄 바꿈) 여부

- 기본 값 묶음(줄 바꿈) 없음
- wrap 여러줄로 묶음
- wrap-reverse  : wrap의 반대 방향으로 묶음

### **justify-content**

- 주 축의 정렬 방법 (x축) 수평정렬
- **flex-start**  flex items를 시작점으로 정렬
- **flex-end**  flex items를 끝점으로 정렬

- **center** flex items를 가운데 정렬
- **space-between** 각 flex items 사이를 균등하게 정렬
- **space-around** 각 flex items의 외부 여백을 균등하게 정렬

### **align-content**

- ***교차 축의 여러 줄 정렬 방법 (수직정렬)***
- **stretch**  flex items를 시작점으로 정렬
- **flex-start**  flex items를 시작점으로 정렬
- **flex-end**  flex items를 끝점으로 정렬

- **center** flex items를 가운데 정렬
- **space-between** 각 flex items 사이를 균등하게 정렬
- **space-around** 각 flex items의 외부 여백을 균등하게 정렬

### **align-items**

- ***교차 축의 한 줄 정렬방법***
- **stretch**  flex items를 교차 축으로 늘림
- **flex-start**  flex items를 각 줄의 시작점으로 정렬
- **flex-end**  flex items를 각 줄의 끝점으로 정렬

- **center** flex items를 각 줄의가운데 정렬

- **order flex item** 의 순서 [ 0 순서 없음 / 숫자가 낮을수록 앞으로 감.]

### flex-grow 

- ***flex item의 증가 너비 비율 [ 비율을 조정하는것 ]***

- 0  증가 비율 없음 / 숫자 증가 비율

### flex-basis

- 공간 배분 전 기본 너비
- 요소의 내용 너비 [auto]

### flex-shrink

- 1  flex container 너비에 따라 감소 비율 적용
- 숫자 감소 비율





# **전환효과**

### **transition**

- 중간단계를 자연스럽게 바뀌게해주는 것을 전환\
- 시작과 끝 효과를 지정하는 단축속성
- **transition-property**
  - 모든 속성에 적용 
  - 전환 효과를 사용할 속성 이름 명시
  - transition :  with 1s; 가로 너비만 해당
- **transition-duration**
  - 0s 전환효과없음
  - 지속시간을 지정
- **transition-timing-function**
- **transition-delay**
  - 전환 효과가 몇 초뒤에 시작할지 대기시간을 설정



**easing functions**

- esing 함수 치트 시트 링크 접속

**easing functions mdn**

**tweenmas easing**

- docs easing-greensock  사이트







# javaScrit

### 표기법

##### dash-case(kebab-case)

- the-quick-brown- : 단어와 단어사이에 **-** dash기호를 넣는 것을 말한다.

##### snake_case

- the_quick_brown_ : 단어와 단어사이에 _ 언더바를 넣는 것을 말한다.

##### camelCase (낙타라는 뜻을 가지고있음)

- theQuickBrownFox : 단어와 단어사이에 대문자로 표기하는 것을 말한다.
- 첫 번째 단어는 소문자로 시작함.

##### PascalCase

- 첫 번째 단어는 대문자로 시작함.  camelCase와 같은 표기.



### 주석

- 한 줄 메모 : //
- 한 줄 메모 : */ 

- /**

  *여러 줄

  *메모 1

  *메모 2
  */

  여러 줄일 때 이 방법의 주석을 쓰는 것이 좋음.



### 데이터 종류(자료형)

##### // string(문자데이터)

- 따옴표를 사용합니다.

- **let myName = "HEROPY";**

  myName 이라는 변수를 생성한다.

  그 변수를 선언하는 것이 let이라는 키워드

  myName이라는 변수에 = 할당할 것이다.

  할당할 데이터는 **"HEROPY"** 라는 글자 입니다.

  ; 으로 닫음으로써 마무리가 된다.

- let email = 'thesecon@gmail.com' ;

  email라는 변수에 thesecon@gmail.com 라는 문자데이터를 = 이라는 기호를 통해 집어넣는 할당이라는 개념.

  **console.log(email);** : 개발자 도구 **console**에 출력해볼려고 하는 것  // thesecon@gmail.com

##### `` backtick 기호 

- 보간법 : 보간법이란 **알고 있는 데이터 값들을 이용하여 모르는 값을 추정**하는 방법의 한 종류이다.

- let hello = `Hello ${myName}?!` : **$ {}** 중괄호 사이에 ~추가적인 데이터를 보간해서 채워 넣겠다.

  채워 넣는것 **myName** 들어 있으므로 출력이 되면 // **Hello HEROPY?!** 라고 출력이된다.

  > ***myName의 할당되는 데이터는 HEROPY 라는 글자이다.***

#### 문자 데이터는 따옴표로 정의를 할 수 있다.



##### // Number(숫자 데이터)

// 정수 및 부동소수점 숫자를 나타냅니다.

- let number = 123;  [123은 정수라는 숫자를 나타냄]

- let opacity = 1.57;  [1.57은 부동소수점 숫자를 나타냄] 

  opacity = 는 부동소수점을 사용 할 때 쓰는 변수



##### // Boolean(불린 데이터)

// ture, false  두 가지 값밖에 없는 논리 데이터입니다.

- let checked = true;  [ 참 ]
- let isShow = false;   [ 거짓 ]



##### // Undefined **: 의도적이지 않는** 

// 값이 할당되지 않은 상태를 나타냅니다.

- let undef;

- let obj = { abc: 123 };

  객체라는 뜻 (object)

  abc라는 속성에 123이라는 숫자데이터를 할당해서 넣어줄수 있음.



**comsole.log(undef); // undefined**

**comsole.log(obj.abc); // 123**

**comsole.log(obj.xyz); // undefined**



##### // Null

// 어떠한 값이 **의도적으로** 비어있음을 의미합니다.

- let empty = null;

  empty 라는 변수가 없다라는 것을 명시하는 것.



**// Object(객체 데이터)**

// 여러 데이터를 **Key:Value** 형태로 저장합니다. {    }

- let user = {

  // key : Value,

  name: 'HEROPY'

  age: 85,

  isValid: true

  };



**comsole.log(user.name); // HEROPY**

**comsole.log(user.age); // 85**

**comsole.log(user.isValid); // true**



##### // Array(배열 데이터)

// 여러 데이터를 순차적으로 저장합니다.  [  ]

- let fruits = [ 'Apple', 'Banna', 'Cherry' ];



**comsole.log(fruits[0]); // 'Apple'**

**comsole.log(fruits[1]); // 'Banana'**

**comsole.log(fruits[2]); // 'Cherry'**



 ratate(degree) 회전(각도)
 변환함수 2d
translate
 3d함수
perspective(n) 원근법(거리) / rotateX(x) 회전/  x, y 
 trasoform; translate(40px, 40px) 

 trasoform; translateX(40px) 인수
한 축만 이동 한다면 x,y로 쓰는 것을 권장한다
transform:scale(1.5) 숫자로 하고 크기를 크게 한다. 
값을 하나만 입력하면 x,y를 크게한다.
기본 값은 1이이다
 0.7이면 70퍼세트 크기로 줄인다 라는 뜻이다.
 rotate는 회전이라는 함수고 / deg는 각도라는 뜻이다. 
 기준을 옮길수가 있다 
원근법 함수는 제일 앞에 작성해야 한다.
prespective: 은 속성이라서 부모요소에 적용대상
transform:perspective 는 함수는 관찰 대상에 적용된다
 backface 는 뒷면 visibility는 보인다는 것임
backface-visibility 는 뒷면 보임 / 안보임 hidden
backface-visibility:hideen	 뒷면을 보여주지 않으면 뒷면은 투명하게 바뀌면서 안보인다.
skewX / deg 단위
기울이는 속성



// 재사용이 가능!
// 변수 선언!

let a = 2;
let b = 5;

console.log(a+b); // 7
console.log(a+b); // -3



// 값(데이터)의 재할당 가능

// 값(데이터)의 재할당 불가!

const a = 12;
console.log(a); // 12

a = 999;
console.log(a); // TtpeError: ~~~

const는 재할당이 불가 하여 에러가 뜸



예약어
특별한 의미를 가지고 있어, 변수나 함수 등으로 사용 수 없는 단어

Reserved Word



SyntaxError : 예약이 되어 있는 단어를 쓰면 에러가 된다

함수 특정 동작(기능)을 수행하는 일부 코드의 집합(부분)
funcion



// 함수 선언
function helloFunc() {
	// 실행 코드
	console.log(1234);
}

// 함수 호출

helloFunc() ;  // 1234



function retuFunc() {
	return 123;
}

let a = returnFunc() ;


console.log(a); // 123

*function 이라는 키워드를 통해서 함수의 이름 returnFunc() 이라는 이름을 만들었고 
return 이라는 반환 키워드를 작성함으로써 123이라는 숫자를 반환하고.

누가 받을 것이냐 let 이라는 키워드를 사용하는 a라는 변수가 retunFunc()이 호출 되면 반환된 숫자 123을 a가 받는 것이다.
a라는 데이터가 숫자 123이라는 데이터를 가지고 있는데, console 에다가 출력을 해보면 숫자 123이 나오더라.
[호출이라는 것은 실행이 된다라는 것]

그래서 추가적으로 사용할 수 있다.



// 함수 선언!

function sum (a, b) { // a와 b는 매개변수(Parameters)

return a + b;
}

// 재사용!



let a = sum(1, 2);  // 1과 2는 인수(Arguments)
let b = sum(7, 12) ; 
let c = sum(2, 4) ; 

console.log(a, b, c); // 3, 19, 6



// 기명(이름이 있는 ) 함수
// 함수 선언!

function hello() {
	console.log('Heoolo~');
}

// 익명(이름이 없는) 함수
// 함수 표현 !
let world = function () {



// 기명(이름이 있는 ) 함수
// 함수 선언!

function hello() {
	console.log('Heoolo~');
}

// 익명(이름이 없는) 함수
// 함수 표현 !
let world = function () {
	console.log('World~');
}

// 함수 호출
hello(); // Hello~
world(); // World~



// 객체 데이터
const heropy = {
	name: 'HEROPY',
	age : 85,

	// 메소드(Method)
	getName: function () {
		return this.name;
	}
};

const hisName = heropy.getName();
console.log(hisName);  // HEROPY

// 혹은
console.log(heropy.getName()); // HEROPY



// 객체 데이터 안에 하나의 속성부분에 하나의 함수를 할당하는 것을 속성이라고 부르지않고 메소드라고 부를 것이다.



조건문

조건의 결과(truthy, falsy) 에 따라 다른 코드를 실행하는 구문

if, else



let siShow = true;
let checked = false;

if (isShow)  {
    console.log('Show'); // show
}

if (checked) {
   console.log('checked');
}

거짓과 참을 사용하면서, 거짓은 콘솔에 보이지 않고 참은 보이는 것.



let isShow = true;

if (isShow) {
	console.log('Show');
} else {
	console.log('Hide');
}

여기서 참이 되면 isShow 가 출력이되고
거짓이면 isShow가 출력이 되지않고 그다음인
else 가 출력이 된다. 



DOM API
- document. object model 의 약어
- html의 object 요소라고 하고 div span 등 을 말함

APi 
- 어플리케이션의 (웹사이트)가 동작하는 프로그래밍 명령들

DOMAPI
html을 제어할 떄 사용하는 명령들 자바스크립트를 쓸때



let boxEl = doument.querySelector('.box');

comsole.log(boxEl);


<script defer src=를 쓰면 스크립트 테그를 읽을 수있음. 
defer가 없이 쓰면 html에 테그 가 명령이 되지않아 null이라고 뜬다.(콘솔창에)

아니면 body테그 맨 마지막에 집어 넣으면 읽게 되어 정상적으로 실행이 된다.

브라우저는 위에서 아래로 읽기 때문이다.
정보의 내용에 구조에 넣으면 좋은 방법이 아니기 때문에. 대도록이면 

헤드 테그 안으로 올려서 정보는 정보대로 코드를 넣어 실행하는 것이 좋다.그래서 defer을 사용한다.

// html 요소(Element) 	1개 검색/찾기
const boxEl = document.querySelector('.box');


// html 요소에 적용할 수 있는 메소드
boxEl.addEventListener();


// 인수(Arguments)를 추가 가능!
boxEl.addEventListener(1, 2);


// 1 - 이벤트(Event, 상황)
boxEl.addEventiListener('click', 2);

//// 1 - 이벤트(Event, 상황)
boxEl.addEventiListener('click', function () { 
console.log('click'); });



Element 요소 : 약어 El



// html 요소(Element) 	1개 검색/찾기
const boxEl = document.querySelector('.box');


// html 요소에 적용할 수 있는 메소드
boxEl.addEventListener();


// 인수(Arguments)를 추가 가능!
boxEl.addEventListener(1, 2);


// 1 - 이벤트(Event, 상황)
boxEl.addEventiListener('click', 2);

// 2 - 헨들러(Handler, 실행할 함수)
boxEl.addEventiListener('click', function () { 
console.log('click'); });







// html 요소(Element) 검색/찾기
const boxEl = document.querySelector('.box');

브라우저의 document라는 객체를 데이터가 있는데,[ 정의가되어있음.] 
querySelector라는 html요소를 검색하고 찾아주는 명령을 추가한 다음에, css 선택자를 선택해서. box라는 요소의 선택자(html)를 찾아서 찾아지면 반환이되어 반환이 되면 boxEl이라는  변수에 들어가더라!

// 요소의 클래스 정보 객체 활용!
boxElclassList.add('active');
let isContains = boxEl.classList.contains('active');
console.log(isContains);  // true
- boxEl 다음에 classList라는 객체 데이터를 사용할 수 있는데 [브라우저에 정의되어있음]
.add라는 메소드를 사용할 수 있다.
add라는 메소드의 요소를 추가하겠다.
.contains(포함이되어져있니?)라는 메소드를 사용해서 active가 있는지 체크해주는데 있으면 
console에 true가 뜨고, 없으면 false라고 뜬다.

 


boxEl.classList.remove('active');
isContains = boxEl.classList.contains('active');
console.log(isContains); // false

-.remove(삭제하겠다. 지우겠다라는 의미)





-



querySelectorAll 
- 클래스의 모든 데이터를 찾아서 반환하는 것.

// 찾은 요소들 반복해서 함수 실행!
// 익명 함수를 인수로 추가!
boxEls.forEach(function () {});
.forEach 

- 반복할수 있는 메소드

// 첫 번째 매개변수 (boxEl) : 	반복 중인 요소
// 두 번째 매개변수(index) : 반복 중인 번호

//출력!
boxEls.forEach(function (boxEl, index) {
	boxEl.classList.add('order-${index + 1}' );
});

boxEls. 라는 요소는 .forEach(메소드)를 통해서 반복으로 해당하는 내용을 돌려가면서 익명의 함수를 실행할 수 있고, 익명함수는 1번 실행 할 때 마다 boxEl와 index라는 매개변수로 내부에서 그 로직을 추가할 수있고,
결국 boxEl은 반복 중인 하나의 요소가 하나 들어 있고 그 요소에 classList를 통해서 어떤 클래스를 추가(.add)할 것인데 backtick('')기호를 추가를 할 것이고,그 내용은 order-${index = 1} [보간] 보간을 이용해서 index부분에 숫자 1를 더해서 클래스를 추가하겠다.



const  boxEls = doucument.querySelectorAll('.box');



boxEls.forEach(function( boxEl, index ) {

​	boxEl,classList.add(`order-${index}`);

console.log(index, boxEl ;
});

//forEach를 사용하려면 querySelectorAll를 통해서 여러개의 요소를 찾았을때, 

//매개변수는 아무 이름 가능 직관적인 이름이 좋음



const  boxEl = doucument.querySelector('.box');

// 재사용 가능하지 않은 변수를 사용하는 것이고, .box라는 클래스가진 제일 처음인 요소에
boxEl부분에 단수 형태인 변수에 할당한다.



##### //Getter, 값을 얻는 용도

console.log(boxEl.textContent); // Box!!

##### // console.log를 통해서 boxEl 요소에 textContent라는 속성을 적용해본다.

​    속성을 통해서 boxEl요소에 들어있는 내용이 반환되는데 텍스트로 반환이되는데 콘솔로그로 출력이 되는것.

##### // Setter, 값을 지정하는 용도

boxEl.textContent = 'HEROPY?!' ;

console.log(boxEl.textContent);  //HEROPY?!

##### // boxEl이라는 요소에 textContent라는 속성을 통해 HEROPY?! 라는 텍스트를 넣겠다고 선언.



const a = 'Hello~'

// split : 문자를 인수 기준으로 쪼개서 배열로 반환.

// reverse : 배열을 뒤집기.

// join : 배열을 인수 기준으로 문자로 병합해 반환.

const b  = a.split('').reverse().join('') ; // 메소드 체이닝...

 

console.log(a) ; // Hello~

console.log(b) ; // ~olleH





# 스타벅스 예제

- https://github.com/ParkYoungWoong/starbucks-vanilla-app

- ##### favicon.ico 아이콘을 사용하면,  브라우저 아이콘을 사용할 수 있다.

- link rel="icon" href="/favicon.png"

- **기본적인 CSS 브라우저 초기화 방법**

  link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/reset-css@5.0.1/reset.min.css"

  ## **seo 검색엔진**

  <meta property="og:type" content="website" />
  <meta property="og:site_name" content="Starbucks" />
  <meta property="og:title" content="Starbucks Coffee Korea" />
  <meta property="og:description" content="스타벅스는 세계에서 가장 큰 다국적 커피 전문점으로, 64개국에서 총 23,187개의 매점을 운영하고 있습니다." />
  <meta property="og:image" content="./images/starbucks_seo.jpg" />
  <meta property="og:url" content="https://starbucks.co.kr" />

  <meta property="twitter:card" content="summary" />
  <meta property="twitter:site" content="Starbucks" />
  <meta property="twitter:title" content="Starbucks Coffee Korea" />
  <meta property="twitter:description" content="스타벅스는 세계에서 가장 큰 다국적 커피 전문점으로, 64개국에서 총 23,187개의 매점을 운영하고 있습니다." />
  <meta property="twitter:image" content="./images/starbucks_seo.jpg" />
  <meta property="twitter:url" content="https://starbucks.co.kr" />

## **폰트 가져오는 방법**

- goole fonts < 검색
- link 방식은 병렬로 html쪽에서 외부에 있는 css를 가져오는 것
- import 방식은 직렬로 css파일에서 가져도오고. 또는 외부의 css파일로 가져옴.
- 링크를 html에 link방식을 넣었으면, css에 **CSS rules to specify families** 
  css속성을 가져와야됨. [ 예 ) font-family: 'Nanum Gothic', sans-serif; ]
- background-attachment: fixed;  // 뷰포트에 스크롤을 내릴때 이미지가 고정이 되는 것.
- background-size: cover;   // 배경의 더 넓은 너비에 이미지를 출력하게 되고,



## material icons (아이콘 가져오는 방법)

- 코드를 통해 icon을 삽입 할수 있음.

- goole material icons < 구글에 검색

- <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />
- https://fonts.google.com/icons

-  <span class="material-symbols-outlined" style="font-size:100px;">

    login

    </span>

  아이콘 사이즈도 키울소 있음. font-size를 통해서 (기본크기는 24px이다.)

- / 기호는(절대경로) index.html 메인페이지로 이동하겠다
- line-height: 1.4 / 글자의 줄 높이
- javascript:void(0) : 자바스크립트를 통해 ~한 기능을 동작 시킬것 인데, 할 것인다.지금은 없다.(void ) / 아무기능을 동작하지 않겠다라고 선언함.
  - 또는 # 
- 링크영역은 누를수 있게 더 영역을 지정해준다. 
  - padding을 사용하고, 인라인요소이기 때문에 display:block을 지정해준다.

header .sub-menu ul.menu li **::** 

- **::** 콜론 기호 2개는 가상의 요소 선택자이다.
- 내부의 앞쪽에 ~내용을 추가하는 것. content라는 요소로 정의 할 수 있음.

- li::before [인라인요소]
- position: absolute / fixed 를 사용하면 인라인요소에서 블록요소로 바뀐다.



header .main-menu .item .item__contents {

  width: 100%;

  position: fixed;

  left: 0;

}

- Top, bottom 속성을 사용하지 않아 수직 위치 값이 된다면, 요소의 원래 위치를 그래도 사용한다.

  만약 position:absolute.를 사용했다면,(위치상) 부모 요소를 기준으로 하므로 화면의 뷰포트 좌우 끝까지

  늘어날 수 없게 된다.



# Js용어

**Loads cdn : js를 외부에서 가져올 수있는 사이트**
**gsap cdn : libraries 사이트** 오픈소스 무료!

- setAttribute : set이라는 것은 무엇인가를 지정한다.htm속성을 Attribute라고 부른다.
  결국 어떤 htmll속성을 지정할때 사용하는 것

- searchInputEl.addEventListener('blur',function () {

  ​    searchEl.classList.remove('foucsed');

  ​    searchInputEl.setAttribute('placeholder', '');

  });

  - blur : 해제 된다라는 뜻

- window 라는 요소는 브라우저의 여러객체를 가지고 있음.

  - Window.addEventistener('scroll' , function () 

    ​	console.log('scroll!');

    })

  - window라는 객체라는 것은 결국에는 우리가 화면에 출력되고 있는 그 화면 자체를 의미하는 것이고, 그 화면 자체에다가 scroll 이벤트를 추가해서 그 화면이 scroll 되면 그 뒤쪽에 있는 익명의 함수( function () 

    ​	console.log('scroll!');) 를  실행하겠다라는 의미 

    - **scroll을 하면 수백개의 함수가 실행이 되는데 그러면 오류도 나고 안좋음, 그래서 _.throttle()를 추가해서** 

      **300(0.3초라는 의미) 라는 단위로 부하를 줘서 함수가 우르르 실행되는 것을 방지하는 용도로 _.throttle()라는**

       **lodash에서 제공하는 특정한 기능을 도입한 것.**

-  if (window.scrollY) 는 window라는 객체에서  scrollY부분의 속성이 그때 그때 마다 갱신이 된다는 것. 

  - Window.addEventistener('scroll' , function () 

    ​	console.log('scroll!'); = console.log(window.scrollY) 로 수정하면 콘솔화면이 스크롤을 할 때마다 몇 px지점에 위치하는지 확인 할수가 있다.

    console.log(window.scrollY > 500) 스크롤의 값이 500보다 크면 어떻게 할것이냐

    esle : 500보다 작으면 어떻게 할것이냐.(안보여진다)

- ​    badgeEl.style.display = 'none' : badgeEl라는 요소에 style이라는 전용속성에 display값을 어떻게 처리 할거냐?

​			안봉게 하겠다 none / 보이게 하겠다 block *참고용*

- **gsap.to();  : gsap에서 제공하는 애니메이션 처리 방법 중에 to라는 기능을 사용해서 애니메이션을 추가하는 것인데**

  **gsap.to(요소, 지속시간, 옵션);  gsap에서 애니메이션을 처리할 요소와 그 애니메이션이 지속되는 시간과 애니메이션을 실제로 어떻게 처리할지라는 옵션인 것**

- 옵션은 객체 데이터로 만들어 낼수 있음 그래서{ 중괄호를 사용할 수 있음}

  - Opacity 속성 처럼 값을 숫자로 입력하는 속성들은,  전환효과(transition 속성이나 gsap 라이브러리 등) 를 통해

    요소의 전/후 상태를 중간 숫자의 값으로 자연스럽게 만들어 줄수 있지만, display 속성 처럼 값이 숫자가 아닌 속성은

    전/후 상태의 중간값이 존재하지 않기 때문에, 자연스러운 전환효과를 사용할 수 없다.

- const promotionEl = document.querySelector('.promotion');

  const promotionToogleBtn = document.querySelector('.toggle-promotion');

  **let isHidePromotion = false;**

  promotionToogleBtn.addEventListener('click', function() {

    **isHidePromotion = !isHidePromotion**

  **!를 앞에 붙이면 반대가 되게 만들어주세요 라는 뜻.**  특정 변수의 값을 지속적으로 반대값으로 전환시켜줄수있는 값 
  if (isHidePromotion) {

  ​    

    } else {

  ​    

    }

  조건문을 추가해서  !isHidePromotion값이 실행이 안되면 else(조건문) 의 내용을 실행하겠습니다 라는 것



# BEM용어

BEM : HTML 클래스 속성의 작명법

- 요소__일부분 : Underscore(Lodash) 기호로 요소의 일부분을 표시
- 요소--상태 : Hyphen(Dash) 기호로 요소으 상태를 표시



##### Position:absolute / fixed 는 가로 넓이가 최소환으로 넓어지려고 함.



**flex-grow**: 최대한의 너비를 쓸수 있도록 늘어나라.



# **유튜브 영상배경 (youtube iframe API )**

padding-top : 56.25%; 를 넣으면 16:9 비율의 너비가 된다.

가상요소선택자

- 스타일을 위해서만 활용하는 것이면  css에서 사용하는 것이 좋다.

  .youtube .youtube__area**::before**  

https://developers.google.cn/youtube/iframe_api_reference?hl=ko

유튜브 영상 삽입 방법 (youtube iframe api)

## youtube.js

- // 2. This code loads the IFrame Player API code asynchronously.

​	var tag = document.createElement('script');



​	tag.src = "https://www.youtube.com/iframe_api";

​	var firstScriptTag = document.getElementsByTagName('script')[0];

​	firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);



​	// 3. This function creates an <iframe> (and YouTube player)

​	//   after the API code downloads.

​	function onYouTubeIframeAPIReady() {

​	 // <div id="player"></div>

​	 new YT.Player('player', {

​	  videoId: 'M7lc1UVf-VE',

​	  events: {

​	   'onReady': onPlayerReady,

​	   'onStateChange': onPlayerStateChange

​	  }

​	 });

​	}

# CSS용어

- ::before 라는 요소는 content라는 요소가 필요함

- img 요소가 display:block + margin :0 auto 인 경우 width 속성이 없이도 가운데 정렬이 가능합니다.
  우리는 현재 프로젝트에서 img 요소에 display:block 을 지정했습니다.









# github사용방법

### 버전관리

- 깃 (사용자  로컬) 

**#개행 문자 (Newline) 설정**

**##macOS**

- git config --global core.autocrlf input

#####  ##windows

- git config --global core.autocrlf true

**#사용자 정보**

##### 커밋(버전생성)을 위한 정보 등록

- git config --global user.name 'YOUR_NAME'
- git config --global user.nemail 'YOUR_MAEIL'

##### #구성확인

##### **Q키를 눌러서 종료!**

- git config --global --list



**#현재 프로젝트에서 변경사항 추적(버전 관리)을 시작.**

- git init

**#변경사항을 추적할 특정 파일(index.html)을 지정**

- git add index.html

**#모든 파일의 변경사항을 추적하도록 지정.**

- git add .

**#메세지(-m)와 함께 버전을 생성**

- git commit -m '프로젝트 생성'

**#origin이란 별칭으로 원격 저장소를 연결**

- git remote add origin https://github.c.....주소

**#origin이란 별칭의 원격 저장소로 버전 내역 전송.**

- git push origin master





# 버전 업로드

**git status**

**git add .** 
**git status**

**git commit -m '수정 내용'**



**git log (확인하기)**

REDME.md 



git push origin master (깃헙에 저장소에 보내기)



# 로그인 브렌치(branch)

- **git checkout master / signin** 



### 로그인 페이지 개발

- common.js (공통적으로 사용된 js)



# 프로젝트 복제

터미널에서 dir 작성.

cd desk + tab  누르고 엔터

그러면 데스크탑에 적용됨

dir을 다시 친다.

cd .. 작성하면 데스크탑의 바깥쪽 폴더로 나가짐.

git clone https://github.com/ycl411/starbucks.git (복사한 주소) 엔터

dir 엔터

터미널에서 여는 방법

- 컨트롤 쉬프트 p (모든명령실행)
- code 명령 설치 (shell command: install 'code' command in path)Part 3. JavaScript Essentials
- path에 code 설치 목록이 없으면 설치.

cd starbucks

code .

code . -r (현재 창에서 열어주는 것)





# **Part 3. JavaScript Essentials**

### node.js

> LTS는 장기적으로 안정되고 신뢰도가 높은 지원이 보장되는 버전 , 유지/보수(서버 운영 등) 에 초점을 맞춰 대부분 사용자에게 추천되는 버전

> [nvm node.js 설치 ](https://github.com/coreybutler/nvm-windows/releases)
>
> 1. download를 찾아서 nvm-setup.zip을 다운설치 하면됨.
> 2. vscode 터미널에서 nvm --version 이라고 쳐서 오류 안뜨면 설치완료.



### npm 개요

> 1. 폴더생성 -> 터미널에서  npm - init -y  ->package.json 이 뜰것임.
>
> 2. npm install parcel-bundler -D 설치.
> 3.  node_modules 폴더 / package.-lock.json이 생성된다.
> 4. npm install lodash 설치
> 5. node_modules 를  설치할 때 npm i 라고 쳐도 된다.



### parcel-bundler

> package.js에 scripts 밑에 test ~라고 되어있는데 삭제하고
>
> "dev" :"parcel index.html" 이라고 적어준다.
>
> 개발용 의존용 패키지로  우리 내부에 프로젝트에만 적용된 것이기 때문에
>
> 우리 프로젝트의 scripts에 옵션에 명령을 적어주면, 우리 프로젝트의 내부에서만 동작하는 것으로 인식 시켜주는 것이고 대신에 그 명령어를 dev명령어로 실행 해주는 것.
>
> ***우리 환경에 개발서버를 열겠다 라는 명령어***
>
> npm run dev 명령어를 터미널에 적어준다.



### dist (실제 웹사이트가 동작한다.)

"build":"parcel build index.html 

번들(bundle) 은 우리가 프로젝트 개발에 사용한 여러 모듈(패키지)을 하나로 묶어내는 작업을 말합니다.



### lodash

> import _ from 'lodash'; 명령어는
>
> _ 안에 lodash라는 js를 사용하겠다 라는 것이다.
>
> console.log('hello world');
>
> console.log(_.camelCase('hello world'));
>
> ***즉, _(lodash)안에 있는 js파일 중 .camelCase(메소드)라는  js파일을  'hello world' 문자데이터를 넣어주면***
>
> ***hello world라는 문자가 camelCase라는 방식으로 변경이 되서 반환이 되서 콘솔에 출력하는 것.***
>
> 



### 유익적 버전(Major.Minor.Patch)

> 12.14.1 (16.15.1)
>
> Major : 12 [기존 버전과 호환되지 않는 새로운 버전] 
>
> Minor : 14 [기존 버전과 호환되는 새로운 기능이 추가된 버전]
>
> Patch : 1 [기존 버전과 호환되는 버그 및 오타 등이 수정된 버전]
>
> *맨 앞에 ^ 이 있으면 Major 버전안에서 가장 최신 버전으로 업데이트 가능 이라는 것.*
>
> 
>
> npm info lodash 버전 확인하는 방법.
>
> npm install lodash@다운 버전 
>
> npm update lodash 업그레이드 버전
> ^ 기호를 지우면 버전을 업그레이드 안됨.



### npm 주의사항

> .gitignore 파일을 만들고
> .cache/
> dist/
>
> node_modules/ 
>
> 명령어를 입력하고 저장한 다음
>
> 터미널에 git init 라고 치면 3개의 명령어는 어둡게 변해서 버전관리가 따로 되지 않는다.
>
> 
> 
