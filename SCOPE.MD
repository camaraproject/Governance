## Functional scope:
From functional perspective the scope is limited to telco APIs, that means APIs in the domain of telco mobile networks, telco fixed line networks or supporting these (e.g. for authentication). The respective API families are clarified during the ramp up of the Telco Global API project, specifically the ones exposed to customers.

## Technical scope:
Technically the scope is about northbound Service APIs, that means an abstraction / aggregation of e.g. 3GPP APIs or TM Forum APIs to hide telco complexity, keep control at the operator side and fulfill regulatory and data privacy constraints. Optionally in scope are east-/westbound APIs on the same abstraction / aggregation level.
![ServiceAPI Architecture](/documentation/ressources/ServiceAPI_Architecture.jpg)

## Service scope:
The service scope of the Telco Global API project is limited to the following activities:
-	Collect API requirements from GSMA OPG subgroup and other sources. That can be a (prioritized) list of API families seen as useful for the customers, a functional descriptions of the APIs (attributes, function, result), and also non-functional requirements for the APIs (response time, scalability, performance, etc.)
-	Specify Service APIs (e.g. by Swagger) and create test cases / tools from a business and customer perspective
-	Implement Service APIs (reference implementation)
-	Create test cases and perform verification/tests from developer perspective (to show that the Service API has been implemented correctly)
-	Create documentation for Service APIs
-	Test Service APIs from business/customer perspective (validation) in telco network(s)
-	Create deployment packages for Service APIs
-	Create a reference architecture for Service APIs (if possible preferred solution is to refer to an existing architecture)

## Deliverables:
The following deliverables are provided by the Telco Global API project:
-	Service API code and documentation and
-	Test cases and tools

both contained in deployment packages. In addition a
-	Reference architecture for Service APIs

