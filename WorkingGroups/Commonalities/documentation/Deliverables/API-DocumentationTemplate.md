# API documentation template

| Section | Sub-section | Description | Mandatory | 
|----|---|---|-|
| Overview | Introduction | This section gives an overview of the API. It explains the use of the API and gives an insight on its benifits. A few lines on some standard usecases can help better explain the API  | yes |
|| Quick Start|It explains how developers can get started with this API. A good example is the Stripe-API documentation: https://stripe.com/docs/api ||
|Authentication| |It explains how developers/consumers can authenticate with the API. Failure to document the authentication schema in a simple and precise way can deter first time API users . 	|yes|
|Documentation|Details|This is an optional section/placeholder. It could include some detailed descriptions or diagrams explaining things in further details and the subsection heading could be changed accordingly.| |
| |Endpoint definitions | What does each endpoint do is a critical part of the api documentation. It explains the consumer/developer your internal system. The documentation should explain what an endpoint is for and how it relates to other endpoints. It should also document:</br> - Http call methods supported. </br> - Parameteres along with description </br> - Expected responses </br> If there are any constraints for an endpoint, it should be documented in this section. </br> It should be made clear if certain enpoints are restricted to only certain roles/users. | yes |
|  |Errors|Error types along with error codes summary table can offer a good reference for the developers working with the API | yes |
|  |Code snippets| Copy-paste sample code snippets help developers to get started right away. It helps provide a rich developer experience. This can include sample request examples. |  |
|API Spec || Complete API Spec in yaml format | yes |
