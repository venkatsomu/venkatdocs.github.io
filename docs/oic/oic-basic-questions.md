# OIC Basic Interview Questions

###  1. What is Oracle Integration Cloud (OIC)?
Oracle Integration Cloud (OIC) is a cloud-based integration platform offered by Oracle that allows organizations to connect applications, services, and data sources seamlessly across cloud and on-premises environments. It facilitates integration, process automation, and the visual design of workflows.

###  2. What are Different Types of Integrations are Available?
App Driven Orchestration, Scheduled Orchestration, File Transfer, Basic Routing, Publish to OIC, Subscribe to OIC.

###  3. What is App Driven Orchestration?
It enables you to create an integration that uses an event or business object to trigger the integration. In laymen's terms  - you have to pass some inputs to trigger the app driven orchestration integrations.

###  4. What is Scheduled Orchestration?
It enables you to create an integartion that uses a schedule to trigger the integration instead of an adapter. After designing such integration, you can schedule when to run it.

Scheduled integration support runtime runtime configuration. Therefore, you can update the integration property value when the integration is active. But App driven orchestration do not support runtime configuration. Therefore, you can update the integration property value when the integration is not active. 

###  5. What are Packages?
You can group one or more Similar integrations into a single structure called a package to easily import and export them to and from OIC service. This is very help full at the time of deployment. Instead of individual integrations deployment, we can simply deploy the respective package to target instance. Packages being optional, integration do not be a part of them. At least one integration is needed for a package to exist.

###  6. What is Logger?
It Enables you to add log messages to the activity stream and diagnostic logs.

###  7. What is Notification?
Enables you to send notification email to relevant users at specific points in the execution of an integration.

The total size limit on a notification email is 1 MB for Oracle Integration and 2 MB for Oracle Integration Generation 2.

###  8. What is Assign?
Enables you to assign variables to integrations.

###  9. What is ForEach?
Enables you to loop over a repeating element and execute one more actions within the scope of the for-each action.

###  10. What is Map?
It Enables you to add ad-hoc mappers to the integration.

###  11. What is Connection?
A Connection is based on an Adapter that allows Oracle Integration to interact with Oracle application instances. For every application instance that participates in integration, a connection is required. In simple words, it is a connector that is utilized for communicating with various external applications. 

###  12. Difference between Trigger & Invoke ?
Trigger ( source connection ) - For request sent to OIC service

Invoke ( target connection ) - For requests sent from OIC Service to the target.

###  13. What are Agents?
When you need to integrate with an application behind firewall, you need to configure the agent on the Server where the application is installed .OIC Connectivity agent registers with oracle integration over SSL using the provided oracle integration credentials.

###  14. What are OIC Lookups?
Lookups help you to configure the static values and use them at run time, eliminates the need of hardcoding the same at the mapping level.

###  15. FTP Adapter?
Using the FTP Adapter, Oracle Integration Cloud Service can retrieve files for processing in Oracle Integration Cloud Service and upload files and messages from Oracle Integration Cloud Service to a directory on a remote FTP server.

###  16. Assigning Business Identifiers for Tracking Fields ?
Business identifiers enable you to track payload fields in messages during runtime.You must assign business identifiers before you can activate an integration.