# How To Ace The AWS Solutions Architect Interview (Technical) by Tech with Lucy (Youtube)
Source: https://youtube.com/watch?v=Iuua4b-pF0w&si=EnSIkaIECMiOmarE

## Q. What is your current understanding of the Solutions Architect role?
<details>
<summary>
Answer - Korean</summary>
<div markdown="1">
솔루션즈 아키텍트는 고객들이 클라우드 서비스를 더욱 효율적으로 사용할 수 있게 도와주는 역할을 합니다.
고객들에게 클라우드 전략을 소개하고 현재 비즈니스 요구 사항과 향후 예상되는 요구 사항을 충족하도록 AWS 서비스를 통합하는 솔루션 설계하고 개발 클라우드 전환 업무를 지원하는 역할들을 수행합니다.
기술적으로 확고한 클라우드 지식을 가지고 고객들과 함께 소통하여 최상의 솔루션을 제공하는 것을 목표로 합니다.
<br>
</div>
</details>

## Q. Can you explain the benefits of Cloud Computing?
<details>
<summary>
Answer - Korean</summary>
<div markdown="1">
클라우드 컴퓨팅은 IT 리소스(서버 및 네트워크 등)를 인터넷으로 빌려주는 서비스입니다. 
직접 리소스를 조달하거나 구성, 관리할 필요가 없이 AWS, Google Cloud, Azure 등과 같은 클라우드 공급자로부터 컴퓨팅 파워, 스토리지, 데이터베이스와 같은 기술 서비스에 액세스 가능하고 사용한 만큼만 비용을 지불하면 됩니다. <br>
클라우드 컴퓨팅의 장점으로는

**민첩성**(클라우드를 통해 여러 기술에 쉽고 빠르게 액세스 가능), <br>
**탄력성**(비즈니스 요구가 변화함에 따라 리소스, 용량 확장과 축소가 용이), <br>
**비용 절감**(클라우드를 통해 고정 비용(데이터 센터, 물리적 서버 등) 감소, 규모의 경제), <br>
**몇분 만에 전 세계로 배포 가능한 점**(클라우드를 사용하면 몇 분 만에 새로운 지리적 리전으로 확장하고 전 세계에 배포 가능)이 있습니다.

<br>
Tip: The on-demand delivery of IT resources over the internet with a pay-as-you-go model <br>
Benefits: <br>
- Agility  <br>
- Elasticity  <br>
- Cost savings  <br>
- Deploy globally in minutes <br>
</div>
</details>

## Q. What is the difference between a SQL database and a NoSQL database? (duplicate)
<details>
<summary>
Answer - Korean</summary>
<div markdown="1">
데이터베이스(DBMS)는 관계형 데이터베이스(SQL DB)와 그 나머지(NoSQL DB)로 분류 가능합니다. 
관계형 데이터베이스와 상호작용할 때 SQL를 사용하면 SQL DB이고 그것이 아니면 NoSQL DB 입니다.<br>
 
**SQL DB**는 데이터를 행과 열이 있는 표형태로 저장합니다. (가장 많이 사용되는 데이터베이스의 유형입니다.)
테이블의 구조와 데이터 타입 등을 사전에 정의합니다. 그리고 테이블에 정의된 내용(스키마(Schema)라는 틀)에 알맞은 형태의 데이터만 삽입할 수 있습니다. 특정한 형식을 지키기 때문에, 데이터를 정확히 입력했다면 데이터를 사용할 때에는 매우 수월합니다.
대표적 제품으로는 MySQL, PostgreSQL, Oracle DB이 있습니다.<br>

**SQL DB 장점**<br>
 - 명확하게 정의된 스키마, 데이터 무결성 보장<br>
 - 관계는 각 데이터를 중복없이 한번만 저장<br>
  
**SQL DB 단점**<br>
 - 덜 유연함. 데이터 스키마를 사전에 계획하고 알려야 함.(나중에 수정하기 힘듬)<br>
 - 관계를 맺고 있어서 조인문이 많은 복잡한 쿼리가 만들어질 수 있음<br>
 - 대체로 수직적 확장만 가능함<br>

**NoSQL DB**는 스키마가 정해진 것이 아니어서 유연성, 확장성 측면에서 더 효과적입니다. 
유연한 스키마를 제공하며, 대량의 데이터와 높은 사용자 부하에서도 손쉽게 확장이 가능
SQL DB가 아닌 모든 것을 말하는 것으로 종류가 다양합니다. 대표적으로 Key-Value, Document, Graph이 있습니다. <br>

 - Key-Value :  Key와 Value 형태로 데이터 저장합니다. 가장 단순한 형태의 데이터베이스 그러므로 가장 빠릅니다. 캐시, 세션 관리, 실시간 분석 등에 주로 사용됩니다. <br>
  대표적인 제품: redis, amazon DynamoDB <br>
 - Document: Key 와 Document (like JSON)의 형태로 데이터 저장합니다. JSON의 형태라 스키마가 변하는데 유연하게 대처 가능합니다.<br>
  대표적인 제품: Amazon DocumentDB, MongoDB<br>
- Graph:  노드의 속성별로 데이터를 저장합니다. 페이스북과 같은 소셜네트워크, 추천엔진을 위한 데이터베이스에 사용됩니다. <br>
  대표적인 제품: Amazon Neptune, neo4j<br>

**NoSQL 장점**<br>
 - 스키마가 없어서 유연함. 언제든지 저장된 데이터를 조정하고 새로운 필드 추가 가능<br>
 - 데이터는 애플리케이션이 필요로 하는 형식으로 저장됨. 데이터 읽어오는 속도 빨라짐<br>
 - 수직 및 수평 확장이 가능해서 애플리케이션이 발생시키는 모든 읽기/쓰기 요청 처리 가능<br>

**NoSQL 단점**<br>
 - 유연성으로 인해 데이터 구조 결정을 미루게 될 수 있음<br>
 - 데이터 중복을 계속 업데이트 해야 함<br>
 - 데이터가 여러 컬렉션에 중복되어 있기 때문에 수정 시 모든 컬렉션에서 수행해야 함 (SQL에서는 중복 데이터가 없으므로 한번만 수행이 가능)<br>

**❗️SQL 데이터베이스와 NoSQL 데이터베이스 차이점**
 - 데이터 저장(Storage) <br>
NoSQL은 key-value, document, wide-column, graph 등의 다양한 방식으로 데이터를 저장합니다. <br>
관계형 데이터베이스는 SQL을 이용해서 데이터를 테이블에 저장합니다. 미리 작성된 스키마를 기반으로 정해진 형식에 맞게 데이터를 저장해야 합니다. <br>
 - 스키마(Schema) <br>
SQL을 사용하려면, 고정된 형식의 스키마가 필요합니다.
다시 말해, 처리하려는 데이터 속성별로 열(column)에 대한 정보를 미리 정해두어야 한다.
스키마는 나중에 변경할 수 있지만, 이 경우 데이터베이스 전체를 수정하거나 오프라인(down-time)으로 전환할 필요가 있습니다. <br>
NoSQL은 관계형 데이터베이스보다 동적으로 스키마의 형태를 관리할 수 있습니다.
행을 추가할 때 즉시 새로운 열을 추가할 수 있고, 개별 속성에 대해서 모든 열에 대한 데이터를 반드시 입력하지 않아도 됩니다. <br>
 - 쿼리(Querying) <br>
쿼리는 데이터베이스에 대해서 정보를 요청하는 질의문입니다.
관계형 데이터베이스는 테이블의 형식과 테이블간의 관계에 맞춰 데이터를 요청해야 합니다.
그래서 정보를 요청할 때, SQL과 같이 구조화된 쿼리 언어를 사용합니다. <br>
비관계형 데이터베이스의 쿼리는 데이터 그룹 자체를 조회하는 것에 초점을 두고 있습니다.
그래서 구조화 되지 않은 쿼리 언어로도 데이터 요청이 가능합니다.
UnQL(UnStructured Query Language)이라고 말하기도 한다. <br>
 - 확장성(Scalability) <br>
일반적으로 SQL 기반의 관계형 데이터베이스는 **수직적으로** 확장합니다.
높은 메모리, CPU를 사용하는 확장이라고도 합니다.
데이터베이스가 구축된 하드웨어의 성능을 많이 이용하기 때문에 비용이 많이 듭니다.
여러 서버에 걸쳐서 데이터베이스의 관계를 정의할 수 있지만, 매우 복잡하고 시간이 많이 소모됩니다.  <br>
NoSQL로 구성된 데이터베이스는 **수평적으로** 확장합니다.
보다 값싼 서버 증설, 또는 클라우드 서비스 이용하는 확장이라고도 합니다.
NoSQL 데이터베이스를 위한 서버를 추가적으로 구축하면, 많은 트래픽을 보다 편리하게 처리할 수 있습니다.
그리고 저렴한 범용 하드웨어나 클라우드 기반의 인스턴스에 NoSQL 데이터베이스를 호스팅할 수 있어서, 수직적 확장보다 상대적으로 비용이 저렴합니다. 

<br>

**❗️ SQL 기반의 관계형 데이터베이스를 사용하는 케이스**<br>
1. 데이터베이스의 ACID 성질을 준수해야 하는 경우  <br>
 - ACID: Atomicity(원자성), Consistency(일관성), Isolation(격리성), Durability(지속성) <br>
 - 각 단어는 데이터베이스에서 실행되는 하나의 트랜잭션(Transaction)에 의한 상태의 변화를 수행하는 과정에서, 안전성을 보장하기 위해 필요한 성질입니다. <br>
 - SQL을 사용하면 데이터베이스와 상호 작용하는 방식을 정확하게 규정할 수 있기 때문에, 데이터베이스에서 데이터를 처리할 때 발생할 수 있는 예외적인 상황을 줄이고, 데이터베이스의 무결성을 보호할 수 있습니다. <br>
 - 전자 상거래를 비롯한 모든 금융 서비스를 위한 소프트웨어 개발 에서는 반드시 데이터베이스의 ACID 성질을 준수해야 합니다. <br>
2. 소프트웨어에 사용되는 데이터가 구조적이고 일관적인 경우 <br>
 - 소프트웨어(프로젝트)의 규모가 많은 서버를 필요로 하지 않고 일관된 데이터를 사용하는 경우, 관계형 데이터베이스를 사용하는 경우가 많습니다. <br>
 - 다양한 데이터 유형과 높은 트래픽을 지원하도록 설계된 NoSQL 데이터베이스를 사용해야만 하는 이유가 없기 때문입니다.<br>

**❗️ NoSQL 기반의 비관계형 데이터베이스를 사용하는 케이스**<br>
1. 데이터의 구조가 거의 또는 전혀 없는 대용량의 데이터를 저장하는 경우 <br>
 - 대부분의 NoSQL 데이터베이스는 저장할 수 있는 데이터의 유형에 제한이 없습니다. <br>
 - 필요에 따라, 언제든지 데이터의 새 유형을 추가할 수 있습니다. <br>
 - 소프트웨어 개발에 정형화 되지 않은 많은 양의 데이터가 필요한 경우, NoSQL을 적용하는 것이 더 효율적일 수 있습니다. <br>
2. 클라우드 컴퓨팅 및 저장공간을 최대한 활용하는 경우 <br>
 - 클라우드 기반으로 데이터베이스 저장소를 구축하면, 저렴한 비용의 솔루션을 제공받을 수 있습니다. <br>
 - 소프트웨어에 데이터베이스의 확장성이 중요하다면, 별다른 번거로움 없이 확장할 수 있는 NoSQL 데이터베이스를 사용하는 것이 좋습니다. <br>
3. 빠르게 서비스를 구축하는 과정에서 데이터 구조를 자주 업데이트 하는 경우 <br>
 - NoSQL 데이터베이스의 경우 스키마를 미리 준비할 필요가 없기 때문에 빠르게 개발하는 과정에 매우 유리합니다. <br>
 - 시장에 빠르게 프로토타입을 출시해야 하는 경우가 이에 해당합니다. <br>
 - 또한 소프트웨어 버전별로 많은 다운타임(데이터베이스 서버를 오프라인으로 전환하여 데이터 처리를 진행하는 작업 시간) 없이 데이터 구조를 자주 업데이트 해야하는 경우, 스키마를 매번 수정해야 하는 관계형 데이터베이스 보다 NoSQL 기반의 비관계형 데이터베이스를 사용하는 게 더 적합합니다. <br>

Source: 
<br>
https://hanamon.kr/데이터베이스-sql-vs-nosql/
<br>
https://velog.io/@swhan9404/NoSQL-의-종류별-특징
</div>
</details>

## Q. How do you secure your 3-tier web application in the cloud?
<details>
<summary>
Answer - WIP</summary>
<div markdown="1">
- Networking best practices  <br>
- Data protection <br>
- Identity and access management  <br>
</div>
</details>

## Q. Give me an example of how you might use machine learning to enhance a product or bring benefit to a company.
<details>
<summary>
Answer - WIP</summary>
<div markdown="1">
e.g. You run an E-Commerce Website <br>
Once custoner buys something, they get recommended with other products to buy ... <br>
--> Based on the purchase history of similar shoppers  <br>
</div>
</details>

## Q. How do you scale your application for a big traffic day?
<details>
<summary>
Answer - WIP</summary>
<div markdown="1">
</div>
</details>


## Q. What happens behind the scenes when you hit enter on website URL, e.g. google.com?
<details>
<summary>
Answer - WIP</summary>
<div markdown="1">
</div>
</details>

## Q. What is the difference between IaaS, PaaS, SaaS?
<details>
<summary>
Answer - WIP</summary>
<div markdown="1">
</div>
</details>

## Q. What are containers?
<details>
<summary>
Answer - WIP</summary>
<div markdown="1">
</div>
</details>

## Q. How do you migrate an application from on-premises to the cloud?

<details>
<summary>
Answer - WIP</summary>
<div markdown="1">
</div>
</details>
