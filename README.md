# 정보처리기사 준비
## 데이터베이스

### 정보와 자료
-자료(Data):현실 세계에서 관찰이나 측정을 통해 수집한 단순한 사실이나 결과값으로, 가공되지 않은 상태  
-정보(Information):의사 결정에 도움을 줄 수 있는 유용한 형태로, 자료를 가공(처리)해서 얻는 결과물

### 데이터베이스의 정의
-통합된 데이터(Integrated Data):자료의 중복을 배제한 데이터의 모임  
-저장된 데이터(Stored Data):컴퓨터가 접근할 수 있는 저장 매체에 저장된 자료  
-운영 데이터(Operational Data):조직의 업무를 수행하는데 있어서 존재 가치가 확실하고 없어서는 안 될 반드시 필요한 자료  
-공용 데이터(Shared Data):여러 응용 시스템들이 공동으로 소유하고 유지하는 자료  

### 데이터베이스의 특징
-실시간 접근성(Real Time Accessibility):수시적이고 비정형적인 질의(조회)에 대하여 실시간 처리(Real-Time Processing)에 의한 응답이 가능함  
-계속적인 변화(Continuous Evolution):새로운 데이터의 삽입, 삭제, 갱신으로 항상 최신의 데이터를 유지함  
-동시공유(Concurrent Sharing):여러 사용자가 동시에 자기가 원하는 데이터를 이용할 수 있음  
-내용에 의한 참조(Content Reference):데이터베이스에 있는 데이터를 참조할 때 데이터 주소나 위치에 의해서가 아니라 사용자가 요구하는 데이터 내용으로 데이터를 찾음  

### DBMS(DataBase Management System)의 정의
-사용자와 데이터베이스 사이에서 사용자의 요구에 따라 정보를 생성해 주고, 데이터베이스를 관리해 주는 소프트웨어이다.

### DBMS의 필수 기능
-정의(Definition):데이터의 타입과 구조, 데이터가 DB에 저장될 때의 제약조건 등을 명시하는 기능  
-조직(Manipulation):데이터 검색(요청), 갱신(변경), 삽입, 삭제등을 체계적으로 처리하기 위해 데이터 접근 수단 등을 정하는 기능  
-제어(Control):
>데이터의 무결성이 유지되도록 제어해야 한다.  
보안을 유지하고 권한을 검사할 수 있어야 한다.  
병행 제어(Concurrency Control)를 할 수 있어야 한다.

### 논리적 독립성과 물리적 독립성
-논리적 독립성:응용 프로그램과 데이터베이스를 독립시킴으로써, 데이터의 논리적 구조를 변경시키더라도 응용 프로그램은 변경되지 않음  
-물리적 독립성:응용 프로그램과 보조기억장치 같은 물리적 장치를 독립시킴으로써, 데이터베이스 시스템의 성능 향상을 위해 새로운 디스크를 도입하더라도 응용 프로그램에는 영향을 주지 않고 데이터의 물리적 구조만을 변경함

### 스키마(Schema)  

-**정의**
>데이터베이스의 구조와 제약조건에 관한 전반적인 명세를 기술한다.  
데이터베이스를 구성하는 데이터 개체(Entity), 속성(Attribute), 관계(Relationship) 및 데이터 조작 시 데이터 값들이 갖는 제약조건 등에 관해 전반적으로 정의한다.  

-**스키마 3계층**
>-외부스키마(External Schema) = 서브 스키마 = 사용자 뷰
>사용자나 응용 프로그래머가 각 개인의 입장에서 필요로 하는 데이터베이스의 논리적 구조를 정의한다.  
전체 데이터베이스의 한 논리적인 부분으로 볼 수 있으므로 서브 스키마라고도 한다.  
하나의 데이터베이스 시스템에는 여러 개의 외부 스키마가 존재할 수 있으며, 하나의 외부 스키마를 여러개의 응용 프로그램이나 사용자가 공용할 수 있다.  
같은 데이터베이스에 대해서도 서로 다른 관점을 정의할 수 있도록 허용한다.  
일반 사용자는 SQL을 사용하여 DB를 사용한다.

-스키마