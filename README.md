# AZ900 - Exam Preparation

Knowledge trail: https://docs.microsoft.com/en-us/learn/certifications/exams/az-900.

## Microsoft Azure Fundamentals: Describe core Azure concepts

### Introduction to Azure fundamentals

#### Introduction

- Cloud computing platform
- Build solutions to meet your business goals
- In this module, you'll take an entry-level, end-to-end look at Azure and its capabilities

#### What is Azure fundamentals?

- Série de seis roteiros de aprendizagem
- Ajudam você a se familiarizar com o Azure e seus diversos serviços e recursos

##### Why should I take Azure fundamentals?

###### Preparation for Exam AZ-900

Exame inclui seis áreas de domínio de conhecimento:

| AZ-900 Domain Area                                              | Weight |
| --------------------------------------------------------------- | ------ |
| Describe cloud concepts                                         | 20-25% |
| Describe core Azure services                                    | 15-20% |
| Describe core solutions and management tools on Azure           | 10-15% |
| Describe general security and network security features         | 10-15% |
| Describe identity, governance, privacy, and compliance features | 20-25% |
| Describe Azure cost management and Service Level Agreements     | 10-15% |

#### What is cloud computing?

- Delivery of computing services over the internet
- Services = servers, storage, databases, networking, software, analytics, and intelligence
- Compute power = how much processing your computer can deliver
- Storage = amount of data that can be stored on your computer

#### Why is cloud computing typically cheaper to use?

- Cloud computing is the delivery of computing services over the Internet using a pay-as-you-go pricing model
- You only pay for the cloud services you use, which helps:
  - Reduce operating costs
  - Run infrastructure more efficiently
  - Scale operations according to business needs
- The cloud provider is responsible for maintaining the underlying infrastructure for you

#### Why should I move to the cloud?

- Two current trends:
  - Teams deliver new features to users in record time
  - Users expect an increasingly sophisticated and immersive experience across their devices and software.
- Weekly or daily releases

#### What is Azure?

- Tipos de serviços:

  - SAAS
  - PAAS
  - IAAS

- VMs
- Cloud Base Storage
  - Store application or backup safely
- Escalable hosting platforms
  - Azure Web Apps
    - Deploy, operate and scale app
  - Azure Functions
    - Event driven, serverless application, with no coding required
  - Azure Container Instances and Azure Kubernetes Service
    - Deploy containerized applications with fully managed services
- Fully managed relational and in-memory databases, spanning proprietary and open source engines
- Microsoft Cosmos DB
  - Support for several popular NoSQL APIs
- Azure Artificial Inteligence and Machine Learing services

  - Empower developers and data scientists
  - Wide range productive experiences for building, training and deploying machine learing models faster

- Azure's regional data centers allow you to ditribute your applications globally so you can locate your data in apps where they're needed most
- Azure Portal lets you create, configure and control all your services and resources from a single easy to use web-based interface

#### How does Azure work?

- Azure uses a technology known as virtualization
- Virtualization separates the tight coupling between a computer's hardware (HW) and its operating system using an abstraction layer called a hypervisor
- The **hypervisor** emulates all the functions of a real computer and its CPU in a virtual machine
- Each **data center** has mini racks filled with servers
- Each **server** includes a hypervisor to run multiple virtual machines
- **Network switch** provides connectivity to all those servers
- One server in each rack runs a special piece of SW called **fabric controller**
- Each **fabric controller** is connected to another special piece of SW known as **Orchestrator**
- **Orchestrator** is responsible for managing everything that happens in Azure:
  - Responding to user requests
- User's make requests using the **Orchestrator's Web API**
  - Can be called by the user interface (UI) of the Azure Portal

#### What is the Azure Portal?

- Web-based, unified console that provides an alternative to command-line tools
- Manage your Azure subscription by using a graphical user interface
  - Build, manage, and monitor everything from simple web apps to complex cloud deployments
  - Create custom dashboards for an organized view of resources
  - Configure accessibility options for an optimal experience
- Designed for resiliency and continuous availability
  - Maintains a presence in every Azure datacenter
  - Resilient to individual datacenter failures and avoids network slowdowns by being close to users
  - Requires no downtime for maintenance activitie

#### What is Azure Marketplace?

- Customers can find, try, purchase, and provision applications and services from hundreds of leading service providers
- All solutions and services are certified to run on Azure

#### Tour of Azure Services

##### Azure Services

![Azure Services big-picture](https://docs.microsoft.com/en-us/learn/azure-fundamentals/intro-to-azure-fundamentals/media/azure-services-6c41a736.png)

###### Compute

Range of options for hosting applications and services.

Some examples of compute services in Azure:

| Service Name                     | Service Function                                                         |
| -------------------------------- | ------------------------------------------------------------------------ |
| Azure Virtual Machines           | Windows or Linux virtual machines (VMs) hosted in Azure                  |
| Azure Virtual Machine Scale Sets | Scaling for Windows or Linux VMs hosted in Azure                         |
| Azure Kubernetes Service         | Cluster management for VMs that run containerized services               |
| Azure Service Fabric             | Distributed systems platform that runs in Azure or on-premises           |
| Azure Batch                      | Managed service for parallel and high-performance computing applications |
| Azure Container Instances        | Containerized apps run on Azure without provisioning servers or VMs      |
| Azure Functions                  | An event-driven, serverless compute service                              |

###### Networking

Linking compute resources and providing access to applications is the key of Azure networking.

Connect the outside world to services and features in the global Azure datacenters.

Some examples of networking services in Azure:

| Service name                   | Service function                                                                     |
| ------------------------------ | ------------------------------------------------------------------------------------ |
| Azure Virtual Network          | Connects VMs to incoming virtual private network (VPN) connections                   |
| Azure Load Balancer            | Balances inbound and outbound connections to applications or service endpoints       |
| Azure Application Gateway      | Optimizes app server farm delivery while increasing application security             |
| Azure VPN Gateway              | Accesses Azure Virtual Networks through high-performance VPN gateways                |
| Azure DNS                      | Provides ultra-fast DNS responses and ultra-high domain availability                 |
| Azure Content Delivery Network | Delivers high-bandwidth content to customers globally                                |
| Azure DDoS Protection          | Protects Azure-hosted applications from distributed denial of service (DDOS) attacks |
| Azure Traffic Manager          | Distributes network traffic across Azure regions worldwide                           |
| Azure ExpressRoute             | Connects to Azure over high-bandwidth dedicated secure connections                   |
| Azure Network Watcher          | Monitors and diagnoses network issues by using scenario-based analysis               |
| Azure Firewall                 | Implements high-security, high-availability firewall with unlimited scalability      |
| Azure Virtual WAN              | Creates a unified wide area network (WAN) that connects local and remote sites       |

###### Storage

Four main types of storage services:

| Service name        | Service function                                                                                                                                                                   |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Azure Blob storage  | Storage service for very large objects, such as video files or bitmaps                                                                                                             |
| Azure File storage  | File shares that can be accessed and managed like a file server                                                                                                                    |
| Azure Queue storage | A data store for queuing and reliably delivering messages between applications                                                                                                     |
| Azure Table storage | Table storage is a service that stores non-relational structured data (also known as structured NoSQL data) in the cloud, providing a key/attribute store with a schemaless design |

These services all share several common characteristics:

- **Durable** and highly available with redundancy and replication
- **Secure** through automatic encryption and role-based access control
- **Scalable** with virtually unlimited storage
- **Managed** handling maintenance and any critical problems for you
- **Accessible** from anywhere in the world over HTTP or HTTPS

###### Mobile

- Create mobile back-end services for IOS, Android and Windows apps quickly and easily
- Adding corporate sign-in and the connecting to on-premises resources such as SAP, Oracle, SQL Server and SharePoint
- Offline data synchronization
- Connectivity to on-premises data
- Broadcasting push notifications
- Autoscaling to match business needs

###### Databases

Provides multiple databases services to store a wide variety of data types and volumes.

| Service name                         | Service function                                                                                    |
| ------------------------------------ | --------------------------------------------------------------------------------------------------- |
| Azure Cosmos DB                      | Globally distributed database that supports NoSQL options                                           |
| Azure SQL Database                   | Fully managed relational database with auto-scale, integral intelligence, and robust security       |
| Azure Database for MySQL             | Fully managed and scalable MySQL relational database with high availability and security            |
| Azure Database for PostgreSQL        | Fully managed and scalable PostgreSQL relational database with high availability and security       |
| SQL Server on Azure Virtual Machines | Service that hosts enterprise SQL Server apps in the cloud                                          |
| Azure Synapse Analytics              | Fully managed data warehouse with integral security at every level of scale at no extra cost        |
| Azure Database Migration Service     | Service that migrates databases to the cloud with no application code changes                       |
| Azure Cache for Redis                | Fully managed service caches frequently used and static data to reduce data and application latency |
| Azure Database for MariaDB           | Fully managed and scalable MariaDB relational database with high availability and security          |

###### Web

Includes firts-class support to build and host web apps and HTTP-based web services.

| Service name                          | Description                                                               |
| ------------------------------------- | ------------------------------------------------------------------------- |
| Azure App Service                     | Quickly create powerful cloud web-based apps                              |
| Azure Notification Hubs               | Send push notifications to any platform from any back end                 |
| Azure API Management                  | Publish APIs to developers, partners, and employees securely and at scale |
| Azure Cognitive Search                | Deploy this fully managed search as a service                             |
| Web Apps feature of Azure App Service | Create and deploy mission-critical web apps at scale                      |
| Azure SignalR Service                 | Add real-time web functionalities easil                                   |

###### IoT

| Service name  | Description                                                                                                                                                                                         |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| IoT Central   | Fully managed global IoT software as a service (SaaS) solution that makes it easy to connect, monitor, and manage IoT assets at scale                                                               |
| Azure IoT Hub | Messaging hub that provides secure communications between and monitoring of millions of IoT devices                                                                                                 |
| IoT Edge      | Fully managed service that allows data analysis models to be pushed directly onto IoT devices, which allows them to react quickly to state changes without needing to consult cloud-based AI models |

###### Big data

- Open-source cluster technologies developed to deal with large data sets
- Azure supports a broad range of technologies and services to provide big data and analytics solutions

| Service name            | Description                                                                                                                                                                                     |
| ----------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Azure Synapse Analytics | Run analytics at a massive scale by using a cloud-based enterprise data warehouse that takes advantage of massively parallel processing to run complex queries quickly across petabytes of data |
| Azure HDInsight         | Process massive amounts of data with managed clusters of Hadoop clusters in the cloud                                                                                                           |
| Azure Databricks        | Integrate this collaborative Apache Spark-based analytics service with other big data services in Azure                                                                                         |

###### AI

- AI, in the context of cloud computing, is based around a broad range of services, the core of which is machine learning
  - Data science technique that allows computers to use existing data to forecast future behaviors, outcomes, and trends
  - Using machine learning, computers learn without being explicitly programmed

| Service name                   | Description                                                                                                                                                                                                                                                  |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Azure Machine Learning Service | Cloud-based environment you can use to develop, train, test, deploy, manage, and track machine learning models. It can auto-generate a model and auto-tune it for you. It will let you start training on your local machine, and then scale out to the cloud |
| Azure ML Studio                | Collaborative visual workspace where you can build, test, and deploy machine learning solutions by using prebuilt machine learning algorithms and data-handling modules                                                                                      |

- Closely related services: Cognitive Services
  - Prebuilt APIs to solve complex problems

| Service name                | Description                                                                                                                             |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| Vision                      | Use image-processing algorithms to smartly identify, caption, index, and moderate your pictures and videos                              |
| Speech                      | Convert spoken audio into text, use voice for verification, or add speaker recognition to your app                                      |
| Knowledge mapping           | Map complex information and data to solve tasks such as intelligent recommendations and semantic search                                 |
| Bing Search                 | Add Bing Search APIs to your apps and harness the ability to comb billions of webpages, images, videos, and news with a single API call |
| Natural Language processing | Allow your apps to process natural language with prebuilt scripts, evaluate sentiment, and learn how to recognize what users want       |

###### DevOps

- Automating software delivery
- You can create build and release pipelines that provide continuous integration, delivery, and deployment for your applications
- You can integrate repositories and application tests, perform application monitoring, and work with build artifacts
- You can also work with and backlog items for tracking, automate infrastructure deployment, and integrate a range of third-party tools and services such as Jenkins and Chef

| Service name       | Description                                                                                                                                                                                                                            |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Azure DevOps       | Use development collaboration tools such as high-performance pipelines, free private Git repositories, configurable Kanban boards, and extensive automated and cloud-based load testing. Formerly known as Visual Studio Team Services |
| Azure DevTest Labs | Quickly create on-demand Windows and Linux environments to test or demo applications directly from deployment pipelines                                                                                                                |

#### Get started with Azure accounts

- To create and use Azure services, you need an Azure subscription
- You need to create an Azure account, and a subscription will be created for you
- For example, your company might use a single Azure account for your business and separate subscriptions for development, marketing, and sales departments
- After you've created an Azure subscription, you can start creating Azure resources within each subscription

![Azure accounts hierarchy](https://docs.microsoft.com/en-us/learn/azure-fundamentals/intro-to-azure-fundamentals/media/scope-levels-12669ee1.png)

##### Create an Azure account

- You can purchase Azure access directly from Microsoft by signing up on the Azure website or through a Microsoft representative
- You can also purchase Azure access through a Microsoft partner
- Free account:
  - $200 credit
  - azure.microsoft.com/free
- Multiple subscriptions -> organize them into invoice sections
  - Each invoice section is a line item on the invoice that shows the charges incurred that month
- Multiple invoices -> Billing profiles
  - Has it's own monthly invoice and payment method
- Subscription:
  - (Documentation)[docs.microsoft.com]
  - Support
  - Videos

##### What is the Azure free account?

- Includes:
  - Free access to popular Azure products for 12 months
  - A credit to spend for the first 30 days
  - Access to more than 25 products that are always free
- To sign up you need:
  - A phone number
  - A credit card
  - A Microsoft or Github account

##### What is the Azure free student account?

- Includes:
  - Free access to certain Azure services for 12 months
  - A credit ($100) to use in the first 12 months
  - Free access to certain software developer tools

You can sign up without credit card.

##### What is Learn sandbox?

- Temporary subscription
- Allows you to create Azure resources for the duration of a Lear module
- Automatically cleans up the temporary resources for you after you've completed the module

#### Case study introduction

- Tailwind Traders currently manages an on-premises datacenter that hosts the company's retail website
- The datacenter also stores all of the data and streaming video for its applications
- The IT department is currently responsible for all of the management tasks for its computing HW and software
- IT team handles the procurement process to buy new HW, installs and configures software, and deploys everything throughout the datacenter
- It would be advantageous to have servers, storage, databases, and other services immediately available when you develop and deploy applications

#### Summary

- Describe the basic concepts of cloud computing
- Determine wheter Azure is the right solution for your business needs
- Differentiate between the different methods of creating an Azure subscription

### Discuss Azure fundamental concepts

#### Introduction

- Tailwind Traders -> decided to migrate its applications and data to Microsoft Azure

#### Discuss different types of cloud models

##### What are public, private, and hybrid clouds?

- Three deployment models for cloud computing:
  - Public cloud
  - Private cloud
  - Hybrid cloud

<table>
  <thead>
    <tr>
      <th>Deployment model</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Public cloud</td>
      <td>
        <ul>
          <li>Services are offered over the public internet and available to anyone who wants to purchase them</li>
          <li>Cloud resources are owned and operated by a third-party cloud service provider</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>Private cloud</td>
      <td>
        <ul>
          <li>Computing resources used exclusively by users from one business or organization</li>
          <li>Can be phisically located at your organization's on-site (on-premises) datacenter, or it can be hosted by a third-party service provider</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>Hybrid cloud</td>
      <td>
        <ul>
          <li>Computing environment that combines a public cloud and a private cloud by allowing data and applications to be shared between them.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Cloud model comparison

- Public cloud
  - No capital expenditures to scale up
  - Applications can be quickly provisioned and deprovisioned
  - Organizations pay only for what they use
- Private cloud
  - HW must be purchased for start-up and maintenance
  - Organizations have complete control over resources and security
  - Organizations are responsible for HW maintenance and updates
- Hybrid cloud
  - Provides the most flexibility
  - Organizations determine where to run their applications
  - Organizations control security, compliance, or legal requirements

#### Describe cloud benefits and considerations

##### What are some cloud computing advantages?

Advantages that a cloud environment has over a physical environment:

- **High availability**: depending on the service-level agreement (SLA) that you choose, you cloud-based apps can provide a continuous user experience with no apparent downtime, even when things go wrong
- **Scalability**:
  - Scale vertically: adding RAM or CPUs
  - Scale horizontally: adding instances of resources, such as VMs
- **Elasticity**:
  - Autoscaling
  - Always have the resources they need
- **Agility**: deploy and configure quickly as app requirements change
- **Geo-distribution**: deploy apps and data to regional datacenters around the globe, thereby ensuring that your customers have the best performance
- **Disaster recovery**: backup services, data replication and geo-distribution
  - Deploy apps with the confidence that comes from knowing that your data is safe in the event of disaster

##### Capital expenses vs. operating expenses

- **Capital Expenditure (CapEx)**:
  - Up-front spending of money on physical infraestructure
  - Deducts that up-front expense over time
- **Operational Expenditure (OpEx)**:
  - Spending money on services or products now
  - Billed for them now
  - Deducts this expense in the same year you spend it
  - There is no up-front cost as you pay for a service or product as you use it

Tailwind Traders:

- Owns its infraestructure
- Accountants categorize as CapEx
- Limited useful lifespan -> assets are depreciated or amortized

Cloud services -> OpEx -> because their consumption model -> cloud service provider manages the costs that are associated with the purchase and lifespan of the physical equipment

##### Cloud computing is a consumption-based model

End users only pay for the resources that they use.

Benefits:

- No upfront costs
- No need to purchase and manage costly infraestructure that users might not use to its fullest
- The ability to pay for additional resources when they are needed
- The ability to stop paying for resources that are no longes needed

#### Describe different cloud services

##### What are cloud service models?

![Cloud service models schema](https://docs.microsoft.com/en-us/learn/azure-fundamentals/fundamental-azure-concepts/media/iaas-paas-saas-575a09e9.png)

These models define the different levels of shared responsibility that a cloud provider and cloud tenant are responsible for.

<table>
  <thead>
    <tr>
      <th>Model</th>
      <th>Definition</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>IaaS</td>
      <td>Infraestructure-as-a-service</td>
      <td>
        <ul>
          <li>Closest to managing physical servers</li>
          <li>Operating system maintenance and network configuration is up to you</li>
          <li>Advantage: rapid deployment</li>
          <li>Example: Azure virtual machines</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>PaaS</td>
      <td>Platform-as-a-service</td>
      <td>
        <ul>
          <li>Managed hosting environment</li>
          <li>The cloud provider manages the virtual machines and networking resources</li>
          <li>The cloud tenant deploys their applications into the managed hosting environment</li>
          <li>Example: Azure App Services</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>SaaS</td>
      <td>Software-as-a-Service</td>
      <td>
        <ul>
          <li>The cloud provider manages all aspects of the application environment, such as virtual machines, networking resources, data storage and applications</li>
          <li>The cloud tenant only needs to provide their data to the application managed by the cloud provider</li>
          <li>Example: Microsoft Office 365</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

###### IaaS

Most fleixble category of cloud services. It aims to give you complete control over the HW that runs your application.

- Advantages:
  - **No CapEx**
  - **Agility**: applications can be made accessible quickly and deprovisioned whenever needed
  - **Management**: shared responsability
    - User -> manages and maintains the services they have provisioned
    - Cloud provider -> manages and maintains the cloud infraescruture
  - **Consumption-based model**:
    - OpEx model
    - Pay for what uses
  - **Skills**: no deep technical skills are required
  - **Cloud benefits**: organizations can use the skills and expertise of the cloud provider to ensure workloads are made secure and highly available
  - **Flexibility**: most flexible cloud service
    - Control do configure and manage the HW running your application

###### PaaS

Same benefits and considerations as IaaS, but there are some additional benefits.

- Advantages:
  - **No CapEx**
  - **Agility**: PaaS is more agile than IaaS, and users don't need to configure servers for running applications
  - **Consumption-based model**
  - **Skills**: no deep technical skills are required
  - **Cloud benefits**: users can gain access to more cutting-edge development tools. They can then apply these tools across an application's lifecycle
  - **Productivity**: users can focus on application development only, because the cloud provider handles all platform management
- Disadvantage:
  - **Platform limitations**: there can be some limitations to a cloud platform that might affect how an application runs

###### SaaS

SW centrally hosted and managed for you and your users or customers.
Licensed through a monthly or annual subscription.
Provides the same benefits as IaaS, but again there are some additional benefits.

- Advantages:
  - **No CapEx**
  - **Agility**: users can provide staff with access to the lastest SW quickly and easily
  - **Pay-as-you-go princing model**
  - **Skills**: no deep technical skills are required
  - **Flexibility**: users can access the same application data from anywhere
- Disadvantage:
  - **SW limitations**: there can be some limitations to a SW applicatio that might affect how users work. Because you're using as-is SW, you don't have direct control of features

##### Cloud service model comparison

<table>
  <thead>
    <tr>
      <th>IaaS</th>
      <th>PaaS</th>
      <th>SaaS</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>The most flexible cloud service</td>
      <td>Focus on application development</td>
      <td>Pay-as-you-go princing model</td>
    </tr>
    <tr>
      <td>You configure and manage the HW for your application</td>
      <td>Platform management is handled by the cloud provider</td>
      <td>Users pay for the SW they use on a subscription model</td>
    </tr>
  </tbody>
<table>

Various levels of responsibility between a cloud provider and a cloud tenant:

![Levels of responsibility](https://docs.microsoft.com/en-us/learn/azure-fundamentals/fundamental-azure-concepts/media/shared-responsibility-76efbc1e.png)

##### What is serverless computing?

Enables devs to build applications faster by eliminating the need for them to manage infra.

Cloud service provider automatically provisions, scales and manages the infra required to run the code.

Serverless architectures are highly scalable and event-driven, only using resources when a specific function or trigger occurs.

The "serverless" name comes from the fact that the tasks associated with infra provisioning and management are invisible to the dev.

Devs can increase their focus on the business logic and deliver more value to the core of the business. Stay focused on innovation.

### Describe core Azure architectural components

#### Overview of Azure subscriptions, management groups, and resources

The Azure organizing structure for resources, which has 4 levels: management groups, subscriptions, resource groups and resources.

![Azure organizing structure for resources](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-architecture-fundamentals/media/hierarchy-372fef74.png)

- **Resources**: instances of services that you create, like VMs, storage or SQL databases
- **Resource groups**: resources are combined into resource groups, which act as a logical container into which Azure resources like web apps, databases and storage accounts are deployed and managed
- **Subscriptions**: groups together user accounts and the resources that have been created by those user accounts. For each subscription, there is limits or quotas on the amount of resources that you can create and use. Organizations can use subscriptions to manage costs and the resources that are created by users, teams and projects
- **Management groups**: help manage access, policy and compliance for multiple subscriptions. All subscriptions in a management group automatically inherit the conditions applied to the management group

#### Azure regions, availability zones, and region pairs

- Resources are created in regions, which are different geographical locations around the globe that contain Azure datacenters.
- Datacenter around the globe
- Azure organizes them into regions
- Some offer availability zones, which are Azure datacenters within that region

##### Azure regions

- Geographical area on the planet that contains at least one potentially multiple datacenters that are nearby and networked together with a low-latency network
- Some services or VM features are only available in certain regions, such as specific VM sizes or storage types
- There are also some global Azure services that don't require you to select a particular region, such as Azure Active Directory, Azure Traffic Manager, and Azure DNS
- All the available regions as of June 2020:

![Available Azure regions](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-architecture-fundamentals/media/regions-small-be724495.png)

##### Why are regions important?

- Flexibility to bring applications closer to your users no matter where they are
- Better scalability and redundancy
- Preserve data residency for your services

##### Special Azure regions

- When you build out your applications for compliance or legal purposes
- Examples:
  - **US DoD Central, US Gov Virginia, US Gov lowa and more**:
    - Physical and logical network-isolated instances for U.S. government
    - Operated by screened U.S. personnel
    - Additional compliance certifications
  - **China East, China North, and more**:
    - Partnership between Microsoft and 21Vianet
    - Microsoft doesn't directly maintain the datacenter

##### Azure availability zones

Azure can help make your app highly available through availability zones.

###### What is an availability zones?

- Physically separate datacenter within Azure region
- Each availability zone is made up for one or more datacenters equipped with independent power, cooling and networking
- Set up to be an _isolation boundary_
- Connected through high-speed, private fiber-optic networks

![Availability zones schema](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-architecture-fundamentals/media/availability-zones-5c3c490c.png)

##### Supported regions

- Not every region has support for availability zones
- [Regions that support availability zones in Azure](https://docs.microsoft.com/en-us/azure/availability-zones/az-region)

##### Use availability zones in your apps

- To run mission-critical applications
- Build high availability into your application architecture by co-locating your compute, storage, networking and data resources within zone and replicating in other zones
- Are primarily for:
  - VMs
  - Managed disks
  - Load balancers
  - SQL databases
- Services that support availability zones:
  - **Zonal services**: pin the resource to a specific zone (VMs, managed disks, IP addresses)
  - **Zone-redundant services**: the platform replicates automatically across zones (zone-redundant storage, SQL database)
  - **Non-regional services**: always available from Azure geographies and ae resilient to zone-wide outages as well as region-wide outages

#### Azure region pairs

- There's a minimum of three zones within a single region
- Large disaster tat could cause an outage to affect two datacenters
  - Azure also creates _region pairs_

##### What is region pair?

- Each Azure region is always paired with another region within the same geography at least 300 miles away
- Allows for the replication of resources
- Helps reduce the likelihood of interruptions because of events such as natural disasters, civil unrest, power outages, or physical network outages that affect both regions at once
- If a region in a pair was affected by a natural disaster, for instance, services would automatically failover to the other region in its region pair

![Example of region pair](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-architecture-fundamentals/media/region-pairs-d9eb9728.png)

- Provide reliable services and data redundancy
- Additional advantages of region pairs:
  - If an extensive Azure outage occurs, one region out of every pair is prioritized to make sure at least one is restored as quickly as possible for applications hosted in that region pair
  - Planned Azure updates are rolled out to paired regions one region at a time to minimize downtime and risk of application outage
  - Data continues to reside within the same geography as its pair (except for Brazil South) for tax- and law-enforcement jurisdiction purposes

#### Azure resources and Azure Resource Manager

- **Resource**: manageable item that's available through Azure
  - VMs
  - Storage accounts
  - Web apps
  - Databases
  - Virtual networks
- **Resource group**: container that holds related resources for an Azure solution

##### Azure resource groups

- Logical container for resources deployed on Azure
- Resources = anything you create in an Azure subscription
  - VMs
  - Azure Application Gateway instances
  - Azure Cosmos DB instances
  - ...
- All resources must be in a resource group
- A resource can only be a member of a single resource group
- Resource groups can't be nested
- Resources can be moved between resource groups with some services having specific limitations or requirements to move

###### Logical grouping

- Exist to help manage and organize your Azure resources

###### Life cycle

- If you delete a resource group, all resources contained within it are also deleted
- Organizing resources by life cycle can be useful in nonproduction environments

###### Authorization

- Scope for applying role-based access control (RBAC) permissions
- Ease administration and limit access to allow only what's needed

##### Azure Resource Manager

- Deployment and management service for Azure
- Provides a management layer that enables you to create, update, and delete resources in your Azure account
- Flux:
  - User sends a request from any of the Azure tools, APIs, or SDKs -> Resource Manager receives the request -> authenticates and authorizes the request -> sends the request to the Azure service, which takes the requested action

![The role Resource Manager plays in handling Azure requests](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-architecture-fundamentals/media/consistent-management-layer-feef9259.png)

- All capabilities that are available in the Azure portal are also available through PowerShell, the Azure CLI, REST APIs, and client SDKs
- Functionality initially released through APIs will be represented in the portal within 180 days of initial release

###### The benefits of using Resource Manager

- Manage your infrastructure through declarative templates rather than scripts. A Resource Manager template is a JSON file that defines what you want to deploy to Azure
- Deploy, manage, and monitor all the resources for your solution as a group, rather than handling these resources individually
- Redeploy your solution throughout the development life cycle and have confidence your resources are deployed in a consistent state
- Define the dependencies between resources so they're deployed in the correct order
- Apply access control to all services because RBAC is natively integrated into the management platform
- Apply tags to resources to logically organize all the resources in your subscription
- Clarify your organization's billing by viewing costs for a group of resources that share the same tag

### Azure subscriptions and management groups

#### Azure subscriptions

- Provides you with authenticated and authorized access to Azure products and services
- Logical unit of Azure services that links to an Azure account
  - Azure account = an identity in Azure Active Directory (Azure AD) or in a directory that Azure AD trusts

![Azure subscription schema](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-architecture-fundamentals/media/subscriptions-afe063a7.png)

- An account can have one subscription or multiple subscriptions
- Define boundaries around Azure products, services, and resources
- Two types of subscription boundaries:
  - **Billing boundary**:
    - Determines how an Azure account is billed for using Azure
    - Separate billing reports and invoices for each subscription
  - **Access control boundary**:
    - Azure applies access-management policies at the subscription level
    - Manage and control access to the resources that users provision with specific subscriptions

#### Create additional Azure subscriptions

---
