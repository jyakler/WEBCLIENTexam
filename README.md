# WEBCLIENTexam
CSS
1. 지역적(inline) : 태그에 style 속성을 사용하는 방법( style="CSS속성명:CSS속성값;CSS속성명:CSS속성값" )
2. 전역적(global) : <head>태그에 <style> 이라는 태그를 작성하고 컨텐트로 CSS 코드 작성하는 방법

    대상 {
      CSS속성명:CSS속성값;
      CSS속성명:CSS속성값;
        }       
    대상 - CSS Selector(선택자)
    
3.외부파일 : CSS 코드를 독립된 파일(xxx.css)로 생성해서 HTML 문서 안으로 포함시키는 방법
                      <link> 또는 import 구문을 사용
                      
***
                      
                       [src]
                       [src=1.png]
                       [src$=png]  (png로 끝나는)
                       [src^=duke]  (duke로 시작하는)
                       
 ***
 
        식1 && 식2  (식1이 true일때 식2 실행)
  
        식1 || 식2  (식1이 false일때 식2 실행)
        
***
        var 변수
        let 변수    (단한번만 가능)
        const 변수=초기값  (단한번만 가능, 할당된 값 변경불가)
        
***
## DOM 객체 찾기
      document.getElementsByTagName("태그명")[index]  --> Element 객체들을 저장한 유사 배열 객체
      document.getElementById("id속성값")  --> Element 객체 또는 null
 
      document.querySelector("찾으려는태그의 CSS선택자")  --> Element 객체 또는 null  (이때 id값이면 앞에 #을 붙여야함 ex. <h1> -> "h1"  /  <h1 id="t1"> -> "#t1")
      document.querySelectorAll("찾으려는태그의 CSS선택자")  --> Element 객체들을 저장한 유사 배열 객체
      
### 이벤트 핸들러 구현 방법
  1. 인라인 이벤트 모델
	<태그명 onxxx = "수행코드">
  2. 고전 이벤트 모델
	dom객체.onxxx = 함수
  3. 표준 이벤트 모델
  dom객체.addEventListener("xxx", 함수)
		
***
## 사이트이동
	location.href=url;
	
***
## 날짜 출력
	var d=new Date();
	d==Tue Feb 15 2022 09:18:09 GMT+0900 (한국 표준시)
	d.toLocaleString()==2022. 2. 15. 오전 9:18:09
	d.getFullYear();
	d.getMonth();
	d.getDate();
	d.getDay(); // 0 : 일요일
		...
