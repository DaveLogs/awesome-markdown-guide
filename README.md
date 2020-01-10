# Awesome Markdown Guide

![Awesome markdown guide](images/0001.jpg)

Image by Pexels  from Pixabay (https://pixabay.com/photos/code-code-editor-coding-computer-1839406/)

<br>

## What is Markdown?

- 마크다운은 웹에서 스타일을 지정하는 방법 중 하나이다.
- 문서 표시를 제어할 수 있다.
  - 단어를 굵게(Bold) 또는 기울임꼴(Italic)로 표시하거나,
  - 이미지를 추가하고,
  - 목록을 만드는 일을 할 수 있다.
- GitHub에서는 
  -  Repository의 README 문서를 작성하거나,
  - [Gist](https://gist.github.com/)를 생성하고,
  - `.md` 또는 `.markdown` 을 확장자로 갖는 문서를 작성한다.  

<br>

## Basic Syntax



### 제목 (Headings)

```
# Heading level 1
## Heading level 2
###### Heading level 6
```

> # Heading level 1
>
> ## Heading level 2
>
> ###### Heading level 6

#### Alternate Syntax

```
Heading level 1
===============
```

> Heading level 1
> ===============

```
Heading level 2
---------------
```

> Heading level 2
> ---------------

<br>

### 강조 (Emphasis)

```
*This text will be italic*
_This will also be italic_
```

> *This text will be italic*
>
> _This will also be italic_

```
**This text will be bold**
__This will also be bold__
```

> **This text will be bold**
>
> __This will also be bold__

```
_You **can** combine them_
```

> _You **can** combine them_

<br>

### 취소선 (Strikethrough)

```
~~This text will have a strikethrough~~
```

> ~~This text will have a strikethrough~~

<br>

### 목록 (Lists)

#### 순서 없는 목록 (Unordered, 글머리 기호)

```
* Item 1
   * Item 1-1
   * Item 1-2
      * Item 1-2-1
- Item 2
+ Item 3
```

> * Item 1
>   * Item 1-1
>   * Item 1-2
>     * Item 1-3
> - Item 3
> + Item 4

```
* Step 1
   - Step 1-1
      + Step 1-1-1
```

> * Step 1
> 	* Step 1-1
> 		* Step 1-1-1

Note.

* 글머리 기호를 혼용해서 사용하길 수도 있다.

<br>

#### 순서 있는 목록 (Ordered, 번호)

```
1. First
1. Second
2. Third
```

> 1. First
> 1. Second
> 2. Third

Note.

* 입력하는 숫자에 관계없이 오름차순으로 배정된다.

<br>

#### 작업 목록 (Tasks)

```
[x] This is a complete item
[ ] This is an incomplete item
```

> [x] This is a complete item
>
> [ ] This is an incomplete item

Note.

- 제대로 동작하는 것인지 잘 모르겠음

<br>

### 인용 (Blockquotes)

```
> This is blockquote
>
> > This is nested blockquote
```

> > This is blockquote
> >
> > > This is nested blockquote

```
> Blockquotes can contain other Markdown formatted elements.
>
> #### Heading
>
> - unordered list
> 1. ordered list
>
> *Not all elements can be used* - **you'll need to experiment to see which ones work.**
```

> > Blockquotes can contain other Markdown formatted elements.
> >
> > #### Heading
> >
> > - unordered list
> > 1. ordered list
> >
> > *Not all elements can be used* - **you'll need to experiment to see which ones work.**

<br>

### 이미지 (Images)

```
![Sample image](images/0002.jpg)
Format: ![Alt Text](url)
```

> ![Sample image](images/0002.jpg)
>
> Photo by [Joris Visser](https://unsplash.com/@jorisv?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/s/photos/cafe?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)

Note.

- 캡션, 사이즈 조절은 지원하지 않음.
- 필요한 경우 HTML 태그로 처리.

<br>

### 링크 (Links)

```
[DaveLogs](http://davelogs.tistory.com)
Format: [Link Text](url)

http://davelogs.tistory.com - automatic!
```

> [DaveLogs](http://davelogs.tistory.com)
>
> http://davelogs.tistory.com - automatic!

<br>

### 인라인 코드 (Inline code)

```
You should write a `README.md` in GitHub.
```

> You should write a `README.md` in GitHub.

<br>

### 이모티콘 (Emoji)

```
Wow! Awesome!! :clap: :+1: :sunglasses:
```

>Wow! Awesome!! :clap: :+1: :sunglasses:

Note.

- [Emoji cheat sheet](https://www.webfx.com/tools/emoji-cheat-sheet/)

<br>

## Extended Syntax

### 테이블 (Tables)

```
Syntax    | Description | Test Text
--------- | ----------- | -----------
Header    | Title       | Here's this
Paragraph | Text        | And more
```

> | Syntax    | Description | Test Text   |
> | --------- | ----------- | ----------- |
> | Header    | Title       | Here's this |
> | Paragraph | Text        | And more    |

```
Syntax    | Description | Test Text
:-------- | :---------: | ----------:
Left      | Center      | Right
This      | is          | Alignment
```

> | Syntax | Description | Test Text |
> | :----- | :---------: | --------: |
> | Left   |   Center    |     Right |
> | This   |     is      | Alignment |

Note.

- 하이픈(`-`)과 파이프(`|`)를 이용해 표를 테이블을 구성
- 3개 이상의 하이픈(`-`)으로 첫번째 행으로 지정
- 콜론(`:`)과 하이픈(`-`)을 이용해 열(column)의 정렬 방법 설정

<br>

### 코드블록 (Fenced Code Blocks)

```
​```
$ sudo apt-get update
​```
```

> ```
> $ sudo apt-get update
> ```

#### Syntax highlighting

```
​```javascript
function fancyAlert(arg) {
   if(arg) {
      $.facebox({div:'#foo'})
   }
}
​```
```

> ```javascript
> function fancyAlert(arg) {
>    if(arg) {
>       $.facebox({div:'#foo'})
>    }
> }
> ```

<br>

```
​```python
def validate(arg):
   if arg is None:
      return False
   return True
​```
```

> ```python
> def validate(arg):
>    if arg is None:
>       return False
>    return True
> ```

<br>

```
​```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
​```
```

> ```json
> {
>   "firstName": "John",
>   "lastName": "Smith",
>   "age": 25
> }
> ```

<br>

## 참고

* [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
* [Getting Started \| Markdown Guide](https://www.markdownguide.org/getting-started/)
* [마크다운 사용법](https://gist.github.com/ihoneymon/652be052a0727ad59601)
* [마크다운(Markdown) 정리](https://blog.kim1jun.xyz/5)

