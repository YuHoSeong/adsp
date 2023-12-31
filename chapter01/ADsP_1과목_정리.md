# ADsP 1과목 : 데이터 이해
## 01 정량적데이터
- 정량적 데이터
    - **지역별 온도, 풍속, 강우량과 같이 수치로 명확하게 표현**되는 이것은 데이터의 양이 크게 증가하더라도 이를 관리하는 시스템에 저장, 검색, 분석하여 활용하기가 매우 용이함
    - 도형, 기호, 숫자의 데이터
- 정성적 데이터
    - 기상특보와 같이 언어, 문자 등으로 기술
    - 비정형 데이터의 형태로 저장, 분석에 시간과 비용이 필요함

## 02 지식경영 데이터
- 데이터는 지식경영의 핵심 이슈인 암묵지와 형식지의 상호작용을 함
- 지식의 차원에 대해 가장 널리 알려진 것은 Polanyi에 의해 두가지 차원으로 구성된 암묵지와 형식지임
- 암묵지
    - 김장김치 담그기의 노하우
    - 암묵지는 개인에게 체화되기 때문에 공유하기 어려움
    - 현장작업과 같은 경험을 통해 획득할 수 있는 지식
    - 개인에 체화된 비밀스러운 지식
- 형식지
    - 문서나 매뉴얼처럼 외부로 표출되어 여러 사람이 공유할 수 있는 지식
    - 회계, 재무 관련 대차대조표에 요구되는 지식의 매뉴얼

## 03 암묵지,형식지의 4단계 지식전환 모드
*(공표연내..)*

- 1단계: 암묵적 지식 노하우를 **다른사람**에게 알려주는 것 - 공통화
- 2단계: 암묵적 지식 노하우를 **책이나 교본 등 형식지로 만드는 것** - 표출화
- 3단계: 책이나 교본(형식지)에 자신이 알고있는 새로운 지식(형식지)를 추가하는 것 - 연결화
- 4단계: 만들어진 책이나 교본(형식지)를 보고 다른 직원들이 암묵적 지식(노하우)을 습득 - 내면화

## 04 데이터와 정보의 관계
- DIKW 피라미드 | 데이터 - 정보 - 지식 - 지혜
    - 정보 : 데이터의 가공 및 처리와 데이터간 연관관계 속에서 의미가 도출된 것
- 데이터 단위
    - KB 킬로 < MB 메가 < GB 기가 < TB 테라 **< PB 페타 < EB 엑사 < ZB 제타 < YB 요타**

## 05 DBMS, RDBMS, ODBMS
- DBMS : 사용자와 데이터베이스 사이에서 사용자의 요구에 따라 정보를 처리해주고 데이터베이스를 관리해주는 소프트웨어
- 관계형 데이터베이스 관리 시스템(RDBMS)
    - 정형화된 테이블로 구성된 데이터 항목들의 집합체
    - SQL: RDBMS의 데이터를 관리하기 위해 설계된 특수 목적의 프로그래밍 언어로 챔벌린과 보이스가 개발되었던 프로그래밍 언어
    - MySQL이 있음
- 객체지향 데이터베이스 관리 시스템(ODBMS)
    - 객체들을 생성하여 계층에서 체계적으로 정리하고, 다시 계층들을 하위 계층이 상위 계층으로부터 속성과 방법들을 물려받을 수 있는 DBMS
    - 복잡한 데이터 구조를 표현 및 관리하는 DBMS

## 06 데이터베이스의 특징
- 통합된 데이터(Integrated data)
    - 데이터베이스에서 같은 내용의 데이터가 중복되지 않게 통합되어 있다.
- 저장된 데이터(Stored data)
    - 컴퓨터가 접근할 수 있는 저장매체에 저장되어 있다.
- 공용 데이터(Shared data)
    - 여러 사용자가 다른 목적으로 데이터를 공유 할 수 있다.
- 변화된 데이터(Operaional data)
    - 삽입,수정,삭제,갱신을 통해 항상 현재의 정확한 데이터를 유지해야 한다.

## 07 데이터베이스 관련
- 데이터베이스 설계 절차
    - 요구조건 분석 -> 개념적 설계 -> 논리적 설계 -> 물리적 설계
- NoSQL 저장방식 도구
    - MongoDB, HBase, Redis
- 트랜잭션(Transaction)
    - 데이터베이스에서 명령을 수행하는 하나의 논리적인 기능의 단위
    - ACID
        - 원자성 Atomicity
            - 트랜잭션은 데이터베이스에 **모두 적용되거나, 모두 적용되지 않아야 함**
        - 일관성 Consistency
            - 트랜잭션의 결과는 항상 일관적이어야함. **(완료하면 항상 유지)**
        - 고립성 Isolation
            - 다른 트랜잭션에 영향을 주지 않아야함. **(중간 과정에 개입 불가)**
        - 지속성 Durability
            - 트랜잭션이 완료되면 **그 결과는 영구적**이어야함.
- 데이터베이스 구성요소
    - 인스턴스 : 하나의 객체 | 사람,동물,물건 등
    - 속성 : 객체를 표현하기 위해 사용되는 값 | 이름,성별,직업 등
    - 엔터디 : 데이터의 집합(개념적 존재) | 개념,장소,사건 등
    - 메타데이터 : 데이터를 설명하는 데이터 | 파일 생성 날짜 등
    - 인덱스 : 자동적으로 생성되는 데이터의 이름 | 정렬, 탐색을 위한 색인
- SQL 언어 : DDL, DML, DCL, TCL
    - DDL :데이터정의 언어
        - CREATE : 테이블 생성
        - ALTER: 테이블 정보 변경
        - RENAME: 테이블 이름 변경
        - DROP: 테이블 삭제
    - DML : 데이터 조작 언어
        - SELECT: 데이터 조회
        - INSERT: 데이터 삽입
        - UPDATE: 데이터 변경
        - DELETE: 데이터 삭제
    - DCL : 데이터 제어 언어
        - GRANT: 권한 부여
        - REVOKE: 권한 회수
    - TCL : 트랜잭션 제어 언어
        - COMMIT: 변경 일괄 적용
        - SAVEPOINT: 현재 상태 기억
        - ROLLBACK: 특정 시점으로

## 08 시대별 기업내부 데이터베이스 솔루션
- OLTP(On-Line Transaction Processing)
    - 각각의 거래단위/트랜잭션에 초점을 맞춘 시스템
    - 기업 활동에서 영역별로 구축되던 **단순 자동화** 중심 시스템
- OLAP(On-Line Analytical Processing)
    - 각각 데이터가 쌓인 전제 데이터에 초점을 맞춤
    - 다차원의 데이터를 대화식으로 분석하기 위한 소프트웨어
    - 단순한 정보 수집, 공유에서 **분석이 중심**이 되는 시스템 구축을 변화
- CRM(Customer Relationship Management)
    - 제조 부문의 고객 관계 관리
    - 기업 **내외부**적인 분석을 통해 마케팅 측면에서 신규고객 창출 또는 기존고객 이탈 방지
- SCM(Supply Chain Management)
    - 유통 부문의 공급망 관리
    - 원자재에서 기업을 거쳐 고객에게 도달할 때까지 **유통단계를 최적화**
    - 물류, 유통업체 등 유통공급망에 참여하는 모든 업체들이 협력을 바탕으로 **정보 기술을 활용, 재고를 최적화하기 위한 솔루션**

## 09 분야별 기업내부 데이터베이스 솔루션 - 제조
- 데이터웨어하우스, DW(Data Warehouse)
    - 정보 검색을 목적으로 구축된 데이터베이스
    - 기업 내의 의사결정 지원 애플리케이션을 위한 정보를 제공하는 하나의 통합된 데이터 저장 공간
    - ETL은 주기적으로 내부 및 외부 데이터베이스로부터 정보를 추출하고 정해진 규약에 따라 정보를 변환한 후에 데이터 웨어하우스에 정보를 적재함
    - 방대한 조직 내에서 분산 운영되는 각각의 데이터 베이스 관리 시스템들을 효율적으로 통합하여 조정, 관리하기 때문에 효율적인 의사결정 시스템을 위한 기초를 제공하는 정보관리시스템
    - 데이터들은 시간적 흐름에 따라 변화하는 값을 유지
    - **데이터웨어아우스의 4대 특성** *(시비주통..시비걸면 죽통을 날려버림..ㅎㅎ)*
        - 데이터의 통합 : 데이터들은 전사적 차원에서 일관된 형식으로 정의됨
        - 데이터의 시계열성 : 관리되는 데이터들은 시간의 흐름에 따라 변화하는 값을 저장함
        - 주체지향적, 비소멸성 : 특정 주제에 따라 데이터들이 분류,저장,관리됨
- 데이터 마트
    - 전사적 차원에서 접근하기보다 재무,생산,운영과 같이 **특정 조직의 특정 업무 분야에 초점**을 두고 있음
    - 전사적으로 구축된 데이터웨어하우스로부터 특정 주제, 부서 중심으로 구축된 소규모 단일 주제의 데이터웨어하우스
- ERP(Enterprise Resource Planning)
    - 제조 부문의 경영자원 통합관리
    - 여러 자원, 업무를 하나로 **통합된 시스템**으로 재구축하여 업무 효율성을 높이는 것이 목적
- BI(Business Intelligence)
    - 제조 부문의 기업 의사결정 프로세스
    - 여러 곳에 산재되어 있는 데이터를 수집,정리하여, **필요한 정보를 정확한 시간에 제공**
    - BI가 빅데이터 분석의 차이점을 표현한 키워드 : ad hoc report(하나의 특정 비즈니스 질문에 답변하도록 설계된 BI)
- BA(Business Analytics)
    - 경영 의사결정을 위한 통계적이고 수학적인 분석에 초점을 둔 기법

## 10 그외 분야별기업내부 데이터베이스 솔루션
- 블록체인(Block Chain) - 금융부문
    - 기존 금융회사의 중앙 집중형 서버에 거래 기록을 보관하는 방식에서 벗어나 거래에 참여하는 모든 사용자에게 거래 내용을 보내주며 거래 때마다 이를 대조하는 데이터 위조 방지 기술
- KMS(Knowledge Management System) - 유통부문
    - 지식 경영 시스템
    - 기업이 보유할 수 있는 **모든 지식을 통합**하여 문제 해결 능력을 향상시키는 것이 목적
- RFID - 유통부문
    - 무선주파수(RF,Radio Frequency)를 이용하여 대상을 식별할 수 있는 기술
    - RF 태그에 사용 목적에 알맞은 정보를 저장하여 적용 대상에 부착한 후 판독기에 해당되는 RFID 리더를 통해 정보를 인식함
- EAI(Enterprise Application Integration)
    - 모든 서비스를 중앙에서 관리하여 애플리케이션 통합
    - 한기업의 여러 서비스간 연계를 위해, 중양에서 관리하면서 **연결루트를 간소화**함
- RTE(Real Time Enterprise)
    - 실시간 기업 경영 스피드 경영
    - 기업 업무 프로세스에서 발생하는 정보를 **실시간**으로 통합, 전달하여 **신속한 대응 가능**
- [국가] 관련
    - ITE : 지능형 교통 시스템
    - NGIS : 국가지리 정보체계,
    - NEIS : 교육행정 정보시스템

## 11 빅데이터의 정의
- 정의
    - 빅데이터는 일반적인 데이터베이스 소프트웨어로 저장, 관리, 분석할 수 있는 범위를 초과하는 규모의 데이터다
    - 빅데이터는 다양한 종류의 대규모 데이터로부터 저렴한 비용으로 가치를 추출하고, 데이터의 초고속 수집, 발굴, 분석을 지원하도록 고안된 차세대 기술 및 아키텍처이다
    - 데이터의 양(Volume) 데이터 유형과 소스 측면의 다양성(Variety), 데이터 수집과 처리 측면에서 속도(Velocity)가 급격히 증가하면서 나타난 현상이다
- 빅데이터의 특징 | 4V
    - ROI관점에서 보는 빅데이터이다
    - Volume, Variety, Velocity 는 '투자비용 요소'이다.
    - Value는 '비즈니스 효과'에 해당한다.

## 12 빅데이터의 출현 배경
- 데이터의 양적 증가
    - 과학기술 발달
    - 컴퓨터, 스마트폰 보급
    - 기술의 패러다임 시프트
- 관련 기술 발전
    - 저장기술 발전
    - 인터넷, 모바일 발전
    - 클라우드컴퓨팅→처리비용↓
        - 클라우드 컴퓨팅 : 빅 데이터 분석에 경제적 효과를 제공해준 결정적 기술
- 산업계 변화
    - 양질 전환의 법칙
    - 거대한 데이터가 새로운 기술을 만나 새로운 가치 창출
- 학계 변화
    - 기술아키텍처, 통계도구 발전
    - 게놈 프로젝트
    - 기후 시뮬레이션 등

## 13 빅데이터의 역할 - 플랫폼
- 페이스북은 SNS 서비스로 시작했지만, 2006년 F8 행사를 기점으로 자신들의 소셜 그래프 자산을 외부 개발자들에게 공개하고 서드파티 개발자들이 페이스북 위에서 작동하는 앱을 만들기 시작했다
- 각종 사용자 데이터나 M2M 센서 등에서 수집된 데이터를 가공, 처리, 저장해 두고, 이 데이터에 접근할 수 있도록 API를 공개하였다

## 14 빅데이터에 의한 변화
- 사전처리 -> 사후처리
- 표본조사 -> 전수조사
- 질 -> 양
- 인과관계 -> 상관관계

## 15 빅데이터의 가치
- 빅데이터 가치 산정의 어려움
    - 데이터 활용방식의 변화
        - 빅데이터 재사용, 재조합, 다목적 개발
        &rarr; 특정 데이터를 누가, 언제, 어떻게, 어디서 활용하는지 알 수 없게 됨.
    - 가치 창출 방식의 변화
        - 빅데이터가 기존에 없던 새로운 가치를 창출함 
        &rarr; 가치를 산정하기 어려움
    - 분석 기술의 발전
        - 데이터 분석 기술의 발전
        &rarr; 가치있는 데이터와 가치없는 데이터의 경계를 나누기 어려워짐

## 16 빅데이터 활용 기법
- 빅데이터 활용
    - 기업 - 구글, 월마트
    - 정부 - 교통, 기후, 지질, 안전 등
    - 개인 - 정치인, 연예인 SNS
- 미래의 빅데이터 활용에 필요한 3요소
    - 데이터 : 모든 것의 데이터화
    - 기술 : 진화하는 알고리즘과 인공지능
    - 인력 : 데이터 사이언티스트, 알고리즈미스트
- 7가지 빅데이터 활용 기법
    - 연관규칙 학습 = 연관분석, 장바구니 분석
        - 어떤 변인간에 주목할만한 **상관관계**가 있는지 분석
        - A를 구매한 사람이 B를 더 많이 구매하는가?
    - 유형분석 | 분류 & 군집화
        - 새로운 사건이 속할 **범주**를 찾아내는 방법
        - 온라인 수강생들의 특성을 반영 &rarr; 어떻게 분류할 것인가?
    - 유전 알고리즘(Genetic algorithms)
        - 자연선택, 돌연변이 등을 통해 점진적으로 **진화**시킴
        - 최적화 문제
        - 배치 효율화 문제
    - 기계학습 = 머신러닝(Machine learning)
        - 훈련 데이터로부터 학습한, 알려진 특성을 통해 예측
        - 영화 추천 시스템, 스팸메일 필터링, 질병진단 예측
    - 회귀분석(Regression analysis)
        - 독립변수를 조작하면서 종속변수가 어떻게 변화하는지 분석
        **&rarr; 두변인의 관계를 파악**
        - 사용자의 만족도가 브랜드 충성도에 어떤 영향을 미치는가?
    - 감성분석(Sentiment analysis)
        - 특정 주제에 대해 말한/서술한 사람의 **감성을 분석**하는 방법
        **&rarr; 비정형/텍스트마이닝 &rarr; 긍부정 선별**
        - 호텔을 이용한 고객의 후기(리뷰)를 분석하여 고객의 니즈를 찾아냄
    - 소셜 네트워크 분석 SNA(Social Network Analysis)
        - SNS와 같은 온라인 공간에서 영향력 있는 사람(오피니언 리더)을 찾아내고, 고객 간 소셜 관계를 파악함
        - 특정인과 타인의 관계가 몇 촌인가?
        - 특정인이 어느 정도 영향력이 있는가?

## 17 빅데이터 위기 요인과 해결 방안
1. 사생활 침해
    - 동의제를 책임제로 전환 : 개인 정보 사용자에게 책임을 지움
    - 익명화(Anonymity) : 빅데이터 시대가 도래하면서 발생하는 사생활 침해를 막기 위해 데이터에 포함된 개인 식별 정보를 삭제하거나 알아볼 수 없는 형태로 변환하는 포괄적 기술
2. 책임원칙 훼손
    - 기존의 책임원칙을 강화한다
    - 책임훼손의 예) 범죄 예측 프로그램을 통해 범죄 전 체포
3. 데이터 오용
    - 데이터 알고리즘에 대한 접근권 허용 및 객관적 인증방안을 도입 필요성

## 18 개인 정보 비식별화 기법
- 가명처리 : 다른값으로 대체
    - 홍길동, 25세 &rarr; 김가명, 20대
- 데이터 마스킹 : 임의의 값으로 대체
    - 홍길동, 한국대학교 &rarr; 홍OO, OO대학교
- 데이터 범주화 : 특정값이 아닌 범위
    - 홍길동, 55세 &rarr; 홍씨, 50-60세
- 데이터값 삭제 : 데이터값의 일부 삭제
    - 901212-2000000 &rarr; 90년대생,여성
- 총계 처리 : 통곗값(총합,평균) 적용
    - 김-50kg, 이-60kg &rarr; 몸무게합=110kg

## 19 대표적인 일차원 분석
- **에너지 : 트레이딩, 공급, 수요 예측**
- 긍융 서비스 : 신용점수 산정, 사기 탐지, 고객 수익성 분석
- 병원 : 가격 책정, 고객 로열티, 수익 관리
- 정보 : 사기 탐지, 사례 관리, 범죄 방지, 수익 최적화
- 소매업 : 재고 보충, 수요예측
- 제조업 : 맞춤형 상품 개발, 신상품 개발
- 온라인 : 웹 매트릭스, 사이트 설계, 고객 추천

## 20 데이터 사이언스(Data Science)
- 데이터로부터 의미 있는 정보를 추출해내는 학문이며, 정형 또는 비정형 막론하고 인터넷, 휴대전화, 감시용 카메라 등에서 생성되는 숫자와 문자, 영상 정보등 다양한 유형의 데이터를 대상으로 하며, 분석뿐 아니라 이를 효과적으로 구현하고 전달하는 과정까지 포함한 포괄적 개념이다
- 데이터 사이언스란 데이터로부터 의미있는 정보를 추출해내는 학문이다
- **강력한 호기심**이야말로 데이터 사이언티스트의 중요한 특징이라고 할 수 있다
- 데이터 사이언스는 과학과 인문학의 교차로에 서 있다고 할 수 있다
- 데이터 사이언스의 핵심 구성요소로는 IT 영역, 분석적 영역, 비즈니스 컨설팅 영역이 있다
- 데이터 공학(Data Engineering), 수학, 통계학, 컴퓨터 공학, 시각화, 해커의 사고방식, 해당 분야의 전문 지식을 종합한 학문
- **통계학 vs 데이터 사이언스**
    - 통계학 : 정형화된 실험 데이터를 분석
    - 데이터 사이언스 : 다양한 유형을 대상으로 함, `총체적(holistic) 접근법`을 사용
- 데이터 사이언스 구성요소
    - Analytics
        - 수학, 확률모델, 머신러닝, 분석학
        - 패턴 인식과 학습
        - 불확실성 모델링 등
    - IT(Data Management)
        - 시그널프로세싱, 프로그래밍
        - 데이터 엔지니어링, 데이터 웨어하우징
        - 고성능 컴퓨팅 등
    - 비즈니스 분석
        - 커뮤니케이션
        - 프레젠테이션
        - 스토리텔링, 시각화 등

## 21 데이터 사이언티스트의 역량
- 가트너가 제시한 역량 : `데이터 관리`, `분석 모델링`, `비즈니스 분석`,`소프트스킬`
- 데이터 사이언티스트는 데이터 해커, 애널리스트, 커뮤니케이션, 신뢰받는 어드바이저 등의 조합이라 할 수 있다
- 하드 스킬과 소프트 스킬 능력을 동시에 갖추고 있어야 한다
- 데이터 처리 기술 이외에 사고방식, 비즈니스 이슈에 대한 감각, 고객들에 대한 공감 능력이 필요하다
- 데이터 사이언티스트가 효과적 분석모델 개발을 위해 고려해야 하는 사항
    - 분석 모델이 예측할 수 없는 위험을 살피기 위해 현실 세계를 돌아보고 분석을 경험과 세상에 대한 통찰력과 함께 활용한다
    - 가정들과 현실의 불일치에 대해 끊임 없이 고찰하고 모델의 능력에 대해 항상 의구심을 갖는다
    - 분석의 객관성에 의문을 제기하고 분석 모델에 포함된 가정과 해석의 개입 등의 한계를 고려한다
    - 모델 범위 바깥의 요인은 판단하지 않는다

## 22 하드 스킬, 소프트 스킬
- 데이터 사이언디스트들은 주로 데이터 처리나 분석 기술과 관련된 (`하드 스킬`)만을 요구 받는 것 처럼 보인다. 하지만 이러한 (`하드 스킬`)은 훌륭한 데이터 사이언티스트가 갖춰야 하는 능력의 절반에 불과하다. 나머지 절반은 통찰력 있는 분석, 설득력 있는 전달, 협력 등 (`소프트 스킬`)이다.
- 하드 스킬
    - 빅데이터에 대한 이론적 지식 : 관련 기법에 대한 이해와 방법론 습득
    - 분석 기술에 대한 숙련 : 최적의 분석 설계 및 노하우 축적
- 소프트스킬
    - 통찰력 있는 분석 : 창의적 사고, 호기심, 논리적 비판
    - 설득력 있는 전달 : 스토리텔링, 시각화(Visualization)
    - 다분야 간 협력 : 커뮤니케이션(Communication)

## 23 가치 패러다임의 변화
- 과거 - 디지털화 Digitalization
    - 아날로그 세상을 어떻게 효과적으로 디지털화하는가
- 현재 - 연결 Connection
    - 디지털화된 정보, 대상들이 서로 연결
    - 이 연결이 얼마나 효과적으로 제고오디는가
- 미래 - 에이전시 Agency
    - 많고 복잡한 연결을 얼마나 효과적이고 신뢰할 수 있도록 관리하는가