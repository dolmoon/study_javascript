# Markdown 소개
## 1. 마크다운(Markdown) 문법 익히기
마크다운 언어는 '.md' 파일로 깃허브(GitHub) 등에서 프로젝트나 소스코드를 설명하는 문서로 많이 사용된다.
간단한 문법만으로 깔끔한 문서를 작성할 수 있다.


### 1.1. 제목(Header)
제목 줄에는 `#`을 사용한다. 줄의 맨 앞에 `#`을 먼저 쓰고 뒤에 제목을 입력하면, HTML의 `<h1>`에 해당하는 제목으로 화면에 표시된다. `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`에 해당하는 제목에는 각각 `##`, `###`, `####`, `#####`, `######`을 사용한다.

|표기법|결과|비고|
|:--:|:--|:--|
|`# Header1`|<h1>Header1</h1>|GitHub에서 글자의 아래에 자동으로 구분선이 추가됨.|
|`## Heading2`|<h2>Header2</h2>|GitHub에서 글자의 아래에 자동으로 구분선이 추가됨.|
|`### Heading3`|<h3>Header3</h3>||
|`#### Heading`|<h4>Heading4</h4>||
|`##### Heading5`|<h5>Heading5</h5>||
|`###### Heading6`|<h6>Heading6</h6>|GitHub에서 글자의 색상이 다른 Heading에 비해 연하게 표시됨|

---
### 1.2. 구분선(Line)
내용을 구분하기 위해 가로선을 넣고 싶을 경우에는 줄의 맨 앞에 `-`, `*` 또는 `=`를 연속해서 쓴다. (한 라인에 공백을 제외한 다른 문자가 포함되지 않은 상태에서 3개 이상이면 됨)
   #### 표기법 1
   ```
   가나다라
   ===  --> GitHub에서는 1레벨 Header(`#`)와 동일한 효과로 나타남
   ```
   #### 결과 1
   가나다라
   ====

   #### 표기법 2
   ```
   가나다라
   --- --> GitHub에서는 2레벨 Header(`##`)와 동일한 효과로 나타남
   ```
   #### 결과 2
   가나다라
   ---

   #### 표기법 3
   ```
   가나다라
   ***
   ```
   #### 결과 3
   가나다라
   ***

   #### 표기법 4
   ```
   가나다라
   - - -
   ```
   #### 결과 4
   가나다라
   - - -

---
### 1.3. 글자체 (Text attributes)
글자체는 **볼드체**와 *이탤릭체*, ~~취소선~~을 지원한다. 각각 `**볼드체**`(또는 `__볼드체__`), `*이탤릭체*` (또는 `_이탤릭체_`), `~~취소선~~`과 같이 사용하면 된다.
이 효과를 방지하려면 `\*` 또는 `\_`와 같이 `\`를 앞에 붙인다. **볼드체** (`\*\*볼드체\*\*`), *이탤릭체* (`\*이탤릭체\*`), ~~취소선~~ (`\~\~취소선\~\~`) 

---
### 1.4. 문단(paragraphs)과 줄 바꿈(line breaks) 
문단을 나누는 방법은 문장 사이에 한 줄 이상의 공백 라인(스페이스나 탭과 같은 white space로 이루어진 줄)을 포함시킨다.
```
첫 번째 문단의 첫 번째 문장입니다.
첫 번째 문단의 두 번째 문장입니다.

두 번째 문단의 첫 번째 문장입니다.
두 번째 문단의 두 번째 문장입니다.
```
줄 바꿈을 위해서는 줄의 끝에 두 개의 공백 문자를 사용하거나 `\`를 사용한다.  
문법: 줄 바꿈은 여기에서 `  `<end of line>이루어진다.  
결과: 줄 바꿈은 여기에서  
   이루어진다.

---
### 1.4. 인용문 (BlockQuotes)
인용문을 표기하기 위해서는 줄의 맨 앞에 `>`을 먼저 쓰고 뒤에 인용문의 내용을 입력한다. 인용문 내에서 다시 인용문을 표시하고자 할 때는 `>>`와 같이 중복해서 사용한다.
> 우리는 빛이 없는 어둠 속에서도...
>> 내재된 인용문은 `>`를 연속해서 사용한다.
>> 
> 기나긴 세월을 기다리어... 

인용문은 Header나 리스트, 코드 블럭과 같은 다른 요소를 포함할 수 있다. 
> #### 인용문 안의 Header
> |컬럼1|컬럼2|컬럼3|
> |:--:|:--|:--|
> |Cell11|Cell12|Cell13|
> |Cell21|Cell22|Cell23|
>

---
### 1.5. 목록 (List)
목록을 표기하기 위해서는 목록을 구성하는 각 항목의 앞에 `* `, `+ ` 또는 `- `를 입력한다. 이 때, `*`, `+` 또는 `-`과 뒤에 오는 항목 명칭 사이에 공백이 있어야 목록으로 표시되는 점에 유의한다.

#### 표기법
   ```
* bullet item1<br>
* bullet item2<br>
* bullet item3<br>
    * sub bullet item1 --> (네 칸 공백 이후에)* sub-bullet item1
   ```
   
#### 결과
* bullet item1
* bullet item2
* bullet item3
    * sub-bullet item1

숫자형 목록을 표기하기 위해서는 각 항목 번호는 '1. ', '2. ', '3. '과 같이 숫자와 점을 쓰고 공백을 하나 추가한 후에 항목의 내용을 입력한다. 첫 번째 항목의 번호가 '3. '으로 시작하면 나머지 번호는 '4. ', '5. '과 같이 자동으로 수정된다. 예를 들어, '3. first item', '7. second item', '6. third item'으로 되어 있더라도 Markdown이 해독할 때 번호를 순서대로 재 조정하여 자동으로 '3. ', '4. ', '5. '로 바꾼다.

#### 표기법
```
1. first item
   > nested blockquote in list item
2. second item
      
      In the original Markdown a code block in a list needs to be indented twice(8 spaces or two tabs).
      ```
      console.log("message");
      ```
3. third item
```

#### 결과
1. first item
   > nested blockquote in list item
2. second item
      
      In the original Markdown a code block in a list needs to be indented twice(8 spaces or two tabs).
      ```
      console.log("message");
      ```
3. third item


---
### 1.6. 링크(Link)
하이퍼링크를 추가하려면 `[링크 설명](URL)`과 같이 입력한다.

|문법|결과|비고|
|--|--|--|
|`Click [Markdown 설명 동영상(드림코딩 by 엘리)](https://www.youtube.com/watch?v=kMEb_BzyUqk)`|Click [Markdown 설명 동영상(드림코딩 by 엘리)](https://www.youtube.com/watch?v=kMEb_BzyUqk)||
|`Click [GitHub Markdown](https://guides.github.com/features/mastering-markdown/)`|Click [GitHub Markdown](https://guides.github.com/features/mastering-markdown/)||

---
### 1.7. 이미지(Image)
이미지를 추가하려면 `![이미지 설명](URL)`과 같이 입력한다.

|문법|결과|
|--|--|
|`![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)`|![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)|
|Markdown에서 이미지의 크기는 조정이 안되므로 HTML의 'image' 태그를 이용하는 것도 방법이다.|<img src = 'https://octodex.github.com/images/yaktocat.png' title = 'Image of Yaktocat' width = '200'></img>| 

---
### 1.8. 테이블(Table)
테이블을 추가하려면 다음의 예와 같이 헤더와 구분줄, 셀 내용을 입력한다.

#### 표기법
```
|Header Column1|Header Column2|Header Column3|
|:--|--:|:--:|  --> 컬럼에 대해 정렬 방식을 지정할 수 있다. (각 컬럼별로 '좌측 정렬', '우측 정렬', '가운데 정렬' 지정)
|Cell11|Cell12|Cell13|
|Cell21|Cell22|Cell23|
```

#### 결과
|Header Column1|Header Column2|Header Column3|
|:--|--:|:--:|
|Cell11|Cell12|Cell13|
|Cell21|Cell22|Cell23|

----
### 1.9. 코드(Code)
코드를 따로 표시하고자 할 경우에는 인라인 코드를 표시하는 방법과 여러 줄을 코드로 표시하는 두 가지 방법이 있다.
  * 인라인 코드는 백틱(\`)으로 코드를 감싸면 된다.

      * 이 줄에는 인라인 코드로 표시되는 코드인, `` `console.log('your message')` ``이 포함되어 있습니다.
    
  * 멀티라인 코드는 다음과 같이 시작 줄과 끝 줄에서 백틱을 세 번 연속으로 사용하면 된다.

  ````javascript
  ```
  console.log('message1');
  console.log('message2');
  console.log('message3');
  ```
  ````
 
다음과 같이 멀티라인 코드 시작 줄에 프로그램 언어 명칭을 같이 적어주면, 해당 언어의 문법을 강조해 표시해준다. 각 줄의 맨 앞에 네 개의 공백을 넣어 주면 들여쓰기(indent)하여 표시한다.

#### 표기법
````
```javascript
if (isAwesome){
return true; --> 들여쓰기 표시를 위해 줄의 맨 앞에 네 개의 공백을 넣음.
}
```
````

#### 결과
```javascript
if (isAwesome){
    return true;
}
```
