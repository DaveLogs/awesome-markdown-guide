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
> [ ] This is an incomplete item

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



<br>

### 링크 (Links)



<br>



<br>

## Extended Syntax



### 테이블 (Tables)



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

