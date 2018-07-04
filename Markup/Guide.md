# Markup guide
W3C 문법을 준수하며 코드에 통일성을 주고, 웹 표준 및 웹 접근성에 어긋나지 않게 시멘틱한 구조에 맞는 Markup을 하기 위한 가이드입니다.

1. 기본 규칙
2. DTD (Document Type Definition) 선언
3. Language 선언
4. Head 구성
5. Body 구성
***

## 1. 기본 규칙
규칙을 정하여 코드의 통일성을 줌으로써 협업 시 용이할 수 있습니다.
***

### 1.1 HTML 문자 인코딩 선언
HTML 문자 인코딩 선언은 meta 태그를 사용하여 기본적으로 utf-8로 설정한다. (여러 스크립트를 사용한 문서의 문자 처리를 단순화 시켜줌)
``` html
<meta charset="utf-8" />
```
### 1.2 HTML 들여쓰기
들여쓰기의 경우 Space를 사용하지 않고 Tab만을 이용하여 작업한다.
``` html
<div class="exem">
  <p>Space 사용 (X)</p>
     <p>Space 사용 (X)</p>
</div>
<div class="exem">
	<p>Tab 사용 (O)</p>
</div>
```
### 1.3 자기 마침 태그(Self-Closing Tags)
자기 마침 태그 사용 시에는 띄어쓰기 후 닫기 슬래시`(/)`를 사용한다.
``` html
<meta name="" content="" />
<link rel="" type="" href="" />
<input type="text" />
<col />
<img />
<hr />
```

## 2. DTD (Document Type Definition) 선언
DOCTYPE 선언은 HTML5 문서를 기본으로 사용하되 HTML5에서 추가된 태그들을 사용하지 않습니다. (IE 하위 버전 크로스 브라우징을 위함)
ex : `<header>`, `<section>`, `<footer>`, `<nav>`, `<article>` 등
``` html
<!DOCTYPE html>
```
