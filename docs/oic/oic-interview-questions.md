# OIC Interview Questions

<pre><code class="shell">1. What is Oracle Integration Cloud (OIC)?</code></pre>
Ans: Oracle Integration Cloud (OIC) is a cloud-based integration platform offered by Oracle that allows organizations to connect applications, services, and data sources seamlessly across cloud and on-premises environments. It facilitates integration, process automation, and the visual design of workflows.


<pre><code class="shell">2. What are the critical components of Oracle Integration Cloud (OIC)?</code></pre>
Ans: Oracle OIC comprises several key components, including:

Integration Designer: A visual interface for creating integrations and orchestrations.

Connection Agent: A secure agent that enables connectivity between on-premises applications and OIC.

Integration Cloud Service: Provides pre-built adapters, connectivity, and transformations for various applications and services.

Process Automation: Enables designing, modelling, and automating business processes.

Visual Builder: A low-code development platform for creating custom applications.

<pre><code class="shell">3. How does OIC handle data transformations and mapping between different applications?</code></pre>
Ans: OIC offers a visual mapper that allows you to define data transformations between source and target applications using a drag-and-drop interface. It supports the graphical mapping of fields, functions, and transformations, making it easier to align data structures and formats between connected systems.

<pre><code class="shell">4. What is Oracle Integration Cloud (OIC)?</code></pre>
Ans: Oracle Integration Cloud (OIC) is a cloud-based integration platform offered by Oracle that allows organizations to connect applications, services, and data sources seamlessly across cloud and on-premises environments. It facilitates integration, process automation, and the visual design of workflows.


<pre><code class="shell">5. What are Difference between Connection and Adaptor?</code></pre>
Ans: Connection is the Starting Point before creating any integration. This is the Place where you specify whether it is an Invoke or Trigger or Both. Connection Always Leverages an Adaptor; it could be an Application Specific or Technology Adaptor. For Instance, ERP cloud, Sales force, Workday adaptors are Application Specific whereas FTP, REST, SOAP are Technology Adaptors.

<pre><code class="shell">6. What are Different Types of Integrations are Available?</code></pre>
Ans: App Driven Orchestration, Scheduled Orchestration, File Transfer, Basic Routing, Publish to OIC, Subscribe to OIC

<pre><code class="shell">7. What is a package in the OIC?</code></pre>
Ans: Packages gives a convenient way to Group Similar kind of Integrations into one Package. This is very help full at the time of deployment. Instead of individual integrations deployment, we can simply deploy the respective package to target instance. 

<pre><code class="shell">8. What are Different Integration Actions available?</code></pre>
Ans: Using integration actions, you can view, Edit, Clone, and Create new Version, Update Property Values*, Export, API Management*, Insight Designer*, Tracing, Configure*

<pre><code class="shell">9. What is the use of Update Property value Action?</code></pre>
Ans: This Action gives the developer an ability to update the design time values outside of the integration. For Instance, In an Email notification activity, you specify an email address to use in the "To" Field during run time which overrides the email address at the design-time. To put it Simply, This option enables you to configure the value without editing the integration design.

<pre><code class="shell">10. What is the Maximum integration properties can be added?</code></pre>
Ans: 10 

<pre><code class="shell">11. In which state the Integration has to be in order to update the properties?</code></pre>
Ans: App Driven Orchestration has to be in configured state to update Properties whereas Scheduled Integration supports even if it the integration is active.

<pre><code class="shell">12. What are Agents?</code></pre>
Ans: When you need to integrate with an application behind firewall, you need to configure the agent on the Server where the application is installed .OIC Connectivity agent registers with oracle integration over SSL using the provided oracle integration credentials.

<pre><code class="shell">13. What are OIC Lookups?</code></pre>
Ans: Lookups help you to configure the static values and use them at run time, eliminates the need of hardcoding the same at the mapping level.

<pre><code class="shell">14. What are different tools available in OIC?</code></pre>
Ans: Application Integration, Process Automation, B2B, Visual Builder, Integration Insights.

<pre><code class="shell">15. What is App Driven Orchestration pattern?</code></pre>
Ans: App Driven Orchestration pattern is the multi-step pattern, allows invoking multiple applications in a single flow, doing a for-each loop, if-else logic, apply complex logic, etc. 

<pre><code class="shell">16. What is Scheduled Orchestration Pattern?</code></pre>
Ans: Scheduled Orchestration pattern allows you to develop an integration that can run on the pre-defined frequency and can be executed on an Adhoc basis.

<pre><code class="shell">17. What is a File Transfer Pattern?</code></pre>
Ans: File Transfer pattern allows to move files across network seamlessly and securely. This is again a scheduled type of pattern.

<pre><code class="shell">18. What is a Basic Routing Pattern?</code></pre>
Ans: Basic Routing pattern can connect only two applications with no logic.

<pre><code class="shell">19. What is publish to OIC and Subscribe to OIC pattern?</code></pre>
Ans: The Publish to OIC pattern allows publishing messages to OIC internal messaging queues. For example, an event is subscribed from Oracle Sales Cloud and Publish the same into Oracle Integration Cloud messaging queue.  

Subscribe to OIC pattern subscribe messages from Oracle Integration Cloud messaging queue and sends the same to different applications  

These queues are managed by OIC itself and you don’t have access of them.

<pre><code class="shell">20. How does OIC ensure security and data privacy in integrations?</code></pre>
Ans: OIC employs various security measures, including:
Secure agent for on-premises connectivity, ensuring data remains within your network.

Role-based access control to manage user permissions.

Encryption of data at rest and in transit.

OAuth and token-based authentication for APIs and connections.

<pre><code class="shell">21. Can you explain the difference between orchestration and choreography in OIC?</code></pre>
Ans: Orchestration: Involves designing a centralized flow where a single component controls the sequence of activities, making decisions and coordinating interactions.

Choreography: Involves a decentralized approach where each participant in the integration knows its role and responsibilities, and interactions are driven by events or triggers.

<pre><code class="shell">22. How can you monitor and troubleshoot integrations in OIC?</code></pre>
Ans: OIC offers monitoring dashboards, logs, and alerts to track integration flows and detect issues. You can view runtime statistics, error details, and performance metrics. Integration Insight provides advanced analytics to identify bottlenecks and optimize processes.


<pre><code class="shell">23. What is the role of the Connection Agent in Oracle Integration Cloud?</code></pre>
Ans: Connection Agent is a lightweight software component that facilitates secure communication between OIC and on-premises applications or data sources. It ensures data integrity, security, and reliable connectivity across hybrid environments.

<pre><code class="shell">24. Can you explain how OIC supports hybrid integrations?</code></pre>
Ans: OIC enables hybrid integrations by using the Connection Agent to securely connect with on-premises systems. This allows organizations to seamlessly integrate cloud and on-premises applications, ensuring data flows smoothly between the two environments.

<pre><code class="shell">25. How does OIC facilitate application lifecycle management and DevOps?</code></pre>
Ans: The OIC supports application lifecycle management by providing versioning, deployment automation, and collaboration features. It integrates with Oracle Developer Cloud Service and supports CI/CD pipelines, allowing teams to manage and deploy integrations using DevOps practices.

Remember, these are sample questions and answers that you can use for reference during your interview preparation. Be sure to study the Oracle Integration Cloud documentation and customize your responses based on your understanding and experience.

<pre><code class="shell">26. How are Versions Handled in OIC?</code></pre>
Ans: Versions syntax is major. minor. patch
Example: 01.00.0001 – Initial Version
     01.01.0001-New Major Version
     01.01.0002- New Patch Version
Creating and activating a new minor or patch version over an existing version will result in this new version of the integration be the active version. There can be only one version of an integration flow with same major version active at any time. Major versions can run Side by Side.




