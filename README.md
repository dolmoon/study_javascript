# 자바스크립트 스터디
## 0. 자바스크립트 입문하기
### 0.1. 마크다운(Markdown) 문법 익히기
마크다운 언어는 '.md' 파일로 깃허브(GitHub) 등에서 프로젝트나 소스코드를 설명하는 문서로 많이 사용된다.
간단한 문법만으로 깔끔하게 문서를 작성할 수 있다.
#### 0.1.1. 제목(Heading)
제목에는 `#`을 사용한다. 줄의 맨 앞에 `#`을 먼저 쓰고 뒤에 제목을 입력하면, HTML의 `<h1>`에 해당하는 제목으로 화면에 표시된다. `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`에 해당하는 제목에는 각각 `##`, `###`, `####`, `#####`, `######`을 사용한다.
  # Heading1 --> `# Heading1`
  ## Heading2 --> `## Heading2`
  ### Heading3 --> `### Heading3`
  #### Heading4 --> `#### Heading4`
  ##### Heading5 --> `##### Heading5`
  ###### Heading6 --> `###### Heading6`
#### 0.1.2. 구분선(Line)
내용을 구분하기 위해 가로선을 넣고 싶을 경우에는 줄의 맨 앞에 `---`를 쓴다.

  ---
  
#### 0.1.3. 글자체 (Text attributes)
글자체는 **볼드체**와 *이탤릭체*, ~~취소선~~을 지원한다. 각각 `**볼드체**`, `*이탤릭체*`, `~~취소선~~`과 같이 사용하면 된다.
#### 0.1.4. 인용문 (Quote)
인용문을 표기하기 위해서는 줄의 맨 앞에 `>`을 먼저 쓰고 뒤에 인용문의 내용을 입력한다.
  > 우리는 빛이 없는 어둠 속에서도...

#### 0.1.5. 목록 (List)
목록을 표기하기 위해서는 목록을 구성하는 각 항목의 앞에 `* ` 또는 `- `를 입력한다. 이 때, `*` 또는 `-`과 뒤에 오는 항목 명칭 사이에 공백이 있어야 목록으로 표시되는 점에 유의한다.

  * bullet item1 --> `*bullet item1`
  * bullet item2 --> `*bullet item2`
  * bullet item3 --> `*bullet item3`
  
  - another bullet item1 --> `- another bullet item1`
  - another bullet item2 --> `- another bullet item2`
  - another bullet item3 --> `- another bullet item3`

숫자형 목록을 표기하기 위해서는 각 항목의 앞에 '1.', '2.', '3.'과 같이 숫자와 점을 쓴다.
  1. first item
  2. second item
  3. third item

#### 0.1.6. 링크(Link)
하이퍼링크를 추가하려면 `[링크 섦명](URL)`과 같이 입력한다.

  Click [here](http://academy.dream-coding.com/) --> `Click [here](http://academy.dream-coding.com/)`

#### 0.1.7. 이미지(Image)
이미지를 추가하려면 `![이미지 설명](URL)`과 같이 입력한다.

  ![image description](https://user-images.githubusercontent.com/61736137/102153953-b2881000-3ebb-11eb-9581-7026bc8e169e.jpg) --> `![image description](https://user-images.githubusercontent.com/61736137/102153953-b2881000-3ebb-11eb-9581-7026bc8e169e.jpg)`

#### 0.1.8. 테이블(Table)
테이블을 추가하려면 다음의 예와 같이 헤더와 구분줄, 셀 내용을 입력한다.

|Header Column1|Header Column2|
|--|--|
|Cell11|Cell12|
|Cell21|Cell22|

#### 0.1.9. 코드(Code)
코드를 따로 표시하고자 할 경우에는 인라인 코드를 표시하는 방법과 여러 줄을 코드로 표시하는 두 가지 방법이 있다. 인라인 코드는 <code>`console.log('your message')`</code>와 같이 백틱("`")으로 코드를 감싸면 된다. 여러 줄을 코드로 표시하려면 백틱을 세 번 연속으로 
