# AccordionMenu

HTML과 CSS만을 이용해 아코디언 메뉴를 만들어 보았습니다.

![AccordionMenu](https://user-images.githubusercontent.com/61913417/106174050-f7e86e80-61d7-11eb-9b97-23c9edc5df9d.gif)

#### 구상 과정과 구현
1. 질문 클릭 시 답변이 나오게 하고 싶다!
	- input과 label을 묶어서 선택되는 항목을 지정하였습니다.
    - 답변 공간의 높이를 0을 줬다가 input이 선택 되면 150px을 주도록 설정하여 안나타있는 것 처럼 보이다가 나타나게 만들어 주었습니다.
    - 자연스럽게 하기 위해 transition 속성도 추가해 줬습니다.
      
2. 다음 질문을 클릭하면 전 질문 답변은 닫히게 하고 싶다!
	- input type에 checkbox와 radio 두개를 사용할 수 있었는데 checkbox는 여러개가 선택 가능하므로 두개 이상의 질문의 답변이 나타날 수 있는데 비해 radio는 한개만 선택된다는 속성 때문에 한개의 질문의 답변만 나타날 수 있으므로 radio를 사용하였습니다.
    여러개의 답변창이 나오게 하고 싶으면 input type에 checkbox를 사용하시면 됩니다.
      
3. 화살표 아이콘이 답변 생성시 위를 가리키도록 하고 싶다!
	- 질문이 선택 됐을 때 transform: rotate(180deg); 로 180도 회전 시켜줘서 위를 가리키도록 만들었습니다.
---  
#### 공부
_속성 선택자_
- [attributename="value"] : attributename 속성의 값이 value인 요소를 선택합니다. 속성값이 정확히 일치해야 합니다.  
- [attributename|="value"] : attributename 속성의 값이 value이거나 value-로 시작하는 요소를 선택합니다.  
- [attributename~="value"] : attributename 속성의 값이 value를 포함한 요소를 선택합니다. 포함 여부는 **단어** 기준으로 판다합니다.  
-	[attributename*="value"] : attributename 속성의 값이 value를 포함한 요소를 선택합니다. 포함 여부는 **문자열** 기준으로 판단합니다.  
- [attributename^="value"] : attributename 속성의 값이 value로 시작하는 요소를 선택합니다. 포함 여부는 **문자열** 기준으로 판단합니다.  
- [attributename$="value"] : attributename 속성의 값이 value로 끝나는 요소를 선택합니다. 포함 여부는 **문자열** 기준으로 판단합니다.  
