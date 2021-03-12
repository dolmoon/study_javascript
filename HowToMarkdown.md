# 자바스크립트 스터디
## 0. 자바스크립트 입문하기
### 0.1. 마크다운(Markdown) 문법 익히기
마크다운 언어는 '.md' 파일로 깃허브(GitHub) 등에서 프로젝트나 소스코드를 설명하는 문서로 많이 사용된다.
간단한 문법만으로 깔끔하게 문서를 작성할 수 있다.


#### 0.1.1. 제목(Heading)
제목에는 `#`을 사용한다. 줄의 맨 앞에 `#`을 먼저 쓰고 뒤에 제목을 입력하면, HTML의 `<h1>`에 해당하는 제목으로 화면에 표시된다. `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`에 해당하는 제목에는 각각 `##`, `###`, `####`, `#####`, `######`을 사용한다.

|문법|결과|비고|
|:--:|:--|:--|
|`# Heading1`|<h1>Heading1</h1>|GitHub에서 글자의 아래에 자동으로 구분선이 추가됨.|
|`## Heading2`|<h2>Heading2</h2>|GitHub에서 글자의 아래에 자동으로 구분선이 추가됨.|
|`### Heading3`|<h3>Heading3</h3>||
|`#### Heading`|<h4>Heading4</h4>||
|`##### Heading5`|<h5>Heading5</h5>||
|`###### Heading6`|<h6>Heading6</h6>|GitHub에서 글자의 색상이 다른 Heading에 비해 연하게 표시됨|

---
#### 0.1.2. 구분선(Line)
내용을 구분하기 위해 가로선을 넣고 싶을 경우에는 줄의 맨 앞에 `---`를 쓴다.

    ---

---
#### 0.1.3. 글자체 (Text attributes)
글자체는 **볼드체**와 *이탤릭체*, ~~취소선~~을 지원한다. 각각 `**볼드체**`, `*이탤릭체*`, `~~취소선~~`과 같이 사용하면 된다.

---
#### 0.1.4. 인용문 (Quote)
인용문을 표기하기 위해서는 줄의 맨 앞에 `>`을 먼저 쓰고 뒤에 인용문의 내용을 입력한다.
    > 우리는 빛이 없는 어둠 속에서도...

---
#### 0.1.5. 목록 (List)
목록을 표기하기 위해서는 목록을 구성하는 각 항목의 앞에 `* ` 또는 `- `를 입력한다. 이 때, `*` 또는 `-`과 뒤에 오는 항목 명칭 사이에 공백이 있어야 목록으로 표시되는 점에 유의한다.

  * bullet item1 --> `*bullet item1`
  * bullet item2 --> `*bullet item2`
  * bullet item3 --> `*bullet item3`
      * sub-bullet item1 --> `(네 칸 공백 이후에)* sub-bullet item1`
  
  - another bullet item1 --> `- another bullet item1`
  - another bullet item2 --> `- another bullet item2`
  - another bullet item3 --> `- another bullet item3`
      - sub another bullet item1 --> `(네 칸 공백 이후에)- sub-bullet item1`

숫자형 목록을 표기하기 위해서는 각 항목의 앞에 '1.', '2.', '3.'과 같이 숫자와 점을 쓴다.
  1. first item
  2. second item
  3. third item

#### 0.1.6. 링크(Link)
하이퍼링크를 추가하려면 `[링크 설명](URL)`과 같이 입력한다.

  `Click [Markdown 설명 동영상(드림코딩 by 엘리)](https://www.youtube.com/watch?v=kMEb_BzyUqk)` --> Click [Markdown 설명 동영상(드림코딩 by 엘리)](https://www.youtube.com/watch?v=kMEb_BzyUqk)
  
  `Click [GitHub Markdown](https://guides.github.com/features/mastering-markdown/)` --> Click [GitHub Markdown](https://guides.github.com/features/mastering-markdown/)

#### 0.1.7. 이미지(Image)
이미지를 추가하려면 `![이미지 설명](URL)`과 같이 입력한다.

    `![image description](https://user-images.githubusercontent.com/61736137/102153953-b2881000-3ebb-11eb-9581-7026bc8e169e.jpg)`
    
    ![image description](https://user-images.githubusercontent.com/61736137/102153953-b2881000-3ebb-11eb-9581-7026bc8e169e.jpg)

#### 0.1.8. 테이블(Table)
테이블을 추가하려면 다음의 예와 같이 헤더와 구분줄, 셀 내용을 입력한다.

    |Header Column1|Header Column2|Header Column3|
    |:--|--:|:--:|
    |Cell11|Cell12|Cell13|
    |Cell21|Cell22|Cell23|



#### 0.1.9. 코드(Code)
코드를 따로 표시하고자 할 경우에는 인라인 코드를 표시하는 방법과 여러 줄을 코드로 표시하는 두 가지 방법이 있다.
  * 인라인 코드는 백틱(\`)으로 코드를 감싸면 된다.

    `` `console.log('your message')` ``
    
  * 멀티라인 코드는 다음과 같이 시작 줄과 끝 줄에서 백틱을 세 번 연속으로 사용하면 된다.

    ````
    ```
    console.log('message1');
    console.log('message2');
    console.log('message3');
    ```
    ````
 
다음과 같이 멀티라인 코드 시작 줄에 프로그램 언어 명칭을 같이 적어주면, 해당 언어의 문법을 강조해 표시해준다. 지원되는 

    ```javascript
    if (isAwesome){
        return true
    }
    ```
