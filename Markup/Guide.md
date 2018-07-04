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

### 1.1 HTML 문자 인코딩 선언
HTML 문자 인코딩 선언은 meta 태그를 사용하여 기본적으로 utf-8로 설정한다.
``` html
<meta charset="utf-8" />
```

## 2. DTD (Document Type Definition) 선언
DOCTYPE 선언은 HTML5 문서를 기본으로 합니다.

### 1.1 
``` html
<!DOCTYPE html>
```
