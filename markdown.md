# Markdown Cheetsheet
## Heading (제목)
* 행의 가장 앞에 존재하는 '#'의 개수에 따라 제목의 수준(1~6)이 결정  

* 수준에 따라 폰트의 크기가 결정됨  

* 예시  

    * 예시 코드  

        ```
        # level1
        ## level2
        ### level3
        #### level4
        ##### level5
        ###### level6
        ```
    * 출력 결과  

        # level1
        ## level2
        ### level3
        #### level4
        ##### level5
        ###### level6
* 수준 1 제목은 행 직후 '='으로만 구성된 행을 추가하는 방식으로 대체 가능  

    * 예시 코드  

        ```
        level1
        ===
        ```
    * 출력 결과  

        level1
        ===
* 수준2 제목은 행 직후 '-'으로만 구성된 행을 추가하는 방식으로 대체 가능  
    * 예시 코드  

        ```
            level2
            ---
        ```
    * 출력 결과  

        level2
        ---
## Paragraphs (단락)

* 단락을 구분하기 위해 **공백 없는** 빈 행을 삽입  

* 목록 내부에서도 예외 없이 공백 없이 빈 행을 작성해야 함  

## Line Breaks (개행)

* 해당 행 끝에 2개 이상의 공백을 삽입한 뒤 enter(return) 입력  

## Emphasis (강조)

* 강조 표시를 원하는 구역의 시작, 끝에 '*' 또는 '_'를 1~3개 삽입

    * *Italic*: '*' 또는 '_'를 **1**개 사용

    * **Bold**: '*' 또는 '_'를 **2**개 사용

    * ***Italic & Bold***: '*' 또는 '_'를 **3**개 사용

    * 예시  
        | 예시 코드 | 출력 결과 |  
        | --- | --- |  
        | `I just love *italic text*.` | I just love *italic text*. |  
        | `I just love __bold text__.` |  I just love __bold text__. |  
        | `I just love ***italic and bold text***.` | I just love ***italic and bold text***. |  
* '*'과 '_' 교차 사용은 불가능
    * 잘못된 예시  
        ```
        I just love *italic text_.
        ```
* '_'는 단어 중간 (이전, 이후 문자와 공백으로 구분되지 않을 때)에는 사용 불가능
    * 잘못된 예시  
        ```
        Love_is_bold
        ```
