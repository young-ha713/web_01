# web_01  
  
  
  
  
  
1.용어정리<키워드는 숲을 그리고 디테일을 잡음>  
- db :(oracle ,my sql)사용함. sql 조작  
- java : 자료형,문법,리스트,맵,배열>1차원,2차원
- html&css  
-javascript  
   
2.서버 클라이언트 구조 이해  
  
  
![image](https://user-images.githubusercontent.com/80766275/201236193-e8bddd17-d74a-44fe-863a-62c99d1165cd.png)

  
방화벽은 ip,port,tcp나 udp관리 등을 함(외에도 있다)
  
-클라이언트  
-서버(서버에서 db와의 구조)  
  
  
  
  
3.개발환경 이해  
  
  
-분홍색의 흐름 이해  
-녹색의 흐름 이해
  
  이 구조가 기본임!!!!!!!!!!!  
  
  웹프로그램 : 
    1.정부24 - 항상 똑같은 화면..  
    2.넷플릭스 - 고객의 성향에 맞춰 화면이 다른 성향  
  
  
  
  
4.통신 과정의 예(암기)    
  
가. view이해- 서버의 응답(response)  
  
보이는 네이버 화면의 소스는 서버에 저장되어있고 클라이언트에게 주는것.. 
서버에서는 클라이언트에게 보여줄 화면을 미리 만들어 놓는다. 
기본은html문서이며 jsp로 병행해서 만들것이다.  
*** 이것을 view 라고 한다. ***  
  
  
나.요청(request)-url로 많이 요청함    
  
a. 요청에서 반드시 필요한것 : 요청명(메인 보여달라, 글 쓰겠다)  
요청명이란 전공단어는 아님.. 의미는 요청하는 의도정도??  
  전공단어 :서블릿 요청(중복불가)  
  
b. 서블릿 요청시 넘겨줄 데이터(파라미터) 유무  
데이터베이스 쿼리 생각해보면 쉽다.where절이 있다면 파라미터 필요한것 많음  
예) 메인화면 요청 : 파라미터 필요 없다.  
    로그인 요청 : 파라미터 필요함.(아이디,비번이 파라미터)  
    게시글에서 3번 자세히 : 파라미터 필요 (글 번호)
    
    **파라미터를 서버에서 어떤 방식으로 전송??
    1.get <a href="서블릿요청?변수=값&변수=값> 등  
    2.post<form action ="" method =post> 등  
            <input type ="text" name="">
            name으로 지정한것이 변수명이 된다..
    3.json (자바스크립트 객체형식으로 보냄)<jquery 등>  
            key,value 로 객체를 정의한다  
  
  
  
다. 서버  
1. 서블릿분석:  클라이언트가 원하는 서비스 분석    
2. 클라이언트가 보낸 파라미터를 받아야한다.  
    *클라이언트가 보낸 방식에 따라 처리 방법이 다름.  
3. 필요하다면 db에서 데이터 조작한다.
4. 클라이언트에게 보낼 화면을 만든다
   화면을 정의한것이 바로 view 파일(html,jsp 등)  
5. 실제코드(html,css,js)을 클라이언트에게 전송한다..  
  
  
지금까지 우리가 공부한 js사용목적을 한 줄로 한다면  
>> html문서의 요소를 조작하여 전체화면이 아닌  
  화면의 일부를 제어한다.  
  응용) 인별그램 사용중...>좋아요 누른다.
        관심1. 하트가 변해야 한다..빨갛게 변하는게 중요  
        관심2.눌러놓고 다른거 한다.  
  무슨 뜻이냐..문서에서 주요기능과 세부기능을 구분  
  클라이언트가 사용하는 주요기능을 방해하지 않으며 세부기능을 구현할 수 있다.  
  
  또는 9시에 댓글을 보고있다..9시 1분에 누가 댓을을 달았다..이 사람은 댓을 볼 수 있다..그런데 화면 일부만 제어하는 기술로
  최근 댓글을 업데이트 할 수 있다.  
    
  장바구니에서 삭제하는 품목이 있을때 화면 전체를 갱신하지 않고 일부분만 삭제하거나 수정할 수 있다.  
  >>이것을 비동기 통신이라고 함..  ..ajax 사용 많이 함  
  
  
![image](https://user-images.githubusercontent.com/80766275/201247563-e021be0f-c02d-4d7e-8c40-bb186f7e1789.png)
  
  
아파치 톰캣은 자바 기반의 서블릿!!!!!  
  
  
  
  
![image](https://user-images.githubusercontent.com/80766275/201254514-569526db-3893-4d47-a2bb-610ac9c12fae.png)
  
  
  
  
--------------------------------------  
  


![image](https://user-images.githubusercontent.com/80766275/201269288-459eb6c4-50bb-44c8-9648-aa00527d8f7d.png)
  
  

![image](https://user-images.githubusercontent.com/80766275/201274530-ae299726-842b-4289-9178-f2f3a30a401e.png)
teamname= 변수명  
  
  
  
  
  
  
![image](https://user-images.githubusercontent.com/80766275/201275345-dc3493e0-1269-4472-821c-9c9a8cbb1560.png)
  
  
  
  
  
오후과제  
  
  
![image](https://user-images.githubusercontent.com/80766275/201291304-fa1560aa-e358-4a87-9b62-3baef30c1ed8.png)
  
  
![image](https://user-images.githubusercontent.com/80766275/201291384-bdafc118-3ebd-4e55-afd0-0acb660443d1.png)
  
  
![image](https://user-images.githubusercontent.com/80766275/201291955-00a4da96-a68c-47fe-bd95-9fd02d43ba43.png)

  
--------------------------------------------------------------------  
  
  
### 정리  
  
1.웹서비스 구조,,서버와 클라이언트 - tcp/udp ip port  
2.설치한 웹 서버 프로그램
3.서블렛이 무엇인가와 서블릿 만드는 방법  
4.클라이언트가 서블렛 호출하는 방법2가지  
5.컨트롤러가 클라이언트에게 파라미터 받는법  
6.컨트롤러가 view를 선택하여 포워딩 하는 과정(view에게 데이터를 넘겨주는 코딩 포함)  
7.클라이언트가 직접 view를 호출하는것과 컨트롤러를 호출하는것의 차이점..  

