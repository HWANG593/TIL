# 마크다운(Markdown)

> 일반 텍스트 형식 구문을 사용하는 마크업 언어의 일종으로 사용법이 쉽고 간결하여 빠르게 문서 정리를 할 수 있습니다. 단, 모든 HTML 마크업을 대체하지는 않습니다.

## 1. 문법

### 1.1 Header

> 헤더는 제목을 표현할 때 사용합니다. 단순히 글자의 크기를 표현하는 것이 아닌 의미론적인 중요도를 나타냅니다.

* `<h1>` 부터`<h6>` 까지 표현 가능합니다.
* `#` 의 개수로 표현하거나 `<h1></h1>` 의 형태로 표현 가능합니다.



# h1 태그입니다.

## h2 태그입니다.

### h3 태그입니다.

#### h4 태그입니다.

##### h5 태그입니다.

###### h6 태그입니다.



### 1.2 List

> 목록을 나열할 때 사용합니다. 순서가 필요한 항목과 그렇지 않은 항목으로 구분할 수 있습니다. 순서가 있는 항목 아래 순서가 없는 항목을 지정할 수 있으며 그 반대도 가능합니다.

* 순서가 없는 목록
  * `1.` 을 누르고 스페이스바를 누르면 생성할 수 있습니다.
  * `tab` 키를 눌러서 하위 항목을 생성할 수 있고 `shift + tab` 키를 눌러서 상위 항목으로 이동 할 수 있습니다.
* 순서가 있는 목록
  * `-` (하이픈)을 쓰고 스페이스바를 누르면 생성할 수 있습니다.
  * `tab` 키를 눌러서 하위 항목을 생성할 수 있고 `shift + tab` 키를 눌러서 상위 항목으로 이동 할 수 있습니다.

1. 순서가 있는 항목
2. 순서가 있는 항목
   1. 순서가 있는 하위 항목
   2. 순서가 있는 하위 항목

* 순서가 없는 항목
* 순서가 없는 항목
  * 순서가 없는 하위 항목
  * 순서가 없는 하위 항목



### 1.3 Code Block

> 코드 블럭은 작성한 코드를 정리하거나 강조하고 싶은 부분을 나타낼 때 사용합니다. 인라인과 블럭 단위로 구분할 수 있습니다.



* Inline
  * 인라인 블럭으로 처리하고 싶은 부분을 `(백틱)으로 감싸줍니다.
* Block
  * \`(백틱)을 3번 입력하고 ```Enter```를 눌러 생성합니다.



​	`add` 한 요소를 remote 저장소에 올리려면 `$ git push origin master` 를 터미널에 입력합니다.

```shell
$ git add.
$ git commit -m "first commit"
$ git push origin master
```



### 1.4 Image

> 로컬에 있는 이미지를 삽입하거나 이미지 링크를 활용하여 이미지를 나타낼 때 사용합니다.

* `![]()` 을 작성하고 `()` 안에 이미지 주소를 입력합니다. `[]` 안에는 이미지 파일의 이름을 작성합니다.
* 로컬에 이미 파일을 저장한 경우 절대 경로가 아닌상대 경로를 사용하여 이미지를 저장합니다.

![git](data:image/png;base64,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)



![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT0UtxhD8qWjdblmhcRaVpENZu1Ff0c0vI3tw&usqp=CAU)





### 1.5 Link

> 특정 주소로 링크를 걸 때 사용합니다.

* `[]()` 을 작성하고 `()` 안에 링크 주소를 작성하고 `[]` 안에 어떤 링크 주소인지 작성합니다.

[git 공식문서](www.naver.com) 

[github 공식문서](www.github.com) 



### 1.6 Table

> 표를 작성하여 요소를 구분할 수 있습니다.

* `|` (파이프) 사이에 컬럼을 작성하고 `enter` 를 입력합니다.
* 마지막 컬럼을 작성하고 뒤에 `|` 를 붙여줍니다.

| working directory | statging area | romoe repo |
| ----------------- | ------------- | ---------- |
| working tree      | index         | history    |
| working copy      | cache         | tree       |



### 1.7 기타

##### 인용문

* `>` 을 입력하고 `enter` 키를 누릅니다.

> git은 컴퓨터 파일의 변경사항을 추적하고 여러 명의 사용자들 간에 해당 파일들의 작업을 조율하기 위한 분산 버전 관리 시스템이다.

* 인용문 안에 인용문을 작성하면 중첩해서 사용할 수 있습니다.

> $ git add .
>
> > $ git commit -m "first commit"
> >
> > > $ git push origin master



##### 수평선

* `---`,`***`,`___`을 입력하여 작성합니다.

Working Directory

---

Staging Area

***

Remote Repository

___

##### 강조

* 이탤릭체는 해당 부분을 `*` 혹은 `_` (언더바)로 감싸줍니다.
* 보드체는 해당 부분을 `**` 혹은 `__` (언더바 2개)로 감싸줍니다.
*  취소선은 `~~` 표시를 사용합니다.

이것은 _이탤릭체_ 입니다.

이것은 __보드체__입니다.

이것은 ~~취소선~~입니다.

# 2. 과제

> 현재의 pdf __문서__를 마크다운 문법을 활용하여 `00_markdown_basic.md`로 만들어 보세요.