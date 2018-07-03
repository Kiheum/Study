# Markup guide
Markup 할때 참고해야 할 사항을 정리
<!-- background: #fff4e3 -->
##DOCTYPE
DOCTYPE 버전 종류
- HTML 5 (HTML5에서는 SGML에 기반을 두지 않아서 DTD 참조가 필요 없으며, 최소한의 코드 작성이 기본 방향이라 매우 간단히 선언할 수 있다.)
- HTML 4.01 Strict (W3C가 의도했던 문서 타입으로, 구조와 표현을 분리하기 위해 단계적으로 사라질 표현에 관한 요소와 속성을 배제한 문서 타입이다. center, font, iframe, strike, u, 새창띄우기 등이 제한된다.)
- HTML 4.01 Transitional (기존에 만들어진 문서들과의 호환성을 유지하기 위해 사용한다. iframe과 새창띄우기(target="_blank")등을 사용할 수 있어 XHTML 사용시 이것을 추천한다.)
- HTML 4.01 Frameset (현재는 거의 사용하지 않는 프레임셋을 구현하기 위해서 사용한다.)
- XHTML 1.0 Strict (W3C가 의도했던 문서 타입으로, 구조와 표현을 분리하기 위해 단계적으로 사라질 표현에 관한 요소와 속성을 배제한 문서 타입이다. center, font, iframe, strike, u, 새창띄우기 등이 제한된다.)
- XHTML 1.0 Transitional (기존에 만들어진 문서들과의 호환성을 유지하기 위해 사용한다. iframe과 새창띄우기(target="_blank")등을 사용할 수 있어 XHTML 사용시 이것을 추천한다.)
- XHTML 1.0 Frameset (현재는 거의 사용하지 않는 프레임셋을 구현하기 위해서 사용한다.)
- XHTML 1.1 (기존의 XHTML 1.0 Strict DTD를 기본으로 한다.)

DOCTYPE 버전별 선언
- HTML5 <!DOCTYPE html>
- HTML 4.01 Strict <!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
- HTML 4.01 Transitional <!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
- HTML 4.01 Frameset <!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN" "http://www.w3.org/TR/html4/frameset.dtd">
- XHTML 1.0 Strict <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1-strict.dtd">
- XHTML 1.0 Transitional <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1-transitional.dtd">
- XHTML 1.0 Frameset <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Frameset//EN" "http://www.w3.org/TR/xhtml1-frameset.dtd">
- XHTML 1.1 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">

##Title
각 페이지마다 서로 다른 규칙으로 사용중인 문서 제목 (<title> 태그) 규칙을 일원화함으로써, 서비스 통일성을 높이고 사내 검색 엔진에 대한 최적화를 꾀한다. 또한 문서 제목에 컨텐츠 제목을 포함시킴으로써, 외부 검색서비스에서 해당 컨텐츠의 노출이 더 잘될 수 있도록 한다.
기본 규칙 : 컨텐츠 제목 - 하위 섹션명 | 서비스명

##Meta
meta 태그는 메타태그는 웹 서버와 웹 브라우저간에 상호 교환되는 정보를 정의하는데 사용한다.

meta 태그의 속성
- http-equiv="항목명" (웹 브라우저가 서버에 명령을 내리는 속성으로 name 속성을 대신하여 사용될 수 있으며, HTML 문서가 응답 헤더와 함께 웹 서버로부터 웹 브라우저에 전송되었을 때에만 의미를 갖음.)
- content="정보값" (meta 정보의 내용을 지정한다.)
- name="정보 이름" (몇 개의 meta 정보의 이름을 정할 수 있으며 지정하지 않으면 http-equiv 와 같은 기능을 한다.)

meta 태그의 종류
