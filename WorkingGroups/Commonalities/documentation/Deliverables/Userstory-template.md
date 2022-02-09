# User Story Template
This document specifies the template for documenting user stories related to API families in CAMARA project. 

| Item | Description | Support Qualifier |
|----|----|----|
|Summary| | M |
|Actors and scope|| M |
|NF Requirements|| O |
|Pre-conditions|| M |
|Begins when|| M |
|Step 1|| (M/O/CM) |
|Step 2|| (M/O/CM|
|...|| (M/O/CM) |
|Step N|| (M/O/CM) |
|Ends when|| M |
|Post-conditions|| M |
|Exceptions|| M | 

Some notes related to the above template:
<ul>
  <li> The <b> Support Qualifier </b> column allows capturing the need for specifying the item. <ins>Options -> M (Mandatory); O (Optional); CM (Conditional Mandatory)</ins>. </li>
  <li> The <b> Summary </b> item provides a user story description as a user persona, following the same syntax structure -> "<ins> <b>As a</b> (Persona), <b>I want</b> (Need), <b>so that</b> (Goal)" </ins>.</li>
  <ul>    
    <li> A user story based on <em>user persona</em> focuses on expectations from the point of view of an end-user. This is contrary to a user story based on <em>system persona </em>, which is designed to represent background system functions that do not require interaction from the end-user (i.e., elaborate on the behind-of-the-scenes integration tasks that are not user-centric).</li>
  </ul>
  <li> The <b>Actors and scope</b> item allows linking user story with existing Cloud/NaaS reference architectures. The architectures that are within the scope of CAMARA project are detailed in this document: https://github.com/telekom/telco-global-api-alliance/files/7065771/Reference.Architectures.pptx)
    <ul>    
        <li> Actor: specifies the role(s) that the corresponding CAMARA API customer (e.g., application service provider, hyperscaler, application developer) plays for the user story. <ins>Options -> customer:user; customer:administrator; customer:business manager</ins>. </li>
        <li> Scope: specifies the service lifecycle area(s) that the user story impacts on. <ins>Options -> Design time ; Prospect to Order (P2O); Usage to Cash (U2C); Order to Activate (O2A); Trouble to Resolution (T2R)</ins>. </li>
    </ul>
  </li>
</ul>


# Linking user story to API design
Once we have the user story, the next step is to clarify the <b>data journey</b> in the context of the target and source systems we are integrating:
<ul>
  <li> Think about triggers for workflows: how and when does data need to be moved between the application and the service? </li>
  <li> Think about dependencies of data objects: does the data in underlying objects need to be regularly kept in sync with another system? </li>
   <li> Think about any parameters the user might need to configure or change. This is particularly important when building self- serve integrations for non-technical end users. </li>
</ul>
