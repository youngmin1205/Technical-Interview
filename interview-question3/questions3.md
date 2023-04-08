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
관계형 데이터베이스와 상호작용할 때 SQL를 사용하면 SQL DB이고 그것이 아니면 NoSQL DB 입니다. 

<br>

**SQL DB**는 데이터를 행과 열이 있는 표형태로 저장합니다. (가장 많이 사용되는 데이터베이스의 유형입니다.)
스키마(Schema)라는 틀에 맞추어 데이터가 저장되어 체계적, 안정적으로 관리 가능합니다. 대표적 제품으로는 MySQL, PostgreSQL, Oracle DB이 있습니다.<br>

**SQL DB 장점**<br>
 - 명확하게 정의된 스키마, 데이터 무결성 보장<br>
 - 관계는 각 데이터를 중복없이 한번만 저장<br>
  
**SQL DB 단점**<br>
 - 덜 유연함. 데이터 스키마를 사전에 계획하고 알려야 함.(나중에 수정하기 힘듬)<br>
 - 관계를 맺고 있어서 조인문이 많은 복잡한 쿼리가 만들어질 수 있음<br>
 - 대체로 수직적 확장만 가능함<br>

**SQL 데이터베이스 사용이 더 좋을 때**<br>
- 관계를 맺고 있는 데이터가 자주 변경되는 애플리케이션의 경우<br>
- NoSQL에서는 여러 컬렉션을 모두 수정해야 하기 때문에 비효율적<br>
- 변경될 여지가 없고, 명확한 스키마가 사용자와 데이터에게 중요한 경우<br>

**NoSQL DB**는 스키마가 정해진 것이 아니어서 유연성, 확장성 측면에서 더 효과적입니다. SQL DB가 아닌 모든 것을 말하는 것으로 종류가 다양합니다. 대표적으로 Key-Value, Document, Graph이 있습니다. <br>

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

**NoSQL 데이터베이스 사용이 더 좋을 때**<br>
 - 정확한 데이터 구조를 알 수 없거나 변경/확장 될 수 있는 경우<br>
 - 읽기를 자주 하지만, 데이터 변경은 자주 없는 경우<br>
 - 데이터베이스를 수평으로 확장해야 하는 경우 (막대한 양의 데이터를 다뤄야 하는 경우)<br>

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