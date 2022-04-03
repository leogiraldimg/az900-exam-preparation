# AZ900 - Exam Preparation

Knowledge trail: https://docs.microsoft.com/en-us/learn/paths/az-900-describe-cloud-concepts/.

## Introduction to Azure fundamentals

### Introduction

- Cloud computing platform
- Build solutions to meet your business goals
- In this module, you'll take an entry-level, end-to-end look at Azure and its capabilities

### What is Azure fundamentals?

- Série de seis roteiros de aprendizagem
- Ajudam você a se familiarizar com o Azure e seus diversos serviços e recursos

#### Why should I take Azure fundamentals?

##### Preparation for Exam AZ-900

Exame inclui seis áreas de domínio de conhecimento:

| AZ-900 Domain Area                                              | Weight |
| --------------------------------------------------------------- | ------ |
| Describe cloud concepts                                         | 20-25% |
| Describe core Azure services                                    | 15-20% |
| Describe core solutions and management tools on Azure           | 10-15% |
| Describe general security and network security features         | 10-15% |
| Describe identity, governance, privacy, and compliance features | 20-25% |
| Describe Azure cost management and Service Level Agreements     | 10-15% |

### What is cloud computing?

- Delivery of computing services over the internet
- Services = servers, storage, databases, networking, software, analytics, and intelligence
- Compute power = how much processing your computer can deliver
- Storage = amount of data that can be stored on your computer

### Why is cloud computing typically cheaper to use?

- Cloud computing is the delivery of computing services over the Internet using a pay-as-you-go pricing model
- You only pay for the cloud services you use, which helps:
  - Reduce operating costs
  - Run infrastructure more efficiently
  - Scale operations according to business needs
- The cloud provider is responsible for maintaining the underlying infrastructure for you

### Why should I move to the cloud?

- Two current trends:
  - Teams deliver new features to users in record time
  - Users expect an increasingly sophisticated and immersive experience across their devices and software.
- Weekly or daily releases

### What is Azure?

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

### How does Azure work?

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

### What is the Azure Portal?

- Web-based, unified console that provides an alternative to command-line tools
- Manage your Azure subscription by using a graphical user interface
  - Build, manage, and monitor everything from simple web apps to complex cloud deployments
  - Create custom dashboards for an organized view of resources
  - Configure accessibility options for an optimal experience
- Designed for resiliency and continuous availability
  - Maintains a presence in every Azure datacenter
  - Resilient to individual datacenter failures and avoids network slowdowns by being close to users
  - Requires no downtime for maintenance activitie

### What is Azure Marketplace?

- Customers can find, try, purchase, and provision applications and services from hundreds of leading service providers
- ## All solutions and services are certified to run on Azure

### Tour of Azure Services

#### Azure Services

![Azure Services big-picture](https://docs.microsoft.com/en-us/learn/azure-fundamentals/intro-to-azure-fundamentals/media/azure-services-6c41a736.png)

##### Compute

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

##### Networking

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

##### Storage

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

##### Mobile

- Create mobile back-end services for IOS, Android and Windows apps quickly and easily
- Adding corporate sign-in and the connecting to on-premises resources such as SAP, Oracle, SQL Server and SharePoint
- Offline data synchronization
- Connectivity to on-premises data
- Broadcasting push notifications
- Autoscaling to match business needs

##### Databases

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

##### Web

Includes firts-class support to build and host web apps and HTTP-based web services.

| Service name                          | Description                                                               |
| ------------------------------------- | ------------------------------------------------------------------------- |
| Azure App Service                     | Quickly create powerful cloud web-based apps                              |
| Azure Notification Hubs               | Send push notifications to any platform from any back end                 |
| Azure API Management                  | Publish APIs to developers, partners, and employees securely and at scale |
| Azure Cognitive Search                | Deploy this fully managed search as a service                             |
| Web Apps feature of Azure App Service | Create and deploy mission-critical web apps at scale                      |
| Azure SignalR Service                 | Add real-time web functionalities easil                                   |

##### IoT

| Service name  | Description                                                                                                                                                                                         |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| IoT Central   | Fully managed global IoT software as a service (SaaS) solution that makes it easy to connect, monitor, and manage IoT assets at scale                                                               |
| Azure IoT Hub | Messaging hub that provides secure communications between and monitoring of millions of IoT devices                                                                                                 |
| IoT Edge      | Fully managed service that allows data analysis models to be pushed directly onto IoT devices, which allows them to react quickly to state changes without needing to consult cloud-based AI models |

##### Big data

- Open-source cluster technologies developed to deal with large data sets
- Azure supports a broad range of technologies and services to provide big data and analytics solutions

| Service name            | Description                                                                                                                                                                                     |
| ----------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Azure Synapse Analytics | Run analytics at a massive scale by using a cloud-based enterprise data warehouse that takes advantage of massively parallel processing to run complex queries quickly across petabytes of data |
| Azure HDInsight         | Process massive amounts of data with managed clusters of Hadoop clusters in the cloud                                                                                                           |
| Azure Databricks        | Integrate this collaborative Apache Spark-based analytics service with other big data services in Azure                                                                                         |

##### AI

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

##### DevOps

- Automating software delivery
- You can create build and release pipelines that provide continuous integration, delivery, and deployment for your applications
- You can integrate repositories and application tests, perform application monitoring, and work with build artifacts
- You can also work with and backlog items for tracking, automate infrastructure deployment, and integrate a range of third-party tools and services such as Jenkins and Chef

| Service name       | Description                                                                                                                                                                                                                            |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Azure DevOps       | Use development collaboration tools such as high-performance pipelines, free private Git repositories, configurable Kanban boards, and extensive automated and cloud-based load testing. Formerly known as Visual Studio Team Services |
| Azure DevTest Labs | Quickly create on-demand Windows and Linux environments to test or demo applications directly from deployment pipelines                                                                                                                |

### Get started with Azure accounts

- To create and use Azure services, you need an Azure subscription
- You need to create an Azure account, and a subscription will be created for you
- For example, your company might use a single Azure account for your business and separate subscriptions for development, marketing, and sales departments
- After you've created an Azure subscription, you can start creating Azure resources within each subscription

![Azure accounts hierarchy](https://docs.microsoft.com/en-us/learn/azure-fundamentals/intro-to-azure-fundamentals/media/scope-levels-12669ee1.png)

### Create an Azure account

---
