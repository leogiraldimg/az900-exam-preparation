# AZ900 - Exam Preparation

Knowledge trail: https://docs.microsoft.com/en-us/learn/certifications/exams/az-900.

## Describe core Azure concepts

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

## Describe cloud concepts

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

##### Create additional Azure subscriptions

You might choose to create additional subscriptions to separate:

- **Environments**:
  - Set up separate environments for development and testing, security, or to isolate data for compliance reasons
  - Resource access control occurs at the subscription level
- **Organizational structures**:
  - Allows you to manage and control access to the resources that users provision within each subscription
- **Billing**:
  - Manage and track costs based on your needs
  - Create one subscription for your production workloads and another subscription for your development and testing workloads

Additional subscriptions:

- **Subscription limits**:
  - Subscriptions are bound to some hard limitations
  - For example, the maximum number of Azure ExpressRoute circuits per subscription is 10
  - If there's a need to go over those limits in particular scenarios, you might need additional subscriptions

##### Customize billing to meet your needs

- Organize subscriptions into invoice sections
- You can set up multiple invoices within the same billing account
  - Create additional billing profiles

![Overview of how billing is structured](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-architecture-fundamentals/media/billing-structure-overview-2c81a8ad.png)

#### Azure management groups

- Manage access, policies, and compliance for subscriptions
- Provide a level of scope above subscriptions
- Organize subscriptions into containers called management groups
  - Apply your governance conditions to the management groups
- Give you enterprise-grade management at a large scale no matter what type of subscriptions you might have
- All subscriptions within a single management group must trust the same Azure AD tenant
- Example: apply policies to a management group that limits the regions available for VM creation

##### Hierarchy of management groups and subscriptions

- Build a flexible structure of management groups and subscriptions to organize your resources into a hierarchy for unified policy and access management

![Example of creating a hierarchy for governance by using management groups](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-architecture-fundamentals/media/management-groups-and-subscriptions-bba71896.png)

- For example, you could limit VM locations to the US West Region in a group called Production
  - This policy will inherit onto all the Enterprise Agreement subscriptions that are descendants of that management group and will apply to all VMs under those subscriptions
- One assignment on the management group can enable users to have access to everything they need instead of scripting RBAC over different subscriptions

##### Important facts about Management Groups

- 10,000 management groups can be supported in a single directory
- A management group tree can support up to six levels of depth. This limit doesn't include the root level or the subscription level
- Each management group and subscription can support only one parent
- Each management group can have many children
- All subscriptions and management groups are within a single hierarchy in each directory

## Describe core Azure services

### Explore Azure compute services

#### Overview of Azure compute services

- Azure compute is an on-demand computing service for running cloud-based applications
- Some of the most prominent services are:
  - ![Azure compute services](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-compute-fundamentals/media/compute-services-13e531e1.png)
  - **Azure Virtual Machines**:
    - _Virtual Machines_:
      - SW emulations of physical computers
      - Includes:
        - Virtual processor
        - Memory
        - Storage
        - Networking resources
      - Can create and use VMs in the cloud
      - Provides IaaS
      - Total control over an operating system (OS) and environment
    - _Virtual machines scale sets_:
      - Deploy and manage a set of identical VMs
      - True autoscale -> VMs configured all the same
      - No pre-provisioning is required
      - Demands goes up -> more VM instances can be added
      - Demands goes down -> VM instances can be removed
      - ☝️ This process can be manual, automated or a combination of both
  - **Azure Container Instances**:
    - _Containers and Kubernets_:
      - Deploy and manage containers
      - Containers are lightweight, virtualized application environments
      - You can run multiple instances of a containerized application on a single host machine
  - **Azure App Service**:
    - Build, deploy, and scale enterprise-grade web, mobile, and API apps running on any platform
    - PaaS
    - Rigorous performance, scalability, security and compliance requirements while using a fully managed platform
  - **Azure Functions (or serverless computing)**:
    - Ideal when you're concerned only about the code running your service and not the underlying platform or infrastructure
    - Used when you need to perform work in response to an event, timer or message from another Azure service
    - Work that can be completed quickly

#### Decide when to use Azure Virtual Machines

- Provides IaaS in the form of a virtualized server
- VMs are an ideal choice when you need:
  - Total control over the OS
  - The ability to run custom software
  - To use custom hosting configurations.
- Preconfigured VM image
  - An image is a template used to create a VM
  - Include an OS and often other software, like development tools or web hosting environments

##### Examples of when to use VMs

- **During testing and development**
- **When running applications in the cloud**
  - Provide substantial economic benefits
    - Application might need to handle fluctuations in demand
    - Shutting down VMs when you don't need them
    - Quickly starting them up to meet a sudden increase in demand
    - You pay only for the resources you use
- **When extending your datacenter to the cloud**
  - Creating a virtual network in Azure and adding VMs to that virtual network
- **During disaster recovery**
  - Get significant cost savings by using an IaaS-based approach to disaster recovery
  - If a primary datacenter fails, you can create VMs running on Azure to run your critical applications

##### Move to the cloud with VMs

- Excellent choice when you move from a physical server to the cloud = "lift and shift"
  - Create an image of the physical server and host it within a VM

##### Scale VMs in Azure

- Single VMs for testing, development, or minor tasks or group VMs to provide high availability, scalability and redundancy
- Features:
  - **Virtual machine scale sets**:
    - Create and manage a group of identical, load-balanced VMs
    - Centrally manage, configure, and update a large number of VMs in minutes to provide highly available applications
    - Automatically increase or decrease in response to demand or a defined schedule
  - **Azure Batch**:
    - Large-scale parallel and high-performance computing (HPC) batch jobs with the ability to scale to tens, hundreds, or thousands of VMs
    - Batch does the following:
      - Starts a pool of compute VMs for you
      - Installs applications and staging data
      - Runs jobs with as many tasks as you have
      - Identifies failures
      - Requeues work
      - Scales down the pool as work completes

#### Decide when to use Azure App Service

- Enables you to build and host web apps, background (BG) jobs, mobile back-ends, and RESTful APIs in the programming language of your choice without managing infrastructure
- Offers automatic scaling and high availability
- Supports Windows and Linux
- Enables automated deployments from GitHub, Azure DevOps, or any Git repo to support a continuous deployment model
- PaaS environment
- Focus on the website and API logic while Azure handles te infrastructure to run and scale your web applications

##### Azure App Service costs

- Pay for the Azure compute resources your app uses while it processes requests based on the App Service plan you choose
- The App Service plan determines how much HW is devoted to your host
- Ex.:
  - Dedicated or shared HW?
  - How much memory reserved for it?
- There's a free tier you can use to host small, low-traffic sites

##### Types of app services

With App Service, you can host most common app service styles like:

- **Web apps**
  - Full support for hosting web apps by using ASP.NET, ASP.NET Core, Java, Ruby, Node.js, PHP, or Python
  - Windows or Linux as the host OS
- **API apps**
  - You can build REST-based web APIs by using your choice of language and framework
  - Full swagger support
  - Ability to package and publish your API in Azure Marketplace
- **WebJobs**
  - Run a program (.exe, Java, PHP, Python, or Node.js) or script (.cmd, .bat, PowerShell, or Bash)
  - Scheduled or run by trigger
  - Background tasks as part of your logic application
- **Mobile apps**
  - Back end for iOS and Android apps
  - Store mobile app data in cloud-based SQL DB
  - Authenticate customers against common social providers, such as MSA, Google, Twitter and Facebook
  - Send push notifications
  - Execute custom back-end logic in C# or Node.js
  - SDK support for native iOS and Android, Xamarin and React Native apps

App Service handles:

- Deployment and management are integrated into de platform
- Endpoints can be secured
- Sites can be scaled quickly to handle high traffic loads
- The built-in load balancing and traffic manager provide high availability

#### Decide when to use Azure Container Instances or Azure Kubernetes Service

- VMs still limited to a single OS per virtual machine
- If you want to run multiple instances of an application on a single host machine, containers are an excellent choice

##### What are containers?

- Virtualization environments
- You can run multiple containers on a single physical or virtual host
- You don't manage the OS for a container
- Containers are lightweight and designed to be created, scaled out, and stopped dynamically
- Containers are designed to allow you to respond to changes on demand
- Most popular container engine: Docker

##### Compare VMs to containers

- **VMs**

  - Provide an abstraction layer for CPU, memory and storage
  - Can be changed without having to invest in new HW
  - You decide de OS, install tools and packaged
  - Downsides:
    - VMs can only run one OS at a time
    - Because it emulates a full computer, tasks like starting one up or taking a snapshot are pretty slow
  - MAIN POINT: virtualize the HW
  - WHEN TO USE: complete control the environment

- **Containers**
  - Bundle a single app and its dependencies
  - Provides a standardized runtime environment
  - Abstracts the OS and infrastructure requirements
  - Allows the containerized application to run side-by-side with other containerized apps
  - Without sacrificing the isolation that the VM originally offered
  - Containerized apps tend to be much smaller in size
  - Can be orchestrated with container cluster orchestration
    - Can easily deploy and manage multiple containerized applications
    - Without worrying about which server will host the container
  - MAIN POINT: virtualize the OS
  - WHEN TO USE:
    - Portability
    - Performance

Azure supports Docker

##### Manage containers

- Containers are managed through a container orchestrator
- Start, stop and scale out application instances as needed
- Two ways to manage both Docker and Microsoft-based containers in Azure:
  - **Azure Container Instances**
    - Fastest and simplest way to run a container in Azure
    - Without manage any VMs
    - Without adopt any additional service
    - PaaS
    - Upload your container -> runs
  - **Azure Kubernetes Services (AKS)**
    - Automating, managing and interacting with a large number of containers is known as orchestration
    - Complete orchestration service for containers with:
      - Distributed architectures
      - Large volumes of containers

##### What is Kubernetes?

- Container management automation
- API to create a cloud-native application management powerhouse
- Manage the placement of pods, which can consist of one or more containers, on a Kubernetes cluster node
- If one of these pods crashes, Kubernetes can create a new instance of it
- If a cluster node is removed, Kubernetes can move any affected workload to a different node in the cluster
- Kubernetes pods can be scaled to provide more or less throughput to meet scale demands
  - These scale operations can be triggered manually or automatically using Kubernetes horizontal pod auto-scaling
- Application needs to be updated -> Kubernetes can stagger the update deployment to minimize downtime
  - Update problematic -> roll back to a previous version
- Manage storage and networking
- Persistent volumes -> present data storage to one or more containers
  - Azure Storage
  - Azure Cosmos DB
- Networking
  - Expose pods to the internet
  - Load balancing
  - Isolation
  - Policy-driven networking security
- Additional capabilities -> Kubernetes API
  - Extends Kubernetes functionality

##### Use containers in your solutions

- _Microservice architecture_
  - Break solutions into smaller, independent pieces
- Separate portions of your app into logical sections that can be maintained, scaled or updated independently

##### What is a microservice?

- Web service small, well-defined scope and is loosely coupled from any other web service
- Each one self-contained and implementing a single business capability
- Don't need to share the same technology stack, libraries or frameworks
- Microservices can communicate with each other by using well-defined APIs
- Benefits
  - High release velocity
  - Highly scalable
  - Rich domains
  - Small development teams

#### Decide when to use Azure Functions

- Event driven -> application waiting for a particular input before it performs any processing
- _Serverless computing_ -> abstraction of servers, infra, and OSs
  - Azure takes care of managing the server infra and the allocation and deallocation of resources based on demand
  - **Abstraction of servers**
    - Execution can run on different compute instances
    - This execution context is transparent to the code
  - **Event-driven scale**
    - Workloads that respond to incoming events
    - Events include triggers by:
      - Timers, for example, if a function needs to run every day at 10:00 AM UTC
      - HTTP, for example, API and webhook scenarios
      - Queues, for example, with order processing
    - Developer authors a function -> contains both code and metadata about its triggers and bindings
    - Platform schedules the function to run and scales the number of compute instances
    - Triggers -> define how a function is invoked
    - Bindings -> provide a declarative way to connect to services from within the code
  - **Micro-billing**
    - Pay only for the time their code runs

##### Serverless computing in Azure

- Abstraction of servers -> take your mind off of infra concerns -> focus on developer concerns
- 3 benefits:
  - No infra management
  - Scalability
  - Only pay for what you use
- Azure -> 2 implementations of serverless compute:
  - **Azure Functions**
    - Perform work in response to an event, timer, or message from another Azure service
    - Can be completed quickly, within seconds or less
    - Scale automatically
    - Solid choice when demand is variable
    - Automatically deallocates resources
    - Can be
      - _Stateless_
        - Default
        - Behave as if they're restarted every time they respond to an event
      - _Stateful_
        - "Durable Functions"
        - Context is passed through the function to track prior activity
  - **Azure Logic Apps**
    - Trigger logic based on an event
    - Functions -> execute code
    - Logic apps -> execute workflows (WFs) -> automate business scenarios -> built from predefined logic blocks
    - Logic app instances that runs the actions in the WFs
    - Can include
      - Data conversions
      - Flow controls (switch, loops, and branching)
    - Using a visual designer on the Azure portal or in Visual Studio
    - Persisted as a JSON file with a known WF schema
    - More than 200 different connectors and processing blocks
    - Can build custom connectors and WF steps
    - Often all without writing any code
    - Ideal for a business analyst role

##### Functions vs. Logic Apps

- Both create complex orchestrations
- Functions -> write code to complete each step
- Logic Apps -> use GUI to define the actions ans how they relate to one another
- You can mix: calling functions from logic apps and calling logic apps from functions

<table>
  <thead>
    <tr>
      <th></th>
      <th>**Functions**</th>
      <th>**Logic Apps**</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>State</td>
      <td>Normally stateless, but Durable Functions provide state.</td>
      <td>Stateful.</td>
    </tr>
    <tr>
      <td>Development</td>
      <td>Code-first (imperative).</td>
      <td>Designer-first (declarative).</td>
    </tr>
    <tr>
      <td>Connectivity</td>
      <td>
        <p>About a dozen built-in binding types.</p>
        <p>Write code for custom bindings.</p>
      </td>
      <td>
        <p>Large collection of connectors.</p>
        <p>Enterprise Integration Pack for B2B scenarios. Build custom connectors.</p>
      </td>
    </tr>
    <tr>
      <td>Actions</td>
      <td>Each activity is an Azure function. Write code for activity functions.</td>
      <td>Large collection of ready-made actions.</td>
    </tr>
    <tr>
      <td>Monitoring</td>
      <td>Azure Application Insights.</td>
      <td>Azure portal, Log Analytics.</td>
    </tr>
    <tr>
      <td>Management</td>
      <td>REST API, Visual Studio.</td>
      <td>Azure portal, REST API, PowerShell, Visual Studio.</td>
    </tr>
    <tr>
      <td>Execution context</td>
      <td>Can run locally or in the cloud.</td>
      <td>Runs only in the cloud.</td>
    </tr>
  </tbody>
</table>

#### Decide when to use Azure Virtual Desktop

##### What is Azure Virtual Desktop?

- Desktop and application virtualization service that runs on the cloud
- Cloud-hosted version of Windows
- Works with apps that you can use to access remote desktops and apps
- Can use most modern browsers to access
- Why desktop virtualization?
  - Central management security
  - Less IT management overhead
  - Separates your OS's data and apps from local HW
    - Running them separately on a remote server
  - Proximity to your data center or the cloud
  - Communicate over a secure outbound connection
  - Multiple users on a single VM

##### Why should you use Azure Virtual Desktop?

- **Provide the best user experience**
  - Connect to with any device over the internet
  - Use a Azure Virtual Desktop client to connect to their published Windows desktop and applications
  - Could either be a native application on the device or the Azure Virtual Desktop HTML5 web client
  - Users stay productive and don't encounter long load times
  - User profiles are containerized by using FSLogix
  - User profile is immediately available and appears in the system exactly like a native user profile
  - Can provide individual ownership through personal desktops
    - Engineering team -> can add or remove programs without impacting other users on that remote desktop
- **Enhance security**
  - Provides centralized security management
  - Azure Active Directory (AD)
  - Multifactor authentication
  - Granular role-based access controls (RBACs)
  - Single and multi-session environments
  - Reverse connect technology -> more secure than Remote Desktop Protocol -> don't open inbound ports to the session host VMs

##### What are some key features of Azure Virtual Desktop?

- **Simplified management**
  - Azure AD and RBACs to manage access to resources
  - Automate VM deployments
  - Manage VM updates
  - Provide disaster recovery
  - Uses Azure Monitor for monitoring and alerts
    - Lets admins identify through a single interface
- **Performance management**
  - Load balance users on your VM host pools
  - _Host pools_ -> collections of VMs with the same configuration assigned to multiple users
  - _Breadth mode_ -> configure load balance to occur as users sign in
    - Users are sequentially allocated across the host pool for your workload
  - _Depth mode_ -> users are fully allocated on one VM before moving to the next
    - Save costs
  - Automatically provision additional VMs when incoming demand exceeds threshold
- **Multi-session Windows 10 deployment**
  - Windows 10 Enterprise multi-session
  - More consistence experience with broader application support

##### How can you reduce costs with Azure Virtual Desktop?

- **Bring your own licenses**
  - No cost if you have an eligible Microsoft 364 license
  - Just pay for the Azure resources used by Azure Virtual Desktop
- **Save on compute costs**
  - Save up to 72% versus pay-as-you-go pricing

### Explore Azure networking services

#### Azure Virtual Network fundamentals

- You want to keep your existing IP addressing scheme and network appliances while ensuring that any data transfer is secure

##### What is Azure virtual networking?

- Enable Azure resources, such as VMs, web apps and databases to communicate with:
  - Each other
  - Users on the internet
  - Your on-premises client computers
- Azure network -> extension of your on-premises network with resources that links other Azure resources
- Network capabilities:
  - Isolation and segmentation
  - Internet communications
  - Communicate between Azure resources
  - Communicate with on-premises resources
  - Route network traffic
  - Filter network traffic
  - Connect virtual networks

###### Network configurations for VMs

- Azure virtual networks = VNets
  - Segmentation and isolation
  - Extension of your own data center into the cloud
  - Filter and route networking traffic between hosts and subnets
  - Interconnect virtual networks in the same region or even across regions using network peering
  - Service endpoints can be created to:
    - Azure Storage
    - Azure SQL Database
    - Azure Cosmos DB
    - Azure SQL Data Warehouse
    - Azure Database for PostgreSQL
    - Azure for MySQL
- Configurations:
  - **Isolation and segmentation**
    - Create multiple isolated virtual networks
    - Define a private IP address space by using either public or private IP address ranges
    - Divide that IP address space into subnets
    - Name resolution -> Azure built in name resolution service or use internal or external DNS server
  - **Internet communications**
    - VM can connect to internet by default
    - Enable incoming from internet -> public IP address or public load balancer
  - **Communicate between Azure resources**
    - _Virtual Networks_
      - VMs, App Service Environment for Power Apps, Azure Kubernetes Service and Azure Virtual Machine scale sets
    - _Service endpoints_
      - Azure SQL Databases and storage accounts
      - Link Azure resources to virtual networks -> improve security and provide optimal routing between resources
  - **Communicate with on-premises resources**
    - Three mechanisms:
      - _Point-to-site VPNs_
        - Computer outside organization into corporate network
        - Encrypted VPN connection
      - _Site-to-site VPNs_
        - Links on-premises VPN device or gateway (GW) to Azure VPN GW in a virtual network
        - Devices in Azure appear as being on the local network
        - Encrypted
        - Over the internet
      - _Azure ExpressRoute_
        - Needs greater bandwidth
        - Higher levels of security
        - Dedicated private connectivity to Azure
        - No internet
  - **Route network traffic**
    - Default: routes traffic between subnets
    - Settings:
      - _Route tables_
        - Define rules about how traffic should be directed
        - Control how packets are routed between subnets
      - _Border GW Protocol (BGP)_
        - Propagate on-premises BGP routes to Azure virtual networks
  - **Filter network traffic**
    - Approaches:
      - _Network security groups_
        - Azure resource
        - Contain multiple inbound and outbound security rules
        - Allow or block traffic
        - Factors
          - Source and destination IP address
          - Port
          - Protocol
      - _Network virtual appliances_
        - Specialized VM
        - Can be compared to a hardened network appliance
        - Carries out a particular network function
          - Firewall
          - Wide area network (WAN) optimization

##### Connect virtual networks

- Connect virtual networks together
- Network _peering_
  - Enables resources in each virtual network to communicate with each other
- User-defined routes (UDR)
  - Significant Azure's Virtual Networks
  - Greater control over network traffic flow
  - Control routing tables between subnets within a VNet or between them

![](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-networking-fundamentals/media/local-or-remote-gateway-in-peered-virual-network-21106a38.png)

#### Azure Virtual Network settings

- Powerful and highly configurable mechanisms for connecting entities in Azure
- Connect Azure resources to one another or to resources on-premises
- Isolate, filter and route your network traffic

##### Create a virtual network

- Configure a number of basic settings
  - ![](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-networking-fundamentals/media/create-virtual-network-286df13c.png)
    - **Subscription**
      - Multiple subscriptions to choose
    - **Resource group**
    - **Network name**
      - Unique in subscription
    - **Region**
  - ![](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-networking-fundamentals/media/create-virtual-network-ip-address-286df13c.png)
    - **Address space**
      - Define the internal address space in Classless Interdomain Routing (CIDR) format
      - Unique within subscription and any other networks that you connect to
    - **Subnet**
      - Create one or more subnets
      - Partitions the virtual network's address space
      - Subnet names must
        - Begin with a letter or number
        - Env with a letter, number or underscore
        - Contain only letters, numbers, underscores, periods or hyphens
      - **Service endpoints**
      - **NAT gateway**
        - Fully managed and highly resilient Network Address Translation (NAT) service
        - Configure a subnet to use a static outbound IP address when accessing the internet
    - ![](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-networking-fundamentals/media/create-virtual-network-security-286df13c.png)
      - **BastionHost**
        - Azure Bastion
        - Provides a secure and seamless RDP/SSH connectivity to VMs directly in the Azure portal over SSL
      - **DDoS Protection Standard**
        - Premium service
      - **Firewall**
        - Managed cloud-based network security service that protects your Azure Virtual Network resources
- Option to configure advanced settings
  - Multiple subnets
  - Distributed denial of service (DDoS) protection
  - Bastion host
  - Azure firewall (FW)
  - Service endpoints
  - NAT gateway

##### Define additional settings

- Define further settings
  - **Network security group**
    - Security rules that enable you to filter the type of network traffic that can flow in and out of virtual network subnets and network interfaces
    - Create network security group separately
    - Associate subnet in the virtual network
  - **Route table**
    - Azure automatically creates a route table for each subnet
    - Add system default routes to the table
    - Can add custom route tables to modify traffic between subnets and virtual networks
  - **Subnet Delegation**
    - Designate the subnet to be used by a dedicate service
- ![](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-networking-fundamentals/media/virtual-network-additional-settings-faff6cec.png)

##### Configure virtual networks

![Virtual network panel](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-networking-fundamentals/media/configure-virtual-network-9d0515c5.png)

- Settings include:
  - **Address spaces**: additional address spaces to the initial definition
  - **Connected devices**: list of all connected host in the virtual network
  - **Subnets**: additional subnets
  - **DDos protection**: Standard DDos protection plan
  - **Firewall**: Azure Firewall service for the virtual network
  - **Security**: security recommendation you can apply to your virtual network
  - **Network Manager**: connectivity and security admin configuration the virtual network is associated to
  - **DNS servers**: configure internal or external DNS servers the resources in the virtual network is associated to
  - **Peerings**: link virtual networks in peering arrangements
  - **Service endpoints**: enable service endpoints and apply them to multiple subnets
  - **Private endpoints**: list of private endpoints enabled in a subnet

#### Azure VPN Gateway fundamentals

- Encrypted tunnel within another network
- Connect two or more trusted private networks to one another over an untrusted network
- Traffic is encrypted
- Prevent (eavesdropping)[https://www.fortinet.com/resources/cyberglossary/eavesdropping]

##### VP GWs

- Type of virtual network GW
- Deployed in a dedicated subnet of the virtual network
- Enable the following connectivity:
  - On-premises <-> virtual networks (_site-to-site_ connection)
  - Individual devices <-> virtual networks (_point-to-site_ connection)
  - virtual networks <-> virtual networks (_network-to-network_ connection)

![VPN GW](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-networking-fundamentals/media/vpngateway-site-to-site-connection-diagram-0e1e7db2.png)

- One VPN GW in each virtual network
- One GW to connect to multiple locations (other virtual networks or on-premises datacenters)
- VPN types for VPN GW:
  - **_policy-based_**
    - Specify statically the IP address of packets that should be encrypted through each tunnel
    - Evaluates every data packet against those sets of IP
    - Choose the tunnel where that packet is going to be sent through
    - Key features:
      - Support for IKEv1 only
      - _Static routing_:
        - Source and destination are declared in the policy
        - Not declared in routing tables
      - Must be used in specific scenarios
        - Compatibility with legacy on-premises VPN devices
  - **_route-based_**
    - IPSec tunnels are modeled as a network interface or virtual tunnel interface
    - IP routing decides which one of these tunnel interfaces to use when sending each packet
    - Preferred connection method for on-premises devices
    - More resilient to topology changes
    - Scenarios:
      - Connections between virtual networks
      - Point-to-site connections
      - Multisite connections
      - Coexistence with an Azure ExpressRoute gateway
    - Key features:
      - Supports IKEv2
      - Uses any-to-any (wildcard) traffic selectors
      - Can use _dynamic routing protocols_
        - Routing/forwarding tables direct traffic to different IPSec tunnels
        - Source and destination networks aren't statically defined as they are in policy-based VPNs or even route-based VPNs with static routing
        - Routing tables are created dynamically using protocols such as Border GW Protocol (BGP)
- Main difference -> how to traffic to be encrypted is specified
- Both types:
  - use a pre-shared key as the only method of authentication
  - rely on Internet Key Exchange (IKE) and Internet Protocol Security (IPSec)
    - IKE is used to set up a security association between two endpoints
    - IPSec suite -> encrypts and decryts data packets

##### VP GW sizes

| SKU       | Site-to-site/Network-to-network tunnels | Aggregate throughput benchmark | BGP support   |
| --------- | --------------------------------------- | ------------------------------ | ------------- |
| Basic     | Maximum: 10                             | 100 Mbps                       | Not supported |
| VpnGw1/Az | Maximum: 30                             | 650 Mbps                       | Supported     |
| VpnGw2/Az | Maximum: 30                             | 1 Gbps                         | Supported     |
| VpnGw3/Az | Maximum: 30                             | 1.25 Gbps                      | Supported     |
| VpnGw4/Az | Maximum: 100                            | 5 Gbps                         | Supported     |
| VpnGw5/Az | Maximum: 100                            | 10 Gbps                        | Supported     |

##### Deploy VPN GWs

- **Required Azure resources**
  - <ins>Virtual network</ins>
    - With enough address space for the additional subnet that you'll need for the VPN GW
    - You can deployy one VPN GW within a virtual network
  - <ins>GatewaySubnet</ins>
    - Subnet called "GatewaySubnet" for the VPN GW
    - Use at least /27 address mask
    - You can't use this subnet for any other services
  - <ins>Public IP address</ins>
    - Create a Basic-SKU dynamic public IP address
    - This address provides a public-routable IP address as the target for your on-premises VPN device
    - Won't change unless you delete and recreate the VPN GW
  - <ins>Local network GW</ins>
    - To define the on-premises network's configuration
    - Includes the on-premises VPN device's public IPv4 address and the on-premises routable networks
    - This information is used by the VPN GW to route packets that are destined for on-premises networks through the IPSec tunnel
  - <ins>Virtual network GW</ins>
    - To route traffic between the virtual network and the on-premises datacenter or other virtual networks
    - A VPN GW or an ExpressRoute GW
  - <ins>Connection</ins>
    - To create a logical connection between the VPN GW and the local network GW
    - Made to the on-premises VPN device's IPv4 address as defined by the local network GW
    - From the virtual network GW and its associated public IP address
    - Can create multiple connections
  - ![What's required to deploy a VPN GW](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-networking-fundamentals/media/resource-requirements-for-vpn-gateway-2518703e.png)
- **Required on-premises resources**
  - A VPN device that supports policy-based or route-based VPN GWs
  - A public-facing (internet-routable) IPv4 address

##### High-availability scenarios

- Ways to ensure you have a fault-tolerant configuration:
  - **Active/standby**
    - VPN GWs deployed as two instances -> active/standby
    - Planned maintenance, unplanned disruption -> standby automatically assumes
    - Without user intervention
    - Connections are interrupted during this failover
    - Restored within a few seconds -> planned maintenance
    - 90 seconds -> unplanned disruptions
    - ![VPN active/standby schema](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-networking-fundamentals/media/active-standby-c4a3c14d.png)
  - **Active/active**
    - Support for the BGP routing protocol
    - Assign a unique public IP address to each instance
    - Create separate tunnels from the on-premises device to each IP address
    - ![VPN active/active schema](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-networking-fundamentals/media/dual-redundancy-d76100c9.png)
  - **ExpressRoute failover**
    - Configure a VPN GW as a secure failover path for ExpressRoute
      - Uses the internet as an alternative method of connectivity
    - Have resiliency built in
    - But they aren't immune to physical problems
  - **Zone-redundant GWs**
    - Regions that support availability zones, VPN GWs and ExpressRoute GWs
    - Brings resiliency, scalability, and higher availability
    - Separates GWs within a region while protecting your on-premises network connectivity to Azure from zone-level failures
      - Require different GW SKUs
      - Use Standard public IP addresses

#### Azure ExpressRoute fundamentals

- Extend your on-premises networks into the Microsoft cloud
- Over a private connection
- Help of a connectivity provider
- Can establish connections to Microsoft cloud services
- Connectivity can be from:
  - Any-to-any (IP VPN) network
  - Point-to-point Ethernet network
  - Virtual cross-connection
    - Through connectivity provider
    - Colocation facility
- Connections don't go over the public internet
- Advantages
  - More reliability
  - Faster speeds
  - Consistent latencies
  - Higher security

![Azure ExpressRoute overview](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-networking-fundamentals/media/azure-expressroute-overview-5520731d.png)

- Two different layers of the Open Systems Interconnection (OSI) model:
  - **Layer 2 (L2)**
    - Data Link Layer
    - Node-to-node communication on the same network
  - **Layer 3 (L3)**
    - Network Layer
    - Provides addressing and routing
    - Between node on a multi-node network

##### Features and benefits of ExpressRoute

- **Layer 3 connectivity between on-premises and Microsoft Cloud**
  - Through connectivity partners
  - Connections can be from:
    - Point-to-point network
    - Any-to-any network
    - Can also be virtual cross-connections through an exchange
- **Connectivity to Microsoft cloud services across all regions**
  - Enables direct access to the following services:
    - Microsoft Office 365
    - Microsoft Dynamics 365
    - Azure compute services (Azure VMs, etc.)
    - Azure cloud services (Azure Cosmos DB, etc.)
- **ExpressRoute premium add-on**
  - Global connectivity to Microsoft services
  - Across all regions
- **Dynamic routing between your network and Microsoft**
  - Uses the BGP routing protocol
    - Exchange routes between on-premises and resources in Azure
- **Built-in redundancy in every peering location**
  - Connectivity provider uses redundant devices
  - Redundant connections are configured with Layer 3 connectivity
    - Meet service-level agreements
- **Connection uptime SLA**
- **QoS support for Skype**
- **Across on-premises connectivity with ExpressRoute Global Reach**
  - Enable ExpressRoute Global Reach to exchange data across your on-premises sites
  - Connect your private datacenter through two ExpressRoute circuits
  - Travel through the Microsoft network

##### ExpressRoute connectivity models

![Azure ExpressRoute connectivity models](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-networking-fundamentals/media/azure-connectivity-models-4deabab1.png)

- Models to connect on-premises to MS cloud:
  - **CloudExchange colocation**
    - Layer 2 and Layer 3 connections
    - Ex.:
      - Your datacenter is colocated at a cloud exchange
      - Request a virtual cross-connection to the Microsoft cloud
  - **Point-to-point Ethernet connection**
    - Layer 2 and Layer 3 connections
    - Point-to-point links
    - Ex.:
      - On-premises datacenter
      - Point-to-point Ethernet link to connect to MS
  - **Any-to-any connection**
    - Integrate WAN with Azure
    - Like you would have between your datacenter and any branch offices
    - Layer 3
    - MS behaves like any other location on your private WAN
  - **Directly from ExpressRoute sites**
    - Connect directly into the MS's global network
    - Peering location strategically distributed
    - Provides dual 100 Gbps or 10 Gbps connectivity
    - Active/Active connectivity at scale

##### Security considerations

- Data doesn't travel over the public internet
- Private connection
  - From on-premises infra
  - To Azure infra
- Still sent over the public internet:
  - DNS queries
  - Certificate revocation list checking
  - Azure Content Delivery Network

### Explore Azure Storage services

#### Azure Storage account fundamentals

- Service that you can use to store files, messages, tables, and other types of information
- Clients can read data from and write data to
- Used by IaaS VMs and PaaS cloud services
- Azure Storage account
  - Created through
    - Azure portal
    - PowerShell
    - AzureCLI
  - Contain
    - Azure Storage data objects
    - Blobs
    - Files
    - Disks
  - Unique namespace for Azure Storage data
    - Accessible from anywhere in the world
    - HTTP or HTTPS
    - Data is secure, highly available, durable and massively scalable

![Create storage account](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-storage-fundamentals/media/create-storage-account-1c42138c.png)

![Account, container and blob](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-storage-fundamentals/media/account-container-blob-4da0ac47.png)

#### Disk storage fundamentals

- Provides disks for Azure VMs
- Applications and other services can access and use these disks
- Data is persistently stored and accessed from an attached virtual hard disk
- Different sizes and performance levels
  - Solid-state drives (SSDs)
  - Spinning hard disk drives (HDDs)
- Standard SSD and HDD -> less critical workloads
- Premium SSD -> mission-critical production applications
- Ultra disks -> data-intensive workloads such as SAP HANA, top tier databases, and transaction-heavy workloads
- IaaS disks with enterprise-grade durability -> ZERO% annualized failure rate

![Azure disks](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-storage-fundamentals/media/azure-disks-7841e01e.png)

#### Azure Blob storage fundamentals

- Object storage solution
- Can store massive amounts of data
  - Text
  - Binary data
- Unstructured -> no restrictions on the kinds of data
- Can manage
  - Thousands of simultaneous uploads
  - Massive amounts of video data
  - Constantly growing log files
- Advantage over disk storage: it does not require devs to think about and manage disks
  - Data is uploaded as blobs
- Ideal for:
  - Serving images or docs directly to a browser
  - Storing files for distributed access
  - Streaming video and audio
  - Storing data for backup and restore, disaster recovery, and archiving
  - Storing data for analysis by an on-premises or Azure-hosted service
  - Storing up to 8TB of data for VMs
- Stored in containers

#### Azure Files fundamentals

- Fully managed file shares
- Accessible via Server Message Block and Network File System protocols
- Mounted concurrently by cloud or on-premises deployments of Windows, Linux and macOS
- Application running in Azure VMs or cloud services can mount it to access file data
- Access simultaneously
- Possible scenarios of use:
  - Many on-premises applications use file shares
    - Makes it easier to migrate
    - Mount Azure file share to the same drive letter -> application should work
  - Store configuration files on a file share and access them from multiple VMs
  - Write data to a file share, and process or analyze the data later
    - Diagnostic logs, metrics and crash dumps
- Azure Files ensures the data is encrypted at rest, and SMP protocol ensures the data is encrypted in transit
  - ![Azure Files](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-storage-fundamentals/media/azure-files-5f942c3e.png)
- != from files on a corporate file share
  - Can access the files from anywhere in the world
  - Using URL that points to the file
  - Can also use Shared Access Signature (SAS) tokens
    - Allow access to a private asset for a specific amount of time
- Example of a service SAS URI:
  - ![SAS storage URI](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-storage-fundamentals/media/sas-storage-uri-037308fa.png)

#### Understand Blob access tiers

- To accommodate different access needs, Azure provides several _access tiers_, which you can use to balance your storage costs with your access needs
- Access tiers for blob storage:
  - **Hot access tier**
    - Data that is accessed frequently
    - Ex.: images for your website
    - Account level
    - Blob level, during upload or after upload
  - **Cool access tier**
    - Data that is infrequently accessed
    - Stored for at least 30 days
    - Ex.: invoices for your costumers
    - Account level
    - Blob level, during upload or after upload
    - Tolerate slightly lower availability
    - Requires high durability, retrieval latency, and throughput characteristics similar to hot data
    - Slightly lower SLA
    - Higher access costs, compared to Hot
    - Lower storage costs, compared to Hot
  - **Archive access tier**
    - Data that is rarely accessed
    - Stored at least 180 days
    - Flexible latency requirements
    - Ex.: long-term backups
    - Isn't available at the account level
    - Blob level, during upload or after upload
    - Stores data offline
    - Lowest storage costs
    - Highest costs to rehydrate and access data
- Choosing between the hot and cool access tiers on a general purpose storage account:
  - ![Account tier](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-storage-fundamentals/media/account-tier-42ec76d7.png)

### Explore Azure database and analytics services

#### Explore Azure Cosmos DB

- Globally distributed, multi-model DB service
- Elastically and independently scale throughput and storage across any number of Azure regions
- Fast, single-digit-millisecond data access by using any one of several popular APIs
- Comprehensive SLAs for throughput, latency, availability, and consistency guarantees
- Supports schema-less data
- A sample Azure Cosmos DB that's used to store data for a training portal website:
  - ![Sample Azure Cosmos DB that's used to store data for a training portal website](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-database-fundamentals/media/azure-cosmos-db-1c115364.png)
- Stores data in atom-record-sequence (ARS) format
- Data is then abstracted and projected as an API
  - SQL, MongoDB, Cassandra, Tables, and Gremlin
- Developers can stick with the API that they're the most comfortable with

#### Explore Azure SQL Database

- Relational DB
- Based on the latest stable version of the Microsoft SQL Server DB engine
- High-performance, reliable, fully managed, and secure DB
- Without needing to manage infra

##### Features

- PaaS DB engine
- Handles most of the database management functions
  - Upgrading
  - Patching
  - Backups
  - Monitoring
- Provides 99.99% availability
- Fully managed service
- MS handles all updates to the SQL and OS code
- Process both relation data and non-relational structures, such as graphs, JSON, spatial, and XML
- Advanced query processing features
  - High-performance, in-memory technologies and intelligent query processing
- The newest capabilities of SQL Server are released first to SQL DB

##### Migration

- Minimal downtime by using the **Azure Database Migration Service**
- Generate assessment reports that provide recommendations to help guide you through required changes prior to performing a migration
- After you assess and resolve any remediation required, you're ready to begin the migration process
- You just change the connection string in your apps

#### Exercise - Create a SQL database

Sandbox link: https://docs.microsoft.com/en-us/learn/modules/azure-database-fundamentals/exercise-create-sql-database

#### Explore Azure database for MySQL

- Relational DB service in the cloud
- Based on the MySQL Community Edition DB engine, versions 5.6, 5.7, and 8.0
- 99.99% availability SLA from Azure
- Built-in security, fault tolerance, and data protection
- Point-in-time restore to recover a server to an earlier state, as far back as 35 days
- Delivers:
  - Built-in high availability with no additional cost
  - Predictable performance and inclusive, pay-as-you-go pricing
  - Scale as needed, within seconds
  - Ability to protect sensitive data at-rest and in-motion
  - Automatic backups
  - Enterprise-grade security and compliance
- You can migrate your existing MySQL DBs with minimal downtime by using the Azure Database Migration Service

![Azure Database for MySQL conceptual diagram](https://docs.microsoft.com/en-us/learn/azure-fundamentals/azure-database-fundamentals/media/azure-db-for-mysql-conceptual-diagram-02e2a10a.png)

- Offers several service tiers -> each tier provides different performance and capabilities to support lightweight to heavyweight database workloads

#### Explore Azure Database for PostgreSQL

- Relational database service in the cloud
- Community version of the open-source PostgreSQL database engine
- Benefits:
  - High availability -> no additional configuration, replication, or cost required
  - Simple and flexible pricing -> predictable performance based on a selected pricing tier
  - Can scale compute or storage independently as needed, to make sure you adapt your service to match usage
  - Automatic backups and point-in-time-restore for up to 35 days
  - Enterprise-grade security and compliance to protect sensitive data at-rest and in-motion
    - Data encryption on disk
    - SSL encryption between client and server communication
- Two deployment options:
  - **Single Server**
    - Delivers
      - High availability with no additional cost
      - Predictable performance and inclusive, pay-as-you-go pricing
      - Vertical scale
      - Monitoring and alerting
      - Enterprise-grade security and compliance
      - Protect sensitive data at-rest and in-motion
      - Backups and point-in-time-restore -> up to 35 days
    - Three pricing tiers
      - Basic
      - General Purpose
      - Memory Optimized
    - Different resource capabilities to support your database workloads
  - **Hyperscale (Citus)**
    - Horizontally scales queries across multiple machines by using sharding
    - Query engine parallelizes incoming SQL queries across these servers for faster responses on large datasets
    - Workloads that are approaching, or already exceed, 100 GB of data
    - Supports
      - Multi-tenant applications
      - Real-time operational analytics
      - High throughput transactional workloads

#### Explore Azure SQL Managed Instance

- scalable cloud data service
- provides the broadest SQL Server database engine compatibility

##### Features

- (PaaS) database engine
- Fully-managed environment
- Quick provisioning
- Service scaling
- Automated patching and version upgrades
- Built-in high availability features
  - 99.99% uptime service level agreement (SLA)
- Automated backups
- Configurable backup retention period
- Azure SQL Database and Azure SQL Managed Instance offer many of the same features
- However, Azure SQL Managed Instance provides several options that might not be available to Azure SQL Database
- For example
  - They would like to migrate their existing databases to a SQL database running in the cloud
  - Their databases use Cyrillic characters for collation
  - Should migrate their databases to an Azure SQL Managed Instance
  - Azure SQL Database only uses the default SQL_Latin1_General_CP1_CI_AS server collation

##### Migration

- Azure Database Migration Service (DMS)

#### Explore big data and analytics

- Big data
- Large volumes of data
- Amount of data becomes increasingly hard to make sense of and to base decisions on
- Volumes are so large that traditional forms of processing and analysis are no longer appropriate

##### Azure Synapse Analytics

- Formerly Azure SQL Data Warehouse
- Limitless analytics service
- Enterprise data warehousing
- Big data analytics
- Serverless or provisioned resources at scale

##### Azure HDInsight

- Fully managed
- Open-source analytics service
- Easier, faster, and more cost-effective to process massive amounts of data
- Can run popular open-source frameworks and create cluster types
  - Apache Spark
  - Apache Hadoop
  - Apache Kafka
  - Apache HBase
  - Apache Storm
- Machine Learning Services
- Range of scenarios
  - Extraction
  - Transformation
  - Loading (ETL)
  - Data warehousing
  - Machine learning
  - IoT

##### Azure Databricks

- Unlock insights from all your data
- Build artificial intelligence solutions
- Apache Spark environment
- Shared projects
- Interactive workspace
- Supports
  - Python
  - Scala
  - R
  - Java
  - SQL
  - TensorFlow
  - PyTorch
  - Scikit-learn

##### Azure Data Lake Analytics

- Simplifies big data
- Queries to transform your data and extract valuable insights
- Jobs of any scale instantly
- Setting the dial for how much power you need.
- Only pay for your job when it's running

## Describe core solutions and management tools on Azure

### Choose the best Azure IoT service for your application

#### Identify the product options

- Azure IoT services
- Send their sensor readings to a specific endpoint in Azure via a message
- Message's data is then collected and aggregated
- Can be converted into reports and alerts
- Devices could be updated with new firmware
- Add new functionality by sending software updates from Azure IoT services
- Messages each machine sends can be received, stored, organized, and displayed by using Azure IoT services

##### Azure IoT Hub

- Managed service
- Hosted in the cloud
- Acts as a central message hub for bi-directional communication between your IoT application and the devices it manages
- Build IoT solutions with reliable and secure communications between millions of IoT devices and a cloud-hosted solution back end
- Supports multiple messaging patterns
  - Device-to-cloud telemetry
  - File upload from devices
  - Request-reply methods
- After an IoT hub receives messages from a device, it can route that message to other Azure services
- Allows for command and control

##### Azure IoT Central

![Azure IoT Central Dashboard](https://docs.microsoft.com/en-us/learn/azure-fundamentals/iot-fundamentals/media/2-identify-product-options-01-9e2f3db7.png)

- Dashboard that allows you to connect, monitor, and manage your IoT devices
- Connect new devices and watch as they begin sending telemetry or error messages
- Can watch the overall performance across all devices in aggregate
- Can set up alerts that send notifications when a specific device needs maintenance
- Can push firmware updates to the device
- Provides starter templates
- Customize the design starter templates directly in the UI
- Control your devices remotely
- Key part of IoT Central -> Device templates
  - Can connect a device without any service-side coding
- Device developers still need to create code to run on the devices
  - That code must match the device template specification

##### Azure Sphere

- End-to-end, highly secure IoT solution
- Encompasses everything from the hardware and operating system on the device to the secure method of sending messages
- Built-in communication and security features for internet-connected devices
- Three parts
  - First part
    - Azure Sphere micro-controller unit (MCU)
    - Processing the operating system and signals from attached sensors
  - Second part
    - Customized Linux operating system (OS)
    - Handles communication with the security service
    - Run the vendor's software
  - Third part
    - Azure Sphere Security Service
    - AS3
    - Its job is to make sure that the device has not been maliciously compromised
    - When the device attempts to connect to Azure, it first must authenticate
    - Certificate-based authentication
    - Established a secure channel of communication
    - AS3 pushes any OS or approved customer-developed software updates to the device

#### Analyze the decision criteria

- The criteria that experts employ when they decide which IoT service to use for a given business need
- **Is it critical to ensure that the device is not compromised?**
  - Not in every case
  - It's more critical to ensure the integrity than others
  - When security is a critical consideration in your product's
  - Azure Sphere
    - Provides a comprehensive end-to-end solution for IoT devices
    - Ensures a secure channel of communication between the device and Azure
      - Controlling everything from the hardware to the operating system and the authentication process
- **Do I need a dashboard for reporting and management?**
  - If you
    - Merely want to connect to your remote devices to receive telemetry && Occasionally push updates && You don't need any reporting capabilities
      - Azure IoT Hub
        - Programmers can still create a customized set of management tools and reports -> IoT Hub RESTful API
  - If you
    - Pre-built customizable user interface
      - IoT Central
        - Integrates with many different Azure products
        - Create a dashboard with reports
        - Management features

#### Use IoT Hub

- Tailwind Traders
  - Decided -> create high-end brand that promises a preemptive maintenance service agreement
  - Appliances will send telemetry information to a centralized location
  - Data can be analyzed and maintenance can be scheduled
  - Devices will not require remote control
  - Merely be sending their telemetry data for analysis and pro-active maintenance
  - Company wants to integrate all functionality into this existing system
- **Which service should you choose?**
  - First
    - Is it critical to ensure that the device or, in this case, each appliance, isn't compromised?
    - It's preferable, but not critical
    - It might not warrant the extra expense or engineering resources that would be required to employ Azure Sphere
  - Second
    - Do I need a dashboard for reporting and management?
    - Tailwind Traders wants to integrate the telemetry data and all other functionality into an existing maintenance request system
    - Azure IoT Central is not required
    - Azure IoT Hub is the best choice in this scenario

#### Use IoT Central

- Tailwind Traders
  - Owns a fleet of delivery vehicles
  - Transport products
    - From warehouses to distribution centers
    - From distribution centers to stores and homes
  - Looking for a complete logistics solution
  - Takes data sent from an onboard vehicle computer
  - Turns it into actionable information
  - Shipments can be outfitted with sensors from a third-party vendor
  - Collect and monitor ambient conditions
    - Temperature
    - Humidity
    - Tilt
    - Shock
    - Light
    - Location of a shipment
    - Goals
  - Shipment monitoring with real-time tracing and tracking
  - Shipment integrity with real-time ambient condition monitoring
  - Security from theft, loss, or damage of shipments
  - Geo-fencing, route optimization, fleet management, and vehicle analytics
  - Forecasting for predictable departure and arrival of shipments
  - Prefer a pre-built solution
  - Collect the sensor and vehicle computer data
  - Provide a graphical user interface that displays reports about shipments and vehicles
- **Which service should you choose?**
  - First
    - Is it critical to ensure that the device or, in this case, each appliance, isn't compromised?
      - Security was not mentioned as a critical concern
      - Vehicle computers and sensors are built by a third-party vendor
  - Second
    - Does Tailwind Traders need a dashboard for reporting and management?
      - Reporting and management dashboard is a requirement
      - Azure IoT Central is the best choice in this scenario
        - Connected Logistics starter template
          - Preconfigured to showcase the critical logistics device operations activity
- **Why not use IoT Hub?**
  - Preconfigured for its specific needs by the Connected Logistics starter template
  - Would need to do a lot of custom development

#### Use Azure Sphere

- Tailwind Traders
  - Implement a touchless point-of-sale solution for self-checkout
  - Should be, above all else, secure
  - Must be
    - Impervious to malicious code
  - Should
    - Report back vital information on the company's health
    - Allow secure updates to its software remotely
  - Decides to work with a leading engineering firm that specializes in IoT solutions
  - Wants a solution that can help it make sense of all the data that will be generated
  - Wants an easy way to push software updates to its terminals
- **Which service should you choose?**
  - First
    - Is it critical to ensure that the device or, in this case, each point-of-sale terminal, is not compromised?
      - Absolutely
      - Primary requirement
  - Next
    - Does Tailwind Traders need a dashboard for reporting and management?
      - Requires a reporting and management dashboard
      - IoT engineering firm will build a platform on top of both Azure IoT Central and Azure Sphere

### Choose the best AI service for your needs

#### Identify the product options

- Computing that allows a software system to perceive its environment and take action that maximizes its chance of successfully achieving its goals
- Two basic approaches to AI
  - _Deep learning_
    - Discover, learn, and grow through experience
  - _Machine learning_
    - Uses existing data to train a model, test it, and then apply the model to new data to forecast future behaviors, outcomes, and trends

##### Azure product options

###### Azure Machine Learning

- Platform for making predictions
- Tools and services
- Connect to data to train and test models
- Deploy and use it in real time via a web API endpoint
- You can:
  - Create a process that defines how to
  - Obtain data
  - Handle missing or bad data
  - Split the data into either a training set or test set
  - Deliver the data to the training process
  - Train and evaluate predictive models
  - Create pipelines that define where and when to run the compute-intensive experiments
  - Deploy the best-performing algorithm as an API to an endpoint
- Data scientists need complete control over the design and training of an algorithm using your own data

###### Azure Cognitive Services

- Prebuilt machine learning models
- Enable applications to:
  - See
  - Hear
  - Speak
  - Understand
  - Begin to reason
- Analyzing text for emotional sentiment
- Analyzing images to recognize objects or faces
- APIs
- Provides pretrained models
- Can be divided into the following categories:
  - Language services
    - Process natural language
    - Evaluate sentiment
    - Learn how to recognize what users want
  - Speech services
    - Convert speech into text and text into natural-sounding speech
    - Translate
    - Speaker verification and recognition
  - Vision services
    - Recognition and identification
    - Pictures , videos, and other visual content
  - Decision services
    - Personalized recommendations for each user
    - Improve each time they're used
    - Moderate content
    - Detect abnormalities

###### Azure Bot Service

- Creating virtual agents that understand and reply to questions just like a human
- Creates a virtual agent that can intelligently communicate with humans
- Behind the scenes
  - Uses other Azure services, such as Azure Cognitive Services

#### Analyze the decision criteria

- **Are you building a virtual agent that interfaces with humans via natural language?**
  - Azure Bot Service
  - Before you jump in to build a custom chat experience
    - Search for prebuilt, no-code solutions that cover common scenarios
    - Power Virtual Agents integrates with Microsoft Power Platform
    - Can use hundreds of prebuilt connectors for data input
  - Build more complex interactions with Microsoft Bot Framework
- **Do you need a service that can understand the content and meaning of images, video, or audio, or that can translate text into a different language?**
  - Azure Cognitive Services
  - General purpose
  - Work that Microsoft has already done to train and test these models
- **Do you need to predict user behavior or provide users with personalized recommendations in your app?**
  - Azure Cognitive Services Personalizer service
  - Predict their behavior and provide relevant experiences as it identifies usage patterns
  - Create your own custom Azure Machine Learning solution
- **Will your app predict future outcomes based on private historical data?**
  - Azure Machine Learning
- **Do you need to build a model by using your own data or perform a different task than those listed above?**
  - Azure Machine Learning
  - Maximum flexibility

#### Use Machine Learning for decision support systems

- Tailwind Traders e-commerce website
- Marketing team
  - Convinced that it can increase sales dramatically by suggesting add-on products that complement the items in a shopper's cart
  - Suggestions could be influenced by product availability, product profitability, and other factors
- **Which service should you choose?**
  - First -> Tailwind Traders building a virtual agent that interfaces with humans via natural language?
    - No
    - Azure Bot Service is not a good candidate
  - Second -> Does Tailwind Traders need a service that can understand the content and meaning of images, video, audio, or translate text into a different language?
    - No
    - Cognitive Services will not help the company
  - Third -> Does Tailwind Traders need to predict user behavior or provide users with personalized recommendations?
    - Yes
    - Creating recommendations -> only part of the requirement
    - Complex model
      - Historical sales data
      - Trending sales data
      - Inventory
    - Azure Cognitive Services Personalizer -> couldn't handle the entire breadth of the project alone
  - Fourth -> Will the Tailwind Traders app predict future outcomes based on private historical data?
    - Yes
    - Azure Machine Learning is likely the best choice

#### Use Cognitive Services for data analysis

- Tailwind Traders e-commerce website was available exclusively in English
- Only 80 percent of potential customers speak English
- **Which service should you choose?**
  - First -> Is Tailwind Traders building a virtual agent that interfaces with humans via natural language?
    - No
    - Azure Bot Service is not a good candidate
    - Consider using the Translator API to provide real-time translation
  - Second -> Does Tailwind Traders need a service that can understand the content and meaning of images, video, audio, or translate text into a different language?
    - Yes
    - Azure Cognitive Services Translator
  - Third -> Does Tailwind Traders need to predict user behavior or provide users with personalized recommendations?
    - No
    - Azure Cognitive Services Personalizer is not a good candidate
  - Finally -> Will the Tailwind Traders app need to predict future outcomes based on private historical data?
    - No
    - It's possible to create a Machine Learning model for multilanguage translation
      - Expensive
      - Time consuming

#### Use Bot Service for interactive chat experiences

- Customer Service team has long asked for a virtual agent to handle the vast majority of questions it gets asked
- **Which service should you choose?**
  - First -> Is Tailwind Traders building a virtual agent that interfaces with humans via natural language?
    - Yes
    - Azure Bot Service
      - Virtual agent chat experience
  - Second -> Does Tailwind Traders need a service that can understand the content and meaning of images, video, audio, or translate text into a different language?
    - Azure Cognitive Services could be used along with Bot Service to build the solution
      - QnA Maker (part of Cognitive Services)
      - Power Virtual Agents
      - Language Understanding (LUIS)
      - Translator
  - Third -> Does Tailwind Traders need to predict user behavior or provide users with personalized recommendations?
    - No
    - Azure Cognitive Services Personalizer is not a good candidate
  - Finally -> Will the Tailwind Traders app need to predict future outcomes based on private historical data?
    - No

### Choose the best Azure serverless technology for your business scenario

#### Introduction

- **Serverless computing**
  - Execution environment
  - Set up and managed for you
  - Writing code or connecting and configuring components in a visual editor
  - Never have to worry about an outage
  - Your code can scale instantly to meet demand
  - You pay based only on the actual usage

#### Identify the product options

- Serverless computing
  - Cloud-hosted execution environment
  - Abstracts the underlying hosting environment
  - There is a server (or a group of servers) that executes your code or desired functionality
  - Key idea
    - You're not responsible for setting up or maintaining the server
  - You don't have to worry about scaling it
  - You don't have to worry about outages
- Serverless app runs only when it's triggered by an event
- You're billed only for the resources you use
- Ordinarily used to handle back-end scenarios
- Responsible for
  - Sending messages from one system to another
  - Processing messages that were sent from other systems
- Not used for user-facing systems

##### Azure Functions

- Host a single method or function
- Runs in response to an event
  - HTTP request
  - New message on a queue
  - Message on a timer
- Can be written in many common programming languages
- Scales automatically
- Charges accrue only when a function is triggered
- Solid choice when demand is variable
- Stateless environment
  - Behaves as if it's restarted every time it responds to an event
- If state is required
  - Can be connected to an Azure storage account
- Can perform orchestration tasks
  - Extension called Durable Functions
- Allow developers to chain functions together while maintaining state
- Ideal when
  - Concerned only with the code that's running your service
  - Not the underlying platform or infrastructure
  - Perform work in response to an event
  - Work can be completed quickly

##### Azure Logic Apps

- Low-code/no-code development platform hosted as a cloud service
- Helps you
  - Automate and orchestrate
    - Tasks
    - Business processes
    - Workflows
    - Integrate apps, data, systems, and services across enterprises or organizations
- Covers
  - App integration
  - Data integration
  - System integration
  - Enterprise application integration (EAI)
  - Business-to-business (B2B) integration
- Web-based designer
  - Linking triggers to actions with connectors
    - A trigger is an event
    - An action is a task or step that can execute
    - If you can't find the action or connector you need, you can build your own by using custom code

##### What are the differences between these services?

- Primary difference
  - Their intent
    - Azure Functions is a serverless compute service
    - Azure Logic Apps is intended to be a serverless orchestration service
- Are priced differently
  - Azure Functions pricing
    - Based on the number of executions
    - Running time of each execution
  - Logic Apps pricing
    - Based on the number of executions
    - Type of connectors

#### Analyze the decision criteria

- **Do you need to perform an orchestration across well-known APIs?**
  - Azure Logic Apps was designed with orchestration in mind
    - From the web-based visual configurator to the pricing model
  - Azure Functions
    - Might take a considerable amount of time
- **Do you need to execute custom algorithms or perform specialized data parsing and data lookups?**
  - Azure Functions
    - Can use the full expressiveness of a programming language
    - Lets you
      - Build complex algorithms
      - Data lookup
      - Parsing operations
  - Azure Logic Apps
    - More verbose
    - Visually overwhelming
- **Do you have existing automated tasks written in an imperative programming language?**
  - Easier to port your code into the body of an Azure Functions
- **Do you prefer a visual (declarative) workflow or writing (imperative) code?**
  - Developers
    - Imperative
  - IT professionals and business analysts
    - Low-code/no-code (declarative)

### Choose the best tools to help organizations build better solutions

#### Introduction

- Microsoft has created a comprehensive set of tools that help organizations
  - Implement DevOps practices
  - Develop solutions
  - Save money while doing so

#### Understand your product options

- DevOps
  - Combines philosophies and practices to facilitate technical teams as they work toward common goals
  - Practices and processes that automate
    - Development
    - Maintenance
    - Deployment of software systems
- The aim
  - Expedite the release of software changes
  - Ensure the ongoing deployability of the system
  - Ensure that all changes meet a high quality bar
- Microsoft tools enable
  - Source-code management
  - CI/CD
  - Automate the creation of testing environments

##### Product options

- **Azure DevOps Services**
  - Suite of services that address every stage of the software development lifecycle
    - _Azure Repos_
      - Centralized source-code repository
      - Publish code for review and collaboration
    - _Azure Boards_
      - Agile project management suite
      - Includes
        - Kanban boards
        - Reporting
        - Tracking ideas
        - Work from high-level epics to work items and issues
    - _Azure Pipelines_
      - CI/CD pipeline automation tool
    - _Azure Artifacts_
      - Repository for hosting artifacts
        - Compiled source code
      - Can be fed into testing or deployment pipeline steps
    - _Azure Test Plans_
      - Automated test tool
      - Can be used in a CI/CD pipeline
      - Ensure quality before a software release
  - Began as on-premises server software
    - Evolved into SaaS
- **GitHub and GitHub Actions**
  - World's most popular code repository for open-source software
  - GitHub is a hosted version of Git
  - Functionality
    - Shared source-code repository
    - Facilitates project management
    - Supports issue reporting, discussion, and tracking
    - Features CI/CD pipeline automation tooling
    - Includes a wiki for collaborative documentation
    - Can be run from the cloud or on-premises
  - GitHub Actions
    - Enables workflow automation with triggers for many lifecycle events
    - Automating a CI/CD toolchain
  - Both Azure DevOps and GitHub allow public and private code repositories
  - GitHub
    - Lighter-weight tool than Azure DevOps
    - Focus on individual developers contributing to the open-source code
  - Azure DevOps
    - Focused on enterprise development
    - Heavier project-management and planning tools
    - Finer-grained access control
- **Azure DevTest Labs**
  - Automated means of managing the process of building, setting up, and tearing down virtual machines (VMs) that contain builds of your software projects
  - Anything you can deploy in Azure via an ARM template can be provisioned through DevTest Labs
  - Management team can restrict how many labs can be created, how long they run, and so on

#### Analyze the decision criteria

- Do you need to automate and manage test-lab creation?
- Are you building open-source software?
  - Regarding source-code management and DevOps tools, what level of granularity do you need for permissions?
  - Regarding source-code management and DevOps tools, how sophisticated does your project management and reporting need to be?
  - Regarding source-code management and DevOps tools, how tightly do you need to integrate with third-party tools?

### Choose the best tools for managing and configuring your Azure environment

#### Introduction

- Azure management tools
  - Administrators, developers, and managers
    - Perform such tasks as
      - Deploying dozens or hundreds of resources at a time
      - Configuring individual services programmatically
      - Viewing rich reports across usage, health, costs, and more
- Explore the array of Azure management tools
- Decision criteria that experts use to select the right ones

#### Identify the product options

- Two broad categories of management tools:
  - Visual tools
    - Full, visually friendly access to all the functionality of Azure
    - Might be less useful
    - Large deployment of resources
    - Interdependencies and configuration options
  - Code-based tools
    - Might take time to understand the right commands and parameters
    - The code that performs setup and configuration can be stored, versioned, and maintained along with application source code
    - Infrastructure as code
- Two approaches to infrastructure as code:
  - Imperative code
    - Details each individual step that should be performed to achieve a desired outcome
  - Declarative code
    - Details only a desired outcome, and it allows an interpreter to decide how to best achieve that outcome

##### The Azure portal

- Web-based user interface
- Access virtually every feature of Azure
- Provides a friendly, graphical UI

##### The Azure mobile app

- Provides iOS and Android access to your Azure resources
- You can
  - Monitor the health and status of your Azure resources
  - Check for alerts, quickly diagnose and fix issues, and restart a web app or virtual machine (VM)
  - Run the Azure CLI or Azure PowerShell commands to manage your Azure resources

##### Azure PowerShell

- Execute commands called cmdlets (pronounced command-lets )
- Call the Azure Rest API to perform every possible management task
- Cmdlets can be executed
  - Independently
  - Script file
- Orchestrate
  - Routine setup, teardown, and maintenance of a single resource or multiple connected resources
  - Deployment of an entire infrastructure
  - From imperative code
- Available for Windows, Linux, and Mac
- You can access it in a web browser via Azure Cloud Shell

##### The Azure CLI

- Executable program
- Execute commands in Bash
- Commands call the Azure Rest API to perform every possible management task in Azure
- Can run the commands independently or combined into a script
- Run on Windows, Linux, and Mac
- Can be accessed in a web browser via Cloud Shell
- Primary difference is the syntax you use

##### ARM templates

- Azure Resource Manager templates (ARM templates)
- Imperative code in Azure PowerShell or the Azure CLI
- Describe the resources you want to use in a declarative JSON format
- Entire ARM template is verified before any code is executed
- Ensure that the resources will be created and connected correctly
- Orchestrates the creation of those resources in parallel
- Needs only to define the desired state and configuration of each resource

#### Analyze the decision criteria

- **Do you need to perform one-off management, administrative, or reporting actions?**
  - For one-off scenarios, you may prefer more agile tools like PowerShell, Azure CLI scripts, or the Azure portal
  - If you're just learning Azure and/or need to set up and manage resources infrequently -> Azure portal
  - To quickly find the settings and information you want to work with -> Azure CLI or PowerShell
  - It's likely the best choice when a laptop isn't readily available -> Azure mobile app
- **Do you need a way to repeatedly set up one or more resources and ensure that all the dependencies are created in the proper order?**
  - ARM templates
  - Define your application's infrastructure requirements for a repeatable deployment
  - Validation step ensures that all resources can be created in the proper order
- **When you're scripting, do you come from a Windows administration or Linux administration background?**
  - Cloud administrators come from a Windows administration background -> PowerShell
  - Cloud administrators come from a Linux administration background -> Azure CLI

### Choose the best monitoring service for visibility, insight, and outage mitigation

- React quickly to outages
- Research intermittent issues
- Optimize your usage
- Handling future planned downtime

#### Identify your product options

##### Azure Advisor

- Evaluates your Azure resources
- Makes recommendations to help
- Improve reliability, security, and performance
- Achieve operational excellence
- Reduce costs
- Designed to help you save time on cloud optimization
- Advisor dashboard displays personalized recommendations for all your subscriptions
- Recommendations are divided into five categories
  - Reliability -> ensure and improve the continuity of your business-critical applications
  - Security -> detect threats and vulnerabilities that might lead to security breaches
  - Performance -> improve the speed of your applications
  - Cost -> optimize and reduce your overall Azure spending
  - Operational Excellence -> achieve process and workflow efficiency, resource manageability, and deployment best practices

##### Azure Monitor

- Platform for
  - Collecting
  - Analyzing
  - Visualizing
  - Taking action based on the metric and logging data from your entire Azure and on-premises environment
- ![Azure Monitor](https://docs.microsoft.com/en-us/learn/azure-fundamentals/monitoring-fundamentals/media/2-identify-product-options-01.png)
  - On the left -> list of the sources of logging and metric data that can be collected from application to operating system and network
  - In the center -> how the logging and metric data is stored
  - On the right -> data is used
- **Azure Application Insights**
  - Service for sending telemetry information from application source code to Azure
  - Uses Azure Monitor under the hood
  - Application developers gain deep insights into an application's operations
    - Diagnose errors without having to wait for users to report them

##### Azure Service Health

- Provides a personalized view of the health of the Azure services, regions, and resources
- Displays both major and smaller, localized issues that affect you
- Event types
  - Service issues -> affect you right now
  - Planned maintenance -> drill down to the affected services, regions, and details to show how an event will affect you and what you need to do
  - Health advisories -> issues that require you to act to avoid service interruption

#### Analyze the decision criteria

- **Do you need to analyze how you're using Azure to reduce costs, improve resilience, or harden your security?**
  - _Azure Advisor_
- **Do you want to monitor Azure services or your usage of Azure?**
  - _Azure Service Health_
    - Current status of the Azure services
    - Upcoming planned outages
    - Services that will be sunset
  - _Azure Monitor_
    - Keep track of the performance or issues related to your specific VM or container instances, databases, your applications
- **Do you want to measure custom events alongside other usage metrics?**
  - _Azure Monitor_
    - Measure custom events alongside other collected telemetry data
    - Added in the source code of your software applications
- **Do you need to set up alerts for outages or when autoscaling is about to deploy new instances?**
  - _Azure Monitor_
    - Set up alerts for key events that are related to your specific resources

## Describe general security and network security features

### Protect against security threats on Azure

#### Protect against security threats by using Azure Security Center

##### What's Azure Security Center?

- Monitoring service
- Provides visibility of your security posture
- Azure and on-premises
- Security posture
  - Cybersecurity policies and controls, as well as how well you can predict, prevent, and respond to security threats
- Security Center can:
  - Monitor security settings across on-premises and cloud workloads
  - Automatically apply required security settings to new resources
  - Provide security recommendations
  - Monitor your resources and perform automatic security assessments to identify potential vulnerabilities
  - Use machine learning to detect and block malware
  - Adaptive application controls
  - Define rules that list allowed applications to ensure that only applications you allow can run
  - Detect and analyze potential inbound attacks and investigate threats and any post-breach activity
  - Provide just-in-time access control for network ports

##### Understand your security posture

- ![Security Center Compliance](https://docs.microsoft.com/en-us/learn/azure-fundamentals/protect-against-security-threats-azure/media/2-security-center-compliance-32866f57.png)
- **Resource security hygiene** section
  - Health of its resources from a security perspective
  - Recommendations are categorized as low, medium, and high
- **What's secure score?**
  - Measurement of an organization's security posture
  - Based on security controls
  - Based on the percentage of security controls that you satisfy
  - Score improves when you remediate all of the recommendations
  - Helps you:
    - Report
    - Improve your security posture
      - Providing
      - Discoverability
      - Visibility
      - Guidance
      - Control
    - Compare with benchmarks
      - Establish key performance indicators (KPIs)

##### Protect against threats

- Security Center includes advanced cloud defense capabilities:
  - **Just-in-time VM access**
    - Blocks traffic by default to specific network ports of VMs
    - Allows traffic for a specified time when an admin requests and approves it
  - **Adaptive application controls**
    - Control which applications are allowed to run on its VMs
    - Uses machine learning to look at the processes running on a VM
    - Provides alerts that inform the company about unauthorized applications
  - **Adaptive network hardening**
    - Monitor the internet traffic patterns of the VMs
    - Compare those patterns with the company's current network security group (NSG)
  - **File integrity monitoring**
    - Configure the monitoring of changes to important files

##### Respond to security alerts

- Automated response with a workflow automation
  - Uses Azure Logic Apps and Security Center connectors

#### Detect and respond to security threats by using Azure Sentinel

- Security information and event management (SIEM) system
  - Aggregates security data from many different sources
  - Capabilities for threat detection and response

##### Azure Sentinel

- Microsoft's cloud-based SIEM system
- Capabilities
  - Collect cloud data at scale
  - Detect previously undetected threats -> minimize false positives
  - Investigate threats with artificial intelligence -> examine suspicious activities
  - Respond to incidents rapidly -> built-in orchestration and automation
- **Connect your data sources**
  - Built-in connectors or industry-standard log formats and APIs
    - Connect Microsoft solutions
      - Real-time integration
    - Connect other services and solutions
      - Available for common non-Microsoft services and solutions
    - Connect industry-standard data sources
      - Supports data from other sources that use the Common Event Format (CEF) messaging standard, Syslog, or REST API
- **Detect threats**
  - Built in analytics
    - Templates designed by Microsoft
    - Can be customized
    - Search across the environment for any activity that looks suspicious
  - Custom analytics
    - Rules that you create to search for specific criteria within your environment
- **Investigate and respond**
  - Investigation graph
  - Review information from entities directly connected to the alert,
  - ![Investigation graph example](https://docs.microsoft.com/en-us/learn/azure-fundamentals/protect-against-security-threats-azure/media/3-investigate-incidents-54765923.png)
  - _Azure Monitor Workbooks_
    - Automate responses to threats
    - Can be run manually or automatically when a rule triggers an alert

#### Store and manage secrets by using Azure Key Vault

- **Azure Key Vault**
  - Storing an application's secrets in a single, central location
  - Provides secure access to sensitive information
  - Access control and logging capabilities

##### What can Azure Key Vault do?

- Manage secrets
  - Securely store and tightly control access to tokens, passwords, certificates, API keys, and other secrets
- Manage encryption keys
  - Key management solution
  - Create and control the encryption keys that are used to encrypt your data
- Manage SSL/TLS certificates
  - Provision, manage, and deploy your public and private Secure Sockets Layer/Transport Layer Security (SSL/TLS) certificates
- Store secrets backed by hardware security modules (HSMs)

![Key Vault certificates](https://docs.microsoft.com/en-us/learn/azure-fundamentals/protect-against-security-threats-azure/media/4-key-vault-certificates-b32bfbfe.png)

##### What are the benefits of Azure Key Vault?

- Centralized application secrets
  - Control their distribution, and reduces the chances that secrets are accidentally leaked
- Securely stored secrets and keys
  - Access to Key Vault requires proper authentication and authorization
- Access monitoring and access control
  - Monitor and control access to your application secrets
- Simplified administration of application secrets
  - Makes it easier to enroll and renew certificates from public certificate authorities (CAs)
  - Scale up and replicate content within regions and use standard certificate management tools
- Integration with other Azure services
  - Integrate Key Vault with storage accounts, container registries, event hubs, and many more Azure services.
  - Securely reference the secrets stored in Key Vault

#### Host your Azure virtual machines on dedicated physical servers by using Azure Dedicated Host

- VMs run on shared hardware
- VM workloads are isolated from workloads that other Azure customers run
- **Azure Dedicated Host**
  - Provides dedicated physical servers to host your Azure VMs for Windows and Linux
- Diagram that shows how VMs relate to dedicated hosts and host groups
  - ![Dedicated hosts](https://docs.microsoft.com/en-us/learn/azure-fundamentals/protect-against-security-threats-azure/media/6-dedicated-hosts-cab8e670.png)
- _Dedicated host_
  - Mapped to a physical server in an Azure datacenter
- _Host group_
  - Collection of dedicated hosts

##### What are the benefits of Azure Dedicated Host?

- Visibility into, and control over, the server infrastructure
- Helps address compliance requirements
- Lets you choose the number of processors, server capabilities, VM series, and VM sizes within the same host

##### Availability considerations for Dedicated Host

- For high availability, you can provision multiple hosts in a host group
- Maintenance control
  - Control when regular maintenance updates occur

##### Pricing considerations

- You're charged per dedicated host, independent of how many VMs you deploy to it

### Secure network connectivity on Azure

#### What is defense in depth?

- Objective of defense in depth
  - Protect information
  - Prevent it from being stolen by those who aren't authorized to access it
- Defense-in-depth strategy

  - Slow the advance of an attack that aims at acquiring unauthorized access to data

- **Layers of defense in depth**
  - ![Defense in depth](https://docs.microsoft.com/en-us/learn/azure-fundamentals/secure-network-connectivity-azure/media/2-defense-depth.png)
  - Each layer provides protection so that if one layer is breached, a subsequent layer is already in place to prevent further exposure
  - Role of each layer:
    - Physical security
      - Protect computing hardware in the datacenter
      - Securing access to buildings
      - Controlling access to computing hardware within the datacenter
    - Identity and access
      - Controls access to infrastructure and change contro l
      - It's important to:
        - Control access to infra
        - Use single sign-on (SSO) and multifactor authentication
        - Audit events and changes
    - Perimeter
      - Distributed denial of service (DDoS) protection
      - It's important to:
        - Use DDoS protection
        - Use perimeter firewalls
        - It's about protecting from network-based attacks
    - Network
      - Limits communication between resources
      - It's important to:
        - Limit communication between resources
        - Deny by default
        - Restrict inbound internet access and limit outbound access
        - Secure connectivity to on-premises networks
      - Reduce the risk of an attack spreading
    - Compute
      - Secures access to virtual machines
      - It's important to :
        - Secure access to virtual machines
        - Implement endpoint protection on devices
          - Keep systems patched and current
    - Application
      - Helps ensure that applications are secure and free of security vulnerabilities
      - It's important to:
        - Ensure that applications are
          - Secure
          - Free of vulnerabilities
        - Store sensitive application secrets in a secure storage medium
    - Data
      - Controls access to business and customer data
- **Security posture**
  - Organization's ability to protect from and respond to security threats
  - Common principles
    - _Confidentiality_
      - Principle of least privilege
      - Restricting access to information only to individuals explicitly granted access
    - _Integrity_
      - Prevent unauthorized changes to information
    - _Availability_
      - Ensure that services are functioning and can be accessed only by authorized users

#### Protect virtual networks by using Azure Firewall

- Firewall

  - Network security device
  - Monitors incoming and outgoing network traffic
  - Decides whether to allow or block specific traffic
  - Based on a defined set of security rules

- **What's Azure Firewall?**
  - Cloud-based network security service
  - Helps protect resources in your Azure virtual networks
  - Basic Azure Firewall implementation:
    - ![Diagram that shows a basic Azure Firewall implementation](https://docs.microsoft.com/en-us/learn/azure-fundamentals/secure-network-connectivity-azure/media/3-firewall-overview.png)
  - Stateful firewall
    - Analyzes the complete context of a network connection
    - Features
      - High availability
      - Unrestricted cloud scalability
  - Provides a central location to
    - Create
    - Enforce
    - Log application and network connectivity policies
  - Uses a static (unchanging) public IP address
  - Integrated with Azure Monitor to enable logging and analytics
  - Provides
    - Inbound Destination Network Address Translation (DNAT) support
- **What can I configure with Azure Firewall?**
  - You can configure:
    - Application rules that define fully qualified domain names (FQDNs)
    - Network rules that define source address, protocol, destination port, and destination address
    - Network Address Translation (NAT) rules
      - Translate inbound requests
  - Azure Application Gateway, Azure Front Door and Azure Content Delivery Network
    - Provides
      - Web application firewall (WAF)
        - Provides
          - Centralized, inbound protection

#### Protect from DDoS attacks by using Azure DDoS Protection

- **What are DDoS attacks?**
  - Distributed denial of service
  - Attempts to overwhelm and exhaust an application's resources
  - Application slow or unresponsive to legitimate users
- **What is Azure DDoS Protection?**
  - Protect your Azure resources from DDoS attacks
  - Uses the scale and elasticity of Microsoft's global network
  - Analyzing and discarding DDoS traffic at the Azure network edge
  - This diagram shows network traffic flowing into Azure from both customers and an attacker:
    - ![Network traffic flowing into Azure](https://docs.microsoft.com/en-us/learn/azure-fundamentals/secure-network-connectivity-azure/media/4-distributed-denial-service.png)
  - Identifies the attacker's attempt
  - Blocks further traffic from them
  - Ensuring that traffic never reaches Azure resources
  - A cleverly designed DDoS attack can cause you to increase your resource allocation
  - DDoS Protection Standard
  - Ensure that the network load you process reflects customer usage
- **What service tiers are available to DDoS Protection?**
  - _Basic_
    - Automatically enabled for free
    - Always-on traffic monitoring
    - Real-time mitigation of common network-level attacks
    - Same defenses that Microsoft's online services use
    - Ensures that Azure infrastructure itself is not affected during a large-scale DDoS attack
  - _Standard_
    - Provides additional mitigation capabilities
    - Specifically to Azure Virtual Network resources
    - Always-on traffic monitoring
    - Real-time mitigation of common network-level attacks
    - Provides the same defenses that Microsoft's online services use
    - Protection policies are tuned through
    - Dedicated traffic monitoring
    - Machine learning algorithms
    - Policies are applied to public IP addresses
- **What kinds of attacks can DDoS Protection help prevent?**
  - _Volumetric attacks_
    - Flood the network layer with a substantial amount of seemingly legitimate traffic
  - _Protocol attacks_
    - Exploiting a weakness in the layer 3 and layer 4 protocol stack
  - _Resource-layer (application-layer) attacks (only with web application firewall)_
    - Target web application packets
    - Disrupt the transmission of data between hosts
- DDoS Protection Standard protects the WAF from volumetric and protocol attacks

#### Filter network traffic by using network security groups

- **What are network security groups?**
  - Filter network traffic to and from Azure resources within an Azure virtual network
  - Like an internal firewall
  - Can contain multiple inbound and outbound security rules
- **How do I specify NSG rules?**

| Property              | Description                                                                                                               |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| Name                  | A unique name for the NSG.                                                                                                |
| Priority              | A number between 100 and 4096. Rules are processed in priority order, with lower numbers processed before higher numbers. |
| Source or Destination | A single IP address or IP address range, service tag, or application security group.                                      |
| Protocol              | TCP, UDP, or Any.                                                                                                         |
| Direction             | Whether the rule applies to inbound or outbound traffic.                                                                  |
| Port Range            | A single port or range of ports.                                                                                          |
| Action                | Allow or Deny.                                                                                                            |

- When you create a network security group
  - Azure creates a series of default rules to provide a baseline level of security
  - Can't remove the default rules
  - Can override them by creating new rules with higher priorities

#### Combine Azure services to create a complete network security solution

- Recommendations on how to combine Azure services to create a complete network security solution
- **Secure the perimeter layer**
  - Azure DDoS Protection
    - Filter large-scale attacks
  - Azure Firewall
    - Identify and alert on malicious attacks
- **Secure the network layer**
  - Network security groups
    - Create rules that define allowed inbound and outbound communication
  - Recommended practices:
    - Limit communication between resources
      - Segmenting your network
        - Configuring access controls
    - Deny by default
    - Restrict inbound internet access
    - Limit outbound where appropriate
    - Implement secur connectivity to on-premises networks
- **Combine services**
  - Combine Azure networking and security services
  - Two ways you can combine services:
    - _Network security groups and Azure Firewall_
      - Azure Firewall complements Network security groups
      - Provide better defense-in-depth network security
      - Network security groups
        - Provide distributed network-layer traffic filtering
        - Within virtual networks in each subscription
      - Azure Firewall
        - Provides network-level and application-level protection across different subscriptions and virtual networks
    - _Azure Application Gateway web application firewall and Azure Firewall_
      - Web application firewall (WAF)
        - Feature of Azure Application Gateway
        - Centralized, inbound protection against common exploits and vulnerabilities
      - Azure Firewall
        - Inbound protection for non-HTTP/S protocols
        - Outbound network-level protection for all ports and protocols
        - Application-level protection for outbound HTTP/S

## Describe identity, governance, privacy, and compliance features

### Secure access to your applications by using Azure identity services

#### Compare authentication and authorization

- **Authentication (AuthN)**
  - Process of establishing the identity of a person or service that wants to access a resource
  - Act of challenging a party for legitimate credentials
  - Basis for creating a security principal for identity and access control
  - Establishes whether the user is who they say they are
- **Authorization (AuthZ)**
  - Process of establishing what level of access an authenticated person or service has
- **How are authentication and authorization related?**
  - Diagram that shows the relationship between authentication and authorization:
    - ![Relationship between authentication and authorization](https://docs.microsoft.com/en-us/learn/azure-fundamentals/secure-access-azure-identity-services/media/2-id-card-access.png)

#### What is Azure Active Directory?

- Provides identity services that enable your users to sign in and access
  - Microsoft cloud applications
  - Cloud applications that you develop
- Supports single sign-on (SSO)
- **How does Azure AD compare to Active Directory?**
  - Active Directory is related to Azure AD
  - Some key differences
    - _Active Directory_
      - Identity and access management
      - Managed by your own organization
    - _Azure AD_
      - Cloud-based identity and access management
      - Control the identity accounts
      - Microsoft ensures that the service is available globally
  - Connect Active Directory with Azure AD
    - Help protect you by detecting suspicious sign-in attempts at no extra cost
- **Who uses Azure AD?**
  - _IT administrators_
    - Control access to applications and resources
  - _App developers_
    - Provide a standards-based approach for adding functionality to applications
    - SSO functionality
    - Enabling an app to work with a user's existing credentials
  - _Users_
    - Manage their identities
  - _Online service subscribers_
    - Tenant
      - Representation of an organization
      - Has its own identity
  - Each Microsoft 365, Office 365, Azure, and Dynamics CRM Online tenant is automatically an Azure AD tenant
  - Screenshot of what an IT administrator might see in the Azure portal when working with Active Directory:
    - ![IT administrator view of Active Directory](https://docs.microsoft.com/en-us/learn/azure-fundamentals/secure-access-azure-identity-services/media/3-azure-active-directory.png)
- **What services does Azure AD provide?**
  - _Authentication_
    - Verifying identity to access applications and resources
    - Self-service password reset
    - Multifactor authentication
    - Banned passwords
    - Smart lockout services
  - _Single sign-on_
    - Only one username and one password to access multiple applications
  - _Application management_
  - _Device management_
    - Supports the registration of devices
    - Enables devices to be managed through tools like Microsoft Intune
    - Allows for device-based Conditional Access policies
    - Restrict access attempts to only those coming from known devices
- **What kinds of resources can Azure AD help secure?**
  - External and internal resources
    - _External resources_
      - Microsoft Office 365
      - Azure portal
      - (SaaS) applications
    - _Internal resources_
      - Apps on your corporate network and intranet
- **What's single sign-on?**
  - Enables a user to sign in one time
  - Use that credential to access multiple resources and applications
  - Need to remember only one ID and one password
  - Single identity that's tied to the user
  - Simplifies the security model
  - Reduces the effort needed to change or disable accounts
  - Easier for users to manage their identities
  - Increases your security capabilities
- **How can I connect Active Directory with Azure AD?**
  - Most popular method
    - Azure AD Connect
      - Synchronizes user identities between on-premises Active Directory and Azure AD
      - Can use features
      - SSO
      - Multifactor authentication
      - Self-service password reset
      - Diagram that shows how Azure AD Connect fits between on-premises Active Directory and Azure AD:
        - ![How Azure AD Connect fits between on-premises Active Directory and Azure AD](https://docs.microsoft.com/en-us/learn/azure-fundamentals/secure-access-azure-identity-services/media/3-azure-ad-connect.png)

#### What are multifactor authentication and Conditional Access?

- **What's multifactor authentication?**
  - Process where a user is prompted during the sign-in process for an additional form of identification
  - Code on their mobile phone or a fingerprint scan
  - Additional security for your identities
    - Requiring two or more elements to fully authenticate
  - Three categories:
    - _Something the user knows_
      - Email address and password
    - _Something the user has_
      - Code that's sent to the user's mobile phone
    - _Something the user is_
      - Biometric property, such as a fingerprint or face scan
  - Increases identity security by limiting the impact of credential exposure
- **What's Azure AD Multi-Factor Authentication?**
  - Service that provides multifactor authentication capabilities
  - Additional form of authentication during sign-in
  - These services provide Azure AD Multi-Factor Authentication capabilities:
    - _Azure Active Directory_
      - Azure Active Directory free edition
        - Azure AD Multi-Factor Authentication for administrators with the global admin level of access
        - Microsoft Authenticator app, phone call, or SMS code
      - Azure Active Directory Premium (P1 or P2 licenses)
        - Comprehensive and granular configuration of Azure AD Multi-Factor Authentication
    - _Multifactor authentication for Office 365_
- **What's Conditional Access?**
  - Tool that Azure Active Directory uses to allow (or deny) access to resources based on identity signals
    - Who the user is
    - Where the user is
    - What device the user is requesting access from
  - Provides a more granular multifactor authentication experience for users
    - Example
      - User might not be challenged for second authentication factor if they're at a known location
      - They might be challenged for a second authentication factor if their sign-in signals are unusual or they're at an unexpected location
  - Diagram that illustrates this flow:
    - ![Conditional Access flow](https://docs.microsoft.com/en-us/learn/azure-fundamentals/secure-access-azure-identity-services/media/4-conditional-access-signal-decision-enforcement.png)
  - The action is to allow access or require the user to provide a second form of authentication
- **When can I use Conditional Access?**
  - Useful when you need to:
    - _Require multifactor authentication to access an application_
      - All users require multifactor authentication or only certain users
      - All networks or only untrusted networks
    - _Require access to services only through approved client applications_
    - _Require users to access your application only from managed devices_
    - _Block access from untrusted sources, such as access from unknown or unexpected locations._
  - What If tool
    - Helps you plan and troubleshoot your Conditional Access policies
    - Model your proposed Conditional Access policies across recent sign-in attempts
    - Test your proposed Conditional Access policies before you implement them
- **Where is Conditional Access available?**
  - Azure AD Premium P1 or P2 license
  - Microsoft 365 Business Premium license

### Build a cloud governance strategy on Azure

- _Governance_
  - General process of establishing rules and policies and ensuring that those rules and policies are enforced
  - Most beneficial when you have:
    - Multiple engineering teams working in Azure
    - Multiple subscriptions to manage
    - Regulatory requirements that must be enforced
    - Standards that must be followed for all cloud resources

#### Control access to cloud resources by using Azure role-based access control

- Control access
- Built-in roles that describe common access rules for cloud resources
- Can also define your own roles
- Each role has an associated set of access permissions that relate to that role
- **How is role-based access control applied to resources?**
  - Applied to a scope
    - Resource or set of resources
  - Diagram that shows the relationship between roles and scopes:
    - ![Relationship between roles and scopes](https://docs.microsoft.com/en-us/learn/azure-fundamentals/build-cloud-governance-strategy-azure/media/4-role-scope-0223bfae.png)
  - Scopes include:
    - A management group
    - A single subscription
    - A resource group
    - A single resource
  - Grant access at a parent scope -> Permissions are inherited by all child scopes
    - For example:
      - Assign the Owner role to a user at the management group scope -> Can manage everything in all subscriptions within the management group
- **How is Azure RBAC enforced?**
  - Enforced on any action that's initiated against an Azure resource
  - Passes through Azure Resource Manager
    - Management service
    - Organize and secure your cloud resources
  - Doesn't enforce access permissions at the application or data level
    - Must be handled by your application
  - Uses an allow model
- **Who does Azure RBAC apply to?**
  - Can apply
    - Individual person
    - Group
    - Special identity types
      - Used by applications and services to automate access to Azure resources
- **How do I manage Azure RBAC permissions?**
  - Access control (IAM) pane in the Azure portal
  - Following screenshot shows an example of the Access control (IAM) pane:
    - ![Screenshot of an example of the Access Control (IAM) pane](https://docs.microsoft.com/en-us/learn/azure-fundamentals/build-cloud-governance-strategy-azure/media/4-role-based-access-control-blade-360b5130.png)

#### Prevent accidental changes by using resource locks

- Prevents resources from being accidentally deleted or changed
- Risk that people with the right level of access could delete critical cloud resources
- Warning system that reminds you that a resource should not be deleted or changed
- **How do I manage resource locks?**
  - Can manage resource locks from
    - Azure portal
    - PowerShell
    - Azure CLI
    - Azure Resource Manager template
  - To view, add, or delete locks in the Azure portal
  - Settings section of any resource's Settings pane
  - Example that shows how to add a resource lock from the Azure portal:
    - ![How to add a resource lock from the Azure Portal](https://docs.microsoft.com/en-us/learn/azure-fundamentals/build-cloud-governance-strategy-azure/media/7-portal-add-lock-ebc3d24c.png)
- **What levels of locking are available?**
  - _CanNotDelete_
    - Can still read and modify a resource
    - Can't delete the resource without first removing the lock
  - _ReadOnly_
    - Can read a resource
    - Can't delete or change the resource
    - Restricting all authorized users to the permissions granted by the Reader role in Azure RBAC
- **How do I delete or change a locked resource?**
  - First remove the lock
  - After -> Can apply any action you have permissions to perform
  - Helps protect your administrators from doing something they might not have intended to do
    - Regardless of RBAC permissions
- **Combine resource locks with Azure Blueprints**
  - What if a cloud administrator accidentally deletes a resource lock?
    - _Azure Blueprints_
      - Define the set of standard Azure resources that your organization requires
      - Can automatically replace the resource lock if that lock is removed

#### Organize your Azure resources by using tags

- **Resource tags**
  - Provide extra information
  - Metadata
    - About your resources
  - Useful for:
    - Resource management
      - Locate and act on resources that are associated with specific workloads, environments, business units, and owners
    - Cost management and optimization
      - Group resources so that you can report on costs, allocate internal cost centers, track budgets, and forecast estimated cost
    - Operations management
      - Group resources according to how critical their availability is to your business
      - Formulate service-level agreements (SLAs)
    - Security
      - Classify data by its security level, such as public or confidential
    - Governance and regulatory compliance
      - Identify resources that align with governance or regulatory compliance requirements
    - Workload optimization and automation
      - Visualize all of the resources that participate in complex deployments
- **How do I manage resource tags?**
  - Add, modify, or delete resource tags
  - Through PowerShell, the Azure CLI, Azure Resource Manager templates, the REST API, or the Azure portal
  - Can also manage tags by using Azure Policy
    - Ensure that a resource inherits the same tags as its parent resource group
    - Enforce tagging rules and conventions
  - Resource tag consists of a name and a value
    - Example
      - ![Example of names and values for tags](https://docs.microsoft.com/en-us/learn/azure-fundamentals/build-cloud-governance-strategy-azure/media/8-vm-tags-7c63fa8a.png)
  - Can run queries
    - From PowerShell or the Azure CLI
    - List all resources that contain these tags

#### Control and audit your resources by using Azure Policy

- Service in Azure that enables
  - Create, assign, and manage policies that control or audit your resources
- Enforce different rules across all of your resource configurations
  - Configurations stay compliant with corporate standards
- **How does Azure Policy define policies?**
  - Define
    - Individual policies
    - Groups of related policies (initiatives)
  - Evaluates your resources
  - Highlights resources that aren't compliant with the policies you've created
  - Prevent noncompliant resources from being created
  - Comes with built-in policy and initiative definitions for Storage, Networking, Compute, Security Center, and Monitoring
  - Can automatically remediate noncompliant resources and configurations
  - Integrates with Azure DevOps by applying any continuous integration and delivery pipeline policies
- **Azure Policy in action**
  - Implementing a policy in Azure Policy involves three tasks:
    - _Task 1. Create a policy definition_
      - Expresses
        - What to evaluate
        - What action to take
      - Some example policy definitions:
        - Allowed virtual machine SKUs
          - Specify a set of VM SKUs that your organization can deploy
        - Allowed locations
          - Restrict the locations that your organization can specify when it deploys resources
        - MFA should be enabled on accounts with write permissions on your subscription
        - CORS should not allow every resource to access your web applications
          - Allows only required domains to interact with your web app
        - System updates should be installed on your machines
    - _Task 2. Assign the definition to resources_
      - Implement your policy definitions
      - Policy assignment
        - Policy definition that takes place within a specific scope
          - Management group
          - Single subscription
          - Resource group
        - Inherited by all child resources within that scope
        - Can exclude a subscope from the policy assignment
    - _Task 3. Review the evaluation results_
      - Resource is marked as compliant or noncompliant
      - Review the noncompliant policy results
        - Take any action that's needed
      - Happens about once per hour
- **What are Azure Policy initiatives?**
  - Way of grouping related policies together
  - Contains all of the policy definitions
  - Example
    - Azure Policy includes an initiative named Enable Monitoring in Azure Security Center
    - Following policy definitions are included:
      - Monitor unencrypted SQL Database in Security Center
      - Monitor OS vulnerabilities in Security Center
      - Monitor missing Endpoint Protection in Security Center
- **How do I define an initiative?**
  - Using
    - Azure portal
    - Command-line tools
  - Built-in initiatives
  - Custom policy definition
  - Following image shows a few example Azure Policy initiatives in the Azure portal
    - ![Example of Azure Policy initiatives in the Azure Portal](https://docs.microsoft.com/en-us/learn/azure-fundamentals/build-cloud-governance-strategy-azure/media/3-define-initiatives-a834dde7.png)
- **How do I assign an initiative?**
  - Like a policy assignment
  - Initiative definition that's assigned to a specific scope
  - Enables you to increase the number of policies over time

#### Govern multiple subscriptions by using Azure Blueprints

- Define a repeatable set of governance tools and standard Azure resources that your organization requires
- Orchestrates the deployment of various resource templates and other artifacts, such as:
  - Policy assignments
  - Azure Resource Manager templates
  - Resource groups
- Scale their governance practices throughout the organization
- Implementing a blueprint
  - Three steps:
    - Create an Azure blueprint
    - Assign the blueprint
    - Track the blueprint assignments
- Creates a record that associates a resource with the blueprint
- Are also versioned
  - Track and comment on changes
- **What are blueprint artifacts?**
  - Each component in the blueprint definition
  - Contain one or more parameters that you can configure
  - Can specify a parameter's value when you create the blueprint definition or when you assign the blueprint definition to a scope
- **ISO 27001 compliance**
  - Standard that applies to the security of IT systems
  - Azure Blueprints has several built-in blueprint definitions that relate to ISO 27001
  - Following image shows artifacts that are created when you run an ISO 27001 blueprint from a template:
    - ![Artifacts that are created when you run an ISO 27001 blueprint](https://docs.microsoft.com/en-us/learn/azure-fundamentals/build-cloud-governance-strategy-azure/media/10-iso-27001-shared-blueprint-dc443de7.png)
  - Blueprint deploys
    - Artifacts to any existing subscriptions within the management group

#### Accelerate your cloud adoption journey by using the Cloud Adoption Framework for Azure

- Guidance to help with your cloud adoption journey
- Helps you create and implement the business and technology strategies needed to succeed in the cloud
- **What's in the Cloud Adoption Framework?**
  - Consists of
    - Tools
    - Documentation
    - Proven practices
  - Includes these stages:
    - !(Cloud Adoption Framework stages)[https://docs.microsoft.com/en-us/learn/azure-fundamentals/build-cloud-governance-strategy-azure/media/2-framework-stages-9b54ccbe.png]
  - Govern stage
    - Focuses on cloud governance
  - Cloud Adoption Framework breaks out each stage into further exercises and steps
- **Define your strategy**
  - Answer
    - Why you're moving to the cloud?
    - What you want to get out of cloud migration?
  - Should
    - Understand cloud economics
    - Consider business impact, turnaround time, global reach, performance, and more
  - Steps in this stage:
    - _Define and document your motivations_
    - _Document business outcomes_
    - _Evaluate financial considerations_
      - Identify the return expected from a specific investment
    - _Understand technical considerations_
      - Evaluate technical considerations through the completion of first technical project
- **Make a plan**
  - Maps your aspirational goals to specific actions
  - Ensure that your efforts map to the desired business outcomes
  - Steps in this stage:
  - _Digital estate_
    - Create an inventory
      - Existing digital assets and workloads -> plan to migrate to the cloud
  - _Initial organizational alignment_
    - Ensure that the right people are involved
      - Technical standpoint
      - Cloud governance standpoint
  - _Skills readiness plan_
    - Helps individuals -> build the skills -> operate in the cloud
  - _Cloud adoption plan_
    - Brings together
      - Development
      - Operations
      - Business
    - Shared cloud adoption goal
- **Ready your organization**
  - Create a landing zone
  - Environment in the cloud
  - Begin hosting your workloads
  - Steps in this stage:
  - _Azure setup guide_
    - Review the Azure setup guide
    - Become familiar with the tools and approaches to create a landing zone
  - _Azure landing zone_
    - Build out the Azure subscriptions
    - Support each of the major areas of your business
    - Includes
      - Cloud infrastructure
      - Governance
      - Accounting
      - Security capabilities
  - _Expand the landing zone_
    - Refine
    - Ensure that it meets need of
      - Operations
      - Governance
      - Security
  - _Best practices_
    - Recommended and proven practices
    - Ensure that your cloud migration efforts -> scalable and maintainable
- **Adopt the cloud**
  - Begin to migrate your applications to the cloud
  - Two parts:
    - Migrate
      - _Migrate your first workload_
        - Deploy your first project to the cloud
      - _Migration scenarios_
        - Explore more complex migration scenarios
      - _Best practices_
        - Azure cloud migration best practices checklist
      - _Process improvements_
        - Make the migration process scale
        - Requiring less effort
    - Innovate
      - _Business value consensus_
        - Investments in new innovations
        - Add value to the business
        - Meet customer needs
      - _Azure innovation guide_
        - Accelerate development
        - Build a MVP
      - _Best practices_
        - Verify that your progress maps to recommended practices
      - _Feedback loops_
        - Check in frequently with your customers
- **Govern and manage your cloud environments**
  - Form
    - Cloud governance
    - Cloud management
  - Changes over time
  - Cloud governance processes and policies
  - Govern
    - _Methodology_
      - Takes you from your first steps to full cloud governance
    - _Benchmark_
      - Governance benchmark tool
      - Assess
        - Current state
        - Future state
      - Establish a vision for applying the framework
    - _Initial governance foundation_
      - MVP
      - Captures the first steps of your governance plan
    - _Improve the initial governance foundation_
      - Add governance controls
      - Address tangible risks
  - Manage
    - _Establish a management baseline_
      - Minimum set of tools and processes that should be applied to every asset in an environment
    - _Define business commitments_
      - Document supported workloads
      - Establish operational commitments
    - _Expand the management baseline_
      - Apply best practices to iterate on your initial management baseline
    - _Advanced operations and design principles_
      - Perform architecture review

#### Create a subscription governance strategy

- Cloud center of excellence team = Cloud enablement team = Cloud custodian team
  - Implement governance practices
  - Centralized location for the entire organization
- Start Azure governance strategy -> Subscription level
- Three main aspects to consider when you create and manage subscriptions:
  - **Billing**
    - One billing report per subscription
    - Multiple departments
      - Possible solution: organize subscriptions by department or by project
      - Resource tags can also help
  - **Access control**
    - Subscription = Deployment boundary for Azure resources
    - Every subscription is associated with an Azure Active Directory tenant
    - Set granular access through defined roles
      - Azure role-based access control
  - **Subscription limits**
    - Resource limitations
      - Should be considered during your design phase
      - If you'll need to exceed -> Add more subscriptions
