# OIC Interview Questions

###  1. What are the critical components of Oracle Integration Cloud (OIC)?
Oracle OIC comprises several key components, including:

Integration Designer: A visual interface for creating integrations and orchestrations.

Connection Agent: A secure agent that enables connectivity between on-premises applications and OIC.

Integration Cloud Service: Provides pre-built adapters, connectivity, and transformations for various applications and services.

Process Automation: Enables designing, modelling, and automating business processes.

Visual Builder: A low-code development platform for creating custom applications.

###  2. How does OIC handle data transformations and mapping b/w different applications?
OIC offers a visual mapper that allows you to define data transformations between source and target applications using a drag-and-drop interface. It supports the graphical mapping of fields, functions, and transformations, making it easier to align data structures and formats between connected systems.

###  3. Can OIC be used to integrate with non-Oracle applications?
Yes, Oracle Integration Cloud can be used to integrate with a wide range of non-Oracle applications and data sources, including popular cloud applications such as Salesforce and Workday, as well as on-premises systems and custom applications.

###  4. What are Difference between Connection and Adaptor?
Connection is the Starting Point before creating any integration. This is the Place where you specify whether it is an Invoke or Trigger or Both. Connection Always Leverages an Adaptor; it could be an Application Specific or Technology Adaptor. For Instance, ERP cloud, Sales force, Workday adaptors are Application Specific whereas FTP, REST, SOAP are Technology Adaptors.

###  5. What are Different Integration Actions available?
Using integration actions, you can view, Edit, Clone, and Create new Version, Update Property Values*, Export, API Management*, Insight Designer*, Tracing, Configure*

###  6. What is the use of Update Property value Action?
This Action gives the developer an ability to update the design time values outside of the integration. For Instance, In an Email notification activity, you specify an email address to use in the "To" Field during run time which overrides the email address at the design-time. To put it Simply, This option enables you to configure the value without editing the integration design.

###  7. What is the Maximum integration properties can be added?
10 

###  8. In which state the Integration has to be in order to update the properties?
App Driven Orchestration has to be in configured state to update Properties whereas Scheduled Integration supports even if it the integration is active.

###  9. What are different tools available in OIC?
Application Integration, Process Automation, B2B, Visual Builder, Integration Insights.

###  10. What is a File Transfer Pattern?
File Transfer pattern allows to move files across network seamlessly and securely. This is again a scheduled type of pattern.

###  11. What is a Basic Routing Pattern?
Basic Routing pattern can connect only two applications with no logic.

###  12. What is publish to OIC and Subscribe to OIC pattern?
The Publish to OIC pattern allows publishing messages to OIC internal messaging queues. For example, an event is subscribed from Oracle Sales Cloud and Publish the same into Oracle Integration Cloud messaging queue.  

Subscribe to OIC pattern subscribe messages from Oracle Integration Cloud messaging queue and sends the same to different applications  

These queues are managed by OIC itself and you don’t have access of them.

###  13. How does OIC ensure security and data privacy in integrations?
OIC employs various security measures, including:
Secure agent for on-premises connectivity, ensuring data remains within your network.

Role-based access control to manage user permissions.

Encryption of data at rest and in transit.

OAuth and token-based authentication for APIs and connections.

###  14. Can you explain the difference between orchestration and choreography in OIC?
Orchestration: Involves designing a centralized flow where a single component controls the sequence of activities, making decisions and coordinating interactions.

Choreography: Involves a decentralized approach where each participant in the integration knows its role and responsibilities, and interactions are driven by events or triggers.

###  15. How can you monitor and troubleshoot integrations in OIC?
OIC offers monitoring dashboards, logs, and alerts to track integration flows and detect issues. You can view runtime statistics, error details, and performance metrics. Integration Insight provides advanced analytics to identify bottlenecks and optimize processes.


###  16. What is the role of the Connection Agent in Oracle Integration Cloud?
Connection Agent is a lightweight software component that facilitates secure communication between OIC and on-premises applications or data sources. It ensures data integrity, security, and reliable connectivity across hybrid environments.

###  17. Can you explain how OIC supports hybrid integrations?
OIC enables hybrid integrations by using the Connection Agent to securely connect with on-premises systems. This allows organizations to seamlessly integrate cloud and on-premises applications, ensuring data flows smoothly between the two environments.

###  18. How does OIC facilitate application lifecycle management and DevOps?
The OIC supports application lifecycle management by providing versioning, deployment automation, and collaboration features. It integrates with Oracle Developer Cloud Service and supports CI/CD pipelines, allowing teams to manage and deploy integrations using DevOps practices.

Remember, these are sample questions and answers that you can use for reference during your interview preparation. Be sure to study the Oracle Integration Cloud documentation and customize your responses based on your understanding and experience.

###  {==19. How are Versions Handled in OIC?==}
Versions syntax is major. minor. patch
Example: 01.00.0001 – Initial Version
     01.01.0001-New Major Version
     01.01.0002- New Patch Version
Creating and activating a new minor or patch version over an existing version will result in this new version of the integration be the active version. There can be only one version of an integration flow with same major version active at any time. Major versions can run Side by Side.

###  {==320. What is the Difference between Rest and SOAP API?==}
In a service interface, one can use SOAP to expose an application’s business logic to a server, whereas REST uses URIs. REST APIs are designed around data, whereas SOAP APIs are designed around functions. You can include a function like “CreateUser” in a SOAP API that allows creating a user. This function would be a part of the SOAP body.

REST is a data-driven architecture, whereas SOAP is a standard protocol for transmitting structured data that is more function-driven. Unlike SOAP, which only allows the use of XML, REST allows the use of a wide variety of data types, including plain text, HTML, XML, and JSON. The only options for SOAP APIs are XML and the format of the SOAP is called envelope which contains header and body. REST APIs, on the other hand, is format independent. Although JSON is the most popular option, XML, plain text, and XML are all suitable formats for REST APIs.

###  21. What is Opaque Schema?
No need to worry about the file’s schema while performing Read File or Write File operations with an opaque schema. This is the only requirement: Base64-encoded data should be available to the opaque element. The Opaque schema is needed in OIC especially when you need to write a Bse64-encoded data using stage file to extract it into a structured variable. For example, when BIP report is run using Report Service in OIC the response will be always in Base64-encoded data. In order to extract that report response into a structured variable, which will enable to refer the individual elements there is a need to write it using stage file and read back using sample data as per the requirement. The stage file write operation does not have an option to write without structure, in that case Opaque schema can be used.

###  22. What is iCal Expression?
ICal Expressions in OIC is used for defining Complex Scheduling for Scheduled Integration

With default scheduling options we will be only able to Schedule the integration with below options.

Hours and Minutes

Days

Weeks

Months

If there is any requirement to schedule the integration apart the above standard options then we might need to use iCal expression.

FREQ=MONTHLY;BYMONTHDAY=1,10,15;BYHOUR=5,10,15,20;BYMINUTE=15;

This iCal expression indicates that this integration runs each month on the 1st, 10th, and 15th days of the month at 5:15 AM,10:15 AM, 3:15 PM , and 8:15 PM.

<b>Requirement:</b> Schedule an integration from Sunday to Thursday 8 AM to 8PM for every 30 minutes for 1 years

 How do we solve:

FREQ=WEEKLY; INTERVAL=54; BYDAY=SU,MO,TU,WE,TH; BYHOUR=8,9,10,11,12,13,14,15,16,17,18,19,20; BYMINUTE=0,30;