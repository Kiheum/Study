# Markup guide
W3C에서 제정한 웹 표준 및 웹 접근성을 준수하고, 문서 작성 규칙을 일원화함으로써 통일성을 높여 협업 시 업무의 효율성을 높이기 위해 작성한 가이드입니다.

1. DTD (Document Type Definition)
2. language
3. head
4. skip navigation
5. body
6. attribute
7. self-closing tags
***

## 1. DTD (Document Type Definition)
DOCTYPE 선언은 HTML5 문서를 기본으로 사용하되 HTML5에서 추가된 태그들을 사용하지 않는다.  
__IE 하위 버전 Cross Browsing을 위함__  
ex : `<header>`, `<section>`, `<footer>`, `<nav>`, `<article>` 등
``` html
<!DOCTYPE html>
```

## 2. language
language 속성을 기본적으로 `<html>` 태그에 지정한다. (ex : `lang="ko"`, `lang="en"`, lang="ja"`등)
``` html
<html lang="ko">
```

## 3. head
`<head>` 의 자식 요소의 순서는 다음과 같이 작성한다.

1. meta charset (html 문자 인코딩 선언은 `utf-8`을 기본으로 지정)
2. meta X-UA-Compatible (`IE`의 경우 최신버전인 `Edge`를 사용)
3. meta viewport
4. title (컨텐츠 제목 &ndash; 하위 섹션명 | 서비스명 규칙으로 작성)
5. meta etc (ex : `keyword`, `description` 등)
6. link (다른 문서 또는 외부 소스와의 링크)
``` html
<meta charset="utf-8" />
<meta http-equiv="X-UA-Compatible" content="IE=edge" />
<meta name="viewport" content="width=device-width, user-scalable=no" />
<title>2018 히든홀 신비의 동굴 – 이벤트 | KaKaoVX</title>
<meta name="keyword" content="markup guide" />
<link rel="stylesheet" type="text/css" href="reset.css" />
```

## 4. skip navigation
웹 접근성을 준수하여 본문으로 바로 이동 가능한 건너뛰기 링크를 작성한다.  
__skip navigation의 경우 사용자의 혼선을 막기 위해__ `<body>` __가 시작하고 바로 제공할 수 있도록 한다.__
``` html
<body>
	<div id="skip-navigation">
		<a href="#container">본문으로 바로가기</a>
	</div>
	<div id="wrap">
		<div id="header"></div>
		<div id="container"></div>
		<div id="footer"></div>
	</div>
</body>
```

## 5. body
`<body>` 의 문서 안에 JS 문서를 호출하되 반드시 가장 하단에 호출하도록 한다.  
__웹 브라우저가 렌더링 되는 과정에서 HTML, CSS문서를 먼저 해석하고 마지막에 JS를 불러오기 위함__  
전체 컨텐츠를 컨트롤 할 수 있는 `<div class="wrap"></div>` 작성하도록 한다.
``` html
<body>
	<div id="skip-navigation">
		<a href="#container">본문으로 바로가기</a>
	</div>
	<div id="wrap">
		<div id="header"></div>
		<div id="container"></div>
		<div id="footer"></div>
	</div>
	<script type="text/javascript" src="common.js"></script>
</body>
```

## 6. attribute
attribute 작성 시 쌍 따옴표를 사용하고 `""`,  
우선순위는 `rel`, `type`, `href, src`, `width, height`, `target`, `id`, `name`, `class`, `style`, `title, alt`, `기타` 순으로 작성한다.  
__id의 경우 같은 이름으로 작성하지 않는다. 또한 최소화하도록 한다.__
``` html
<a href="" target="" id="" class="" style="" title="">예제</a>
<img src="" width="" height="" id="" class="" style="" alt="" title="" />
<input type="" id="" name="" class="" style="" title="" size="" maxlength="" />
```

## 7. self-closing tags
self-closing tags 작성 시 닫기 슬래시 (`/`)를 사용한다.  
__DOCTYPE이 HTML5 문서라고 하더라도 사용한다. (웹 표준 준수)__
``` html
<meta name="" content="" />
<link rel="" type="" href="" />
<input type="" class="" />
<img src="" alt="" />
<col />
<br />
<hr />
```

