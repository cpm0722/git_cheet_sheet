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
## Blockquotes (인용)

* blockquotes로 만들고 싶은 단락의 가장 앞에 '>'를 추가  

    * 예시 코드  

        ```
        > Dorothy followed her through many of the beautiful rooms in her castle.
        ```

    * 출력 결과  

        > Dorothy followed her through many of the beautiful rooms in her castle.  

* 여러 단락을 blockquotes로 만들고 싶은 경우 여러 단락 사이의 공백 행까지 포함해 모든 단락의 가장 앞에 '>'를 추가  

    * 예시 코드  

        ```
        > Dorothy followed her through many of the beautiful rooms in her castle.  
        >
        > The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.  
        ```

    * 출력 결과  

        > Dorothy followed her through many of the beautiful rooms in her castle.  
        >
        > The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.  

* '>'를 다수 사용해 blockquotes를 중첩으로 사용 가능

    * 예시 코드  

        ```
        > Dorothy followed her through many of the beautiful rooms in her castle.  
        >> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.  
        ```

    * 출력 결과  

        > Dorothy followed her through many of the beautiful rooms in her castle.  
        >> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.  

* blockquotes 내부에 heading, list 등의 다른 markdown 속성을 사용 가능

    * 예시 코드  

        ```
        > ### The quarterly results look great!  
        >
        > - Revenue was off the chart.
        ```

    * 출력 결과  

        > ### The quarterly results look great!  
        >
        > - Revenue was off the chart.

## Lists (목록)

### Ordered Lists (순서 있는 목록)

* 행의 가장 앞에 "숫자."를 추가

    * 예시 코드  

        ```
        1. First item  
        2. Second item  
        3. Third item  
            1. Indented Item  
            1. Indented Item  
        4. Fourth item  
        ```

    * 출력 결과  

        1. First item  
        2. Second item  
        3. Third item  
            1. Indented Item  
            1. Indented Item  
        4. Fourth item  

* 이전에 같은 수준에서 순서 있는 목록을 사용한 경우 현재 입력한 숫자와 관계 없이 이전에 사용한 숫자 + 1이 됨  

    * 예시 코드  

        ```
        1. First item  
        9. Second item  
        9. Third item  
        9. Fourth item  
        ```

    * 출력 결과  

        1. First item  
        9. Second item  
        9. Third item  
        9. Fourth item  

### Unordered Lists (순서 없는 목록)

* 행의 가장 앞에 '-', '*', '+' 중 하나를 추가

    * 예시 코드  

        ```
        - First item  
        - Second item  
        - Third item  
            - Indented item  
            - Indented item  
        - Fourth item  
        ```

    * 출력 결과  

        - First item  
        - Second item  
        - Third item  
            - Indented item  
            - Indented item  
        - Fourth item  

* 같은 목록 내에서 '-', '*', '+' 교차 사용은 권장하지 않음

    * 잘못된 예시 

        ```
        - First item  
        * Second item  
        + Third item  
        - Fourth item  
        ```

### Adding Elements in Lists (목록 내 요소 추가)

* 목록 내에 다른 요소(목록, Blockquotes, 이미지, 일반 텍스트 등)을 추가하고 싶은 경우 tab 또는 4개의 space를 사용해 indent를 한 단계 추가한 후 사용

    * 예시 코드  

        ```
        * This is first list item.
            1. This is first-first list item.
            2. This is first-second list item.
        * Here's the second list item.
            > A blockquote would look great below the second list item.  
        * And here's the third list item.
        ```

    * 출력 결과  

        * This is first list item.
            1. This is first-first list item.
            2. This is first-second list item.
        * Here's the second list item.
            > A blockquote would look great below the second list item.  
        * And here's the third list item.

* code block을 list 내부에 추가하고 싶은 경우 tab 2개 또는 8개의 space를 사용해 indent해야 함  

    * 예시 코드  

        ```
        1.  Open the file.
        2.  Find the following code block on line 21:

                <html>
                <head>
                    <title>Test</title>
                </head>

        3.  Update the title to match the name of your website.
        ```

    * 출력 결과

        1.  Open the file.
        2.  Find the following code block on line 21:

                <html>
                <head>
                    <title>Test</title>
                </head>

        3.  Update the title to match the name of your website.

