# Module: Azure fundamentals

https://docs.microsoft.com/en-us/learn/browse/

# PART 1: Cloud Concepts - Principles of cloud computing
# Introduction

- 4 minutes

When you turn on a light, you simply want the light to work. You know you need electricity for that to happen, but in that moment, the details of how the electricity gets to the light bulb aren’t important. You might not think about electricity being created in a power plant, traveling through a large network of high-voltage transmission lines to your town, going through a substation, and eventually making its way into your home.

![Connecting a plug to represent electricity being delivered](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/1-heading.png)

The process of turning on a light is hidden behind the simple act of flipping a switch. At this point, electricity becomes a utility, which has many benefits. First, you only pay for what you need. When you buy a light bulb, you don’t pay your electricity provider up front for how long you could possibly use it. Instead, you pay for the amount of electricity that you actually use. Second, you don’t worry about how or when power plants upgrade to the latest technology. Finally, you don’t have to manage scaling the electricity. For example, as people move to your town, you can rest assured that your light will stay on.

As a technology professional, it would be nice to have these same benefits when developing and deploying applications. Storing data, streaming video, or even hosting a website all require managing hardware and software. This management is an unnecessary obstacle when delivering your application to your users. Luckily there is a solution to this problem: **cloud computing**.

## Learning objectives

In this module, you will:

- Explore common cloud computing services
- Explore the benefits of cloud computing
- Decide which cloud deployment model is best for you

------

## Next unit: What is cloud computing?

[Continue](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/2-what-is-cloud-computing)







# What is cloud computing?

- 8 minutes

Cloud computing is renting resources, like storage space or CPU cycles, on another company's computers. You only pay for what you use. The company providing these services is referred to as a cloud provider. Some example providers are Microsoft, Amazon, and Google.

The cloud provider is responsible for the physical hardware required to execute your work, and for keeping it up-to-date. The computing services offered tend to vary by cloud provider. However, typically they include:

- **Compute power** - such as Linux servers or web applications
- **Storage** - such as files and databases
- **Networking** - such as secure connections between the cloud provider and your company
- **Analytics** - such as visualizing telemetry and performance data

## Cloud computing services

The goal of cloud computing is to make running a business easier and more efficient, whether it's a small start-up or a large enterprise. Every business is unique and has different needs. To meet those needs, cloud computing providers offer a wide range of services.

You need to have a basic understanding of some of the services it provides. Let's briefly discuss the two most common services that all cloud providers offer – *compute power* and *storage*.

### Compute power

When you send an email, book a reservation on the Internet, pay a bill online, or even take this Microsoft Learn module you're interacting with cloud-based servers that are processing each request and returning a response. As a consumer, we're all dependent on the computing services provided by the various cloud providers that make up the Internet.

When you build solutions using cloud computing, you can choose how you want work to be done based on your resources and needs. For example, if you want to have more control and responsibility over maintenance, you could create a *virtual machine* (VM). A VM is an emulation of a computer - just like your desktop or laptop you're using now. Each VM includes an operating system and hardware that appears to the user like a physical computer running Windows or Linux. You can then install whatever software you need to do the tasks you want to run in the cloud.

![Compute power gauge](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/2-compute-power.png)

The difference is that you don't have to buy any of the hardware or install the OS. The cloud provider runs your virtual machine on a physical server in one of their datacenters - often sharing that server with other VMs (isolated and secure). With the cloud, you can have a VM ready to go in minutes at less cost than a physical computer.

VMs aren't the only computing choice - there are two other popular options: *containers* and *serverless computing*.

#### What are containers?

**Containers** provide a consistent, isolated execution environment for applications. They're similar to VMs except they don't require a guest operating system. Instead, the application and all its dependencies is packaged into a "container" and then a standard runtime environment is used to execute the app. This allows the container to start up in just a few seconds because there's no OS to boot and initialize. You only need the app to launch.

The open-source project, Docker, is one of the leading platforms for managing containers. Docker containers provide an efficient, lightweight approach to application deployment because they allow different components of the application to be deployed independently into different containers. Multiple containers can be run on a single machine, and containers can be moved between machines. The portability of the container makes it easy for applications to be deployed in multiple environments, either on-premises or in the cloud, often with no changes to the application.

#### What is serverless computing?

**Serverless computing** lets you run application code without creating, configuring, or maintaining a server. The core idea is that your application is broken into separate *functions* that run when triggered by some action. This is ideal for automated tasks - for example, you can build a serverless process that automatically sends an email confirmation after a customer makes an online purchase.

The serverless model differs from VMs and containers in that you only pay for the processing time used by each function as it executes. VMs and containers are charged while they're running - even if the applications on them are idle. This architecture doesn't work for every app - but when the app logic can be separated to independent units, you can test them separately, update them separately, and launch them in microseconds, making this approach the fastest option for deployment.

Here's a diagram comparing the three compute approaches we've covered.

![Diagram showing a comparison of virtual machines, containers, and serverless computing](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/2-vm-vs-container-vs-serverless.png)

### Storage

Most devices and applications read and/or write data. Here are some examples:

- Buying a movie ticket online
- Looking up the price of an online item
- Taking a picture
- Sending an email
- Leaving a voicemail

In all of these cases, data is either *read* (looking up a price) or *written* (taking a picture). The type of data and how it's stored can be different in each of these cases.

![Storage gauge](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/2-storage.png)

Cloud providers typically offer services that can handle all of these types of data. For example, if you wanted to store text or a movie clip, you could use a file on disk. If you had a set of relationships such as an address book, you could take a more structured approach like using a database.

The advantage to using cloud-based data storage is you can scale to meet your needs. If you find that you need more space to store your movie clips, you can pay a little more and add to your available space. In some cases, the storage can even expand and contract automatically - so you pay for exactly what you need at any given point in time.

## Summary

Every business has different needs and requirements. Cloud computing is **flexible** and **cost-efficient**, which can be beneficial to every business, whether it's a small start-up or a large enterprise.

------

## Next unit: Benefits of cloud computing

[Continue](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/3-benefits-of-cloud-computing)







# Benefits of cloud computing

- 8 minutes

Cloud computing isn't an all-or-nothing service approach. Companies can choose to use the cloud to store their data and execute logic as much, or as little as necessary to fulfill their business requirements. Existing businesses might choose a gradual movement to save money on infrastructure and administration costs (referred to as "lift and shift"), while a new company might start in the cloud.

Let's learn some of the top benefits of cloud computing.

## It’s cost-effective

Cloud computing provides a **pay-as-you-go** or **consumption-based** pricing model. Rather than paying upfront for a pre-defined amount of computing resources or hardware, you can rent hardware and pay for the resources that you actually use.

This consumption-based model brings with it many benefits, including:

- No upfront costs
- No need to purchase and manage costly infrastructure that you may not use to its fullest
- The ability to pay for additional resources only when they are needed
- The ability to stop paying for resources that are no longer needed

![Paper bill and a cloud representing cost effectiveness](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/3-cost-effective.png)

This also allows for better cost prediction. Prices for individual resources and services are provided so you can predict how much you will spend in a given billing period based on your expected usage. You can also perform analysis based on future growth using historical usage data tracked by your cloud provider.

## It's scalable

You can increase or decrease the resources and services used based on the demand or workload at any given time. Cloud computing supports both *vertical* and *horizontal* scaling depending on your needs.

**Vertical scaling**, also known as "scaling up", is the process of adding resources to increase the power of an existing server. Some examples of vertical scaling are: adding more CPUs, or adding more memory.

**Horizontal scaling**, also known as "scaling out", is the process of adding more servers that function together as one unit. For example, you have more than one server processing incoming requests.

![Growth chart representing scalability](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/3-scalable.png)

Scaling can be done manually or automatically based on specific triggers such as CPU utilization or the number of requests and resources can be allocated or de-allocated in minutes.

## It's elastic

As your workload changes due to a spike or drop in demand, a cloud computing system can compensate by automatically adding or removing resources.

For example, imagine your website is featured in a news article, leading to a spike in traffic overnight. Since the cloud is elastic, it automatically allocates more computing resources to handle the increased traffic. When the traffic begins to normalize, the cloud automatically de-allocates the additional resources to minimize cost.

![Point graph representing elasticity](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/3-elastic.png)

Another example is if you are running an application used by employees, you can have the cloud automatically add resources for the peak operating hours during which most people access the application, and remove the resources at the usual end of the day.

## It's current

When you use the cloud, you’re able to focus on what matters: building and deploying applications. Cloud eliminates the burdens of maintaining software patches, hardware setup, upgrades, and other IT management tasks. All of this is automatically done for you to ensure you're using the latest and greatest tools to run your business.

![Calendar representing staying current](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/3-current.png)

Additionally, the computer hardware is maintained and upgraded by the cloud provider. For example, if a disk fails, the disk will be replaced by the cloud provider. If new hardware update becomes available, you don’t have to go through the process of replacing your hardware. The cloud provider will ensure that the hardware updates are made available to you automatically.

## It's reliable

When you're running a business, you want to be confident your data is always going to be there. Cloud computing providers offer data backup, disaster recovery, and data replication services to make sure your data is always safe. In addition, redundancy is often built into cloud services architecture so if one component fails, a backup component takes its place. This is referred to as *fault tolerance* and it ensures that your customers aren't impacted when a disaster occurs.

![Certificate representing reliability](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/3-reliable.png)

## It's global

Cloud providers have fully redundant datacenters located in various regions all over the globe. This gives you a local presence close to your customers to give them the best response time possible no matter where in the world they are.

You can replicate your services into multiple regions for redundancy and locality, or select a specific region to ensure you meet data-residency and compliance laws for your customers.

![Globe representing multiple datacenters](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/3-global.png)

## It's secure

Think about how you secure your datacenter. You have physical security – who can access the building, who can operate the server racks, and so on. You also have digital security – who can connect to your systems and data over the network.

Cloud providers offer a broad set of policies, technologies, controls, and expert technical skills that can provide better security than most organizations can otherwise achieve. The result is strengthened security, which helps to protect data, apps, and infrastructure from potential threats.

![Lock representing security](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/3-secure.png)

When it comes to physical security – threats to cloud infrastructure, cloud providers invest heavily in walls, cameras, gates, security personnel, and so on, to protect physical assets. They also have strict procedures in place to ensure employees have access only to those resources that they’ve been authorized to manage.

Then there’s digital security. One thing that makes the cloud unique is that you rent compute and storage resources from a shared pool. Plus, data can travel in many different ways – within a datacenter, between datacenters, and over the internet.

For example, you want only authorized users to be able to log into virtual machines or storage systems running in the cloud. The responsibility for securing these resources is shared between you and the cloud provider. Cloud providers offer tools that help you mitigate security threats but you must use these tools to protect the resources you use.

## Summary

Cloud computing makes running a business easier. It’s cost-effective, scalable, elastic, current, reliable, and secure. This means you’re able to spend more time on what matters and less time managing the underlying details.

------

## Next unit: Compliance terms and requirements

[Continue](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/3a-compliance)







# Compliance terms and requirements

- 8 minutes

When selecting a cloud provider to host your solutions, you should understand how that provider can help you comply with regulations and standards. Some questions to ask about a potential provider include:

- How compliant is the cloud provider when it comes to handling sensitive data?
- How compliant are the services offered by the cloud provider?
- How can I deploy my own cloud-based solutions to scenarios that have accreditation or compliance requirements?
- What terms are part of the privacy statement for the provider?

 Tip

Microsoft provides the most comprehensive set of compliance offerings (including certifications and attestations) of any cloud service provider.

### Compliance Offerings

The following list provides details about *some* of the compliance offerings available.

- **Criminal Justice Information Services (CJIS)**. Any US state or local agency that wants to access the FBI’s CJIS database is required to adhere to the CJIS Security Policy. Azure is the only major cloud provider that contractually commits to conformance with the CJIS Security Policy, which commits Microsoft to adhering to the same requirements that law enforcement and public safety entities must meet.
- **Cloud Security Alliance (CSA) STAR Certification**. Azure, Intune, and Microsoft Power BI have obtained STAR Certification, which involves a rigorous independent third-party assessment of a cloud provider’s security posture. This STAR certification is based on achieving ISO/IEC 27001 certification and meeting criteria specified in the Cloud Controls Matrix (CCM). It demonstrates that a cloud service provider conforms to the applicable requirements of ISO/IEC 27001, has addressed issues critical to cloud security as outlined in the CCM, and has been assessed against the STAR Capability Maturity Model for the management of activities in CCM control areas.
- **General Data Protection Regulation (GDPR)**. As of May 25, 2018, a European privacy law — GDPR — is in effect. GDPR imposes new rules on companies, government agencies, non-profits, and other organizations that offer goods and services to people in the European Union (EU), or that collect and analyze data tied to EU residents. The GDPR applies no matter where you are located.
- **EU Model Clauses**. Microsoft offers customers EU Standard Contractual Clauses that provide contractual guarantees around transfers of personal data outside of the EU. Microsoft is the first company to receive joint approval from the EU’s Article 29 Working Party that the contractual privacy protections Azure delivers to its enterprise cloud customers meet current EU standards for international transfers of data. This ensures that Azure customers can use Microsoft services to move data freely through Microsoft's cloud from Europe to the rest of the world.
- **Health Insurance Portability and Accountability Act (HIPAA)**. The HIPAA is a US federal law that regulates patient Protected Health Information (PHI). Azure offers customers a HIPAA Business Associate Agreement (BAA), stipulating adherence to certain security and privacy provisions in HIPAA and the **Health Information Technology for Economic and Clinical Health Act (HITECH)** Act. To assist customers in their individual compliance efforts, Microsoft offers a BAA to Azure customers as a contract addendum.
- **International Organization for Standardization (ISO) and the International Electrotechnical Commission (IEC) 27018**. Microsoft is the first cloud provider to have adopted the ISO/IEC 27018 code of practice, covering the processing of personal information by cloud service providers.
- **Multi-Tier Cloud Security (MTCS) Singapore**. After rigorous assessments conducted by the MTCS Certification Body, Microsoft cloud services received MTCS 584:2013 Certification across all three service classifications—Infrastructure as a Service (IaaS), Platform as a Service (PaaS), and Software as a Service (SaaS). Microsoft was the first global cloud solution provider (CSP) to receive this certification across all three classifications.
- **Service Organization Controls (SOC) 1, 2, and 3**. Microsoft-covered cloud services are audited at least annually against the SOC report framework by independent third-party auditors. The Microsoft cloud services audit covers controls for data security, availability, processing integrity, and confidentiality as applicable to in-scope trust principles for each service.
- **National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF)**. NIST CSF is a voluntary Framework that consists of standards, guidelines, and best practices to manage cybersecurity-related risks. Microsoft cloud services have undergone independent, third-party Federal Risk and Authorization Management Program (FedRAMP) Moderate and High Baseline audits, and are certified according to the FedRAMP standards. Additionally, through a validated assessment performed by the Health Information Trust Alliance (HITRUST), a leading security and privacy standards development and accreditation organization, Office 365 is certified to the objectives specified in the NIST CSF.
- **UK Government G-Cloud**. The UK Government G-Cloud is a cloud computing certification for services used by government entities in the United Kingdom. Azure has received official accreditation from the UK Government Pan Government Accreditor.

------

## Next unit: Economies of scale

[Continue](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/3b-economies-of-scale)







# Economies of scale

- 1 minute

![Icon showing buildings with scale up arrow](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/3b-economiesofscale.png)

*Economies of scale* is the ability to do things more efficiently or at a lower-cost per unit when operating at a larger scale. This cost advantage is an important benefit in cloud computing.

Cloud providers such as Microsoft, Google, and Amazon are large businesses leveraging the benefits of economies of scale, and then pass the savings onto their customers.



These savings are apparent to end users in a number of ways, one of which is the ability to acquire hardware at a lower cost. Cloud providers can also make deals with local governments and utilities to get tax savings, lowering the price of power, cooling, and high-speed network connectivity between sites. Cloud providers are then able to pass on these benefits to end users in the form of lower prices than what you could achieve on your own.

------

## Next unit: Capital expenditure (CapEx) versus operational expenditure (OpEx)

[Continue](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/3c-capex-vs-opex)







# Capital expenditure (CapEx) versus operational expenditure (OpEx)

- 7 minutes

In the past, companies needed to acquire physical premises and infrastructure to start their business. There was a substantial up-front cost in hardware and infrastructure to start or grow a business. Cloud computing provides services to customers without significant upfront costs or equipment setup time.

These two approaches to investment are referred to as:

- **Capital Expenditure (CapEx)**: CapEx is the spending of money on physical infrastructure up front, and then deducting that expense from your tax bill over time. CapEx is an upfront cost, which has a value that reduces over time.
- **Operational Expenditure (OpEx)**: OpEx is spending money on services or products now and being billed for them now. You can deduct this expense from your tax bill in the same year. There's no upfront cost. You pay for a service or product as you use it.

## CapEx computing costs

A typical on-premises data center includes costs such as:

### Server costs

This area includes all hardware components and the cost of supporting them. When purchasing servers, make sure to design fault tolerance and redundancy, such as server clustering, redundant power supplies, and uninterruptible power supplies. When a server needs to be replaced or added to a datacenter, you need to pay for the computer. This can affect your immediate cash flow because you must pay for the server up front.

### Storage costs

This area includes all storage hardware components and the cost of supporting it. Based on the application and level of fault tolerance, centralized storage can be expensive. For larger organizations, you can create tiers of storage where more expensive fault‐tolerant storage is used for critical applications and lower expense storage is used for lower priority data.

### Network costs

Networking costs include all on-premises hardware components, including cabling, switches, access points, and routers. This also includes wide area network (WAN) and Internet connections.

### Backup and archive costs

This is the cost to back up, copy, or archive data. Options might include setting up a backup to or from the cloud. There’s an upfront cost for the hardware and additional costs for backup maintenance and consumables like tapes.

### Organization continuity and disaster recovery costs

Along with server fault tolerance and redundancy, you need to plan for how to recover from a disaster and continue operating. Your plan should consist of creating a data recovery site. It could also include backup generators. Most of these are upfront costs, especially if you build a data recovery site, but there's an additional ongoing cost for the infrastructure and its maintenance.

### Datacenter infrastructure costs

These are costs for electricity, floor space, cooling, and building maintenance.

### Technical personnel

Based on the technology used, you’ll need technical expertise and workforce to install, deploy, and manage the systems in the datacenter and at the data recovery site.

## OpEx cloud computing costs

With cloud computing, many of the costs associated with an on-premises datacenter are shifted to the service provider. Instead of thinking about physical hardware and datacenter costs, cloud computing has a different set of costs. For accounting purposes, all these costs are operational expenses:

### Leasing a cloud-based server

If you lease a server or use a cloud-based server, the cost is typically based on the pay-per-use model.

### Leasing software and customized features

Using a pay-per-use model requires actively managing your subscriptions to ensure users do not misuse the services, and that provisioned accounts are being utilized and not wasted. As soon as the provider provisions resources, billing starts. It is your responsibility to de-provision the resources when they aren't in use so that you can minimize costs.

### Scaling charges based on usage/demand instead of fixed hardware or capacity.

Cloud computing can bill in various ways, such as the number of users or CPU usage time. However, billing categories can also include allocated RAM, I/O operations per second (IOPS), and storage space. Plan for backup traffic and data recovery traffic to determine the bandwidth needed.

### Billing at the user or organization level.

The subscription (pay-per-use) model is a computing billing method that is designed for both organizations and users. The organization or user is billed for the services used, typically on a recurring basis. You can scale, customize, and provision computing resources, including software, storage, and development platforms. For example, when using a dedicated cloud service, you could pay based on server hardware and usage.

## Benefits of CapEx

With capital expenditures, you plan your expenses at the start of a project or budget period. Your costs are fixed, meaning you know exactly how much is being spent. This is appealing when you need to predict the expenses before a project starts due to a limited budget.

## Benefits of OpEx

Demand and growth can be unpredictable and can outpace expectation, which is a challenge for the CapEx model as shown in the following graph.

![A graph showing how expected demand can be different from real demand and how CapEx infrastructure can be exceeded by demand.](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/3c-capexvsopex.png)

With the OpEx model, companies wanting to try a new product or service don't need to invest in equipment. Instead, they pay as much or as little for the infrastructure as required.

OpEx is particularly appealing if the demand fluctuates or is unknown. Cloud services are often said to be *agile*. Cloud agility is the ability to rapidly change an IT infrastructure to adapt to the evolving needs of the business. For example, if your service peaks one month, you can scale to demand and pay a larger bill for the month. If the following month the demand drops, you can reduce the used resources and be charged less. This agility lets you manage your costs dynamically, optimizing spending as requirements change.

------

## Next unit: Cloud deployment models

[Continue](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/4-cloud-deployment-models)







# Cloud deployment models

- 10 minutes

There are three different cloud deployment models. A cloud deployment model defines where your data is stored and how your customers interact with it – how do they get to it, and where do the applications run? It also depends on how much of your own infrastructure you want or need to manage.

## Explore the three deployment methods of cloud computing

#### Public versus Private versus Hybrid

<iframe id="RE2yEv7-ax-0-id-oneplayer" src="https://www.microsoft.com/en-us/videoplayer/embed/RE2yEv7?pid=RE2yEv7-ax-0-id-oneplayer&amp;jsapi=true&amp;postJsllMsg=true&amp;autoplay=false&amp;mute=false&amp;loop=false&amp;market=en-us&amp;playFullScreen=false" class="oneplayer-iframe" allowfullscreen="true" frameborder="0" name="Oneplayer iframe" title="Video: RE2yEv7" style="width: 640px; box-sizing: inherit; position: absolute; top: 0px; left: 0px; right: 0px; bottom: 0px; height: 360px;"></iframe>

### Public cloud

This is the most common deployment model. In this case, you have no local hardware to manage or keep up-to-date – everything runs on your cloud provider’s hardware. In some cases, you can save additional costs by sharing computing resources with other cloud users.

Businesses can use multiple public cloud providers of varying scale. Microsoft Azure is an example of a public cloud provider.

![Public cloud icon](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/4-public-cloud.png)

#### Advantages

- High scalability/agility – you don’t have to buy a new server in order to scale
- Pay-as-you-go pricing – you pay only for what you use, no CapEx costs
- You’re not responsible for maintenance or updates of the hardware
- Minimal technical knowledge to set up and use - you can leverage the skills and expertise of the cloud provider to ensure workloads are secure, safe, and highly available

A common use case scenario is deploying a web application or a blog site on hardware and resources that are owned by a cloud provider. Using a public cloud in this scenario allows cloud users to get their website or blog up quickly, and then focus on maintaining the site without having to worry about purchasing, managing or maintaining the hardware on which it runs.

#### Disadvantages

Not all scenarios fit the public cloud. Here are some disadvantages to think about:

- There may be specific security requirements that cannot be met by using public cloud
- There may be government policies, industry standards, or legal requirements which public clouds cannot meet
- You don't own the hardware or services and cannot manage them as you may want to
- Unique business requirements, such as having to maintain a legacy application might be hard to meet

### Private cloud

In a private cloud, you create a cloud environment in your own datacenter and provide self-service access to compute resources to users in your organization. This offers a simulation of a public cloud to your users, but you remain completely responsible for the purchase and maintenance of the hardware and software services you provide.

![Private cloud icon](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/4-private-cloud.png)

#### Advantages

This approach has several advantages:

- You have complete control over the resources and can ensure the configuration can support any scenario or legacy application
- You have complete control (and responsibility) over security
- Private clouds can meet strict security, compliance, or legal requirements in ways a public cloud might not be able to

#### Disadvantages

Some reasons teams move away from the private cloud are:

- You have upfront CapEx costs and must purchase the hardware for startup and maintenance
- Owning the equipment limits the agility - to scale you must buy, install, and setup new hardware
- Private clouds require IT skills and expertise that's hard to come by

A use case scenario for a private cloud would be when an organization has data that cannot be put in the public cloud, perhaps for legal reasons. For example, they may have medical data that cannot be exposed publicly. Another scenario may be where government policy requires specific data to be kept in-country or privately.

A private cloud can provide cloud functionality to external customers as well, or to specific internal departments such as Accounting or Human Resources.

### Hybrid cloud

A hybrid cloud combines public and private clouds, allowing you to run your applications in the most appropriate location. For example, you could host a website in the public cloud and link it to a highly secure database hosted in your private cloud (or on-premises datacenter).

![Hybrid cloud icon](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/4-hybrid-cloud.png)

This is helpful when you have some things that cannot be put in the cloud, maybe for legal reasons. For example, you may have some specific pieces of data that cannot be exposed publicly (such as medical data) which needs to be held in your private datacenter. Another example is one or more applications that run on old hardware that can’t be updated. In this case, you can keep the old system running locally, and connect it to the public cloud for authorization or storage.

#### Advantages

Some advantages of a hybrid cloud are:

- You can keep any systems running and accessible that use out-of-date hardware or an out-of-date operating system
- You have flexibility with what you run locally versus in the cloud
- You can take advantage of economies of scale from public cloud providers for services and resources where it's cheaper, and then supplement with your own equipment when it's not
- You can use your own equipment to meet security, compliance, or legacy scenarios where you need to completely control the environment

#### Disadvantages

Some concerns you'll need to watch out for are:

- It can be more expensive than selecting one deployment model since it involves some CapEx cost up front
- It can be more complicated to set up and manage

## Summary

Cloud computing is flexible and gives you the ability to choose how you want to deploy it. The cloud deployment model you choose depends on your budget, and on your security, scalability, and maintenance needs.

------

## Next unit: Types of cloud services

[Continue](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/5-types-of-cloud-services)





# Types of cloud services

- 10 minutes

When talking about cloud computing, there are three major categories. It's important to understand them because they are used in conversation, documentation, and training.

## Explore the three categories of cloud computing

#### IaaS versus SaaS versus PaaS

<iframe id="RE2yEbs-ax-3-id-oneplayer" src="https://www.microsoft.com/en-us/videoplayer/embed/RE2yEbs?pid=RE2yEbs-ax-3-id-oneplayer&amp;jsapi=true&amp;postJsllMsg=true&amp;autoplay=false&amp;mute=false&amp;loop=false&amp;market=en-us&amp;playFullScreen=false" class="oneplayer-iframe" allowfullscreen="true" frameborder="0" name="Oneplayer iframe" title="Video: RE2yEbs" style="width: 640px; box-sizing: inherit; position: absolute; top: 0px; left: 0px; right: 0px; bottom: 0px; height: 360px;"></iframe>

![IaaS icon](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/5-iaas.png)

### Infrastructure as a service (IaaS)

Infrastructure as a Service is the most flexible category of cloud services. It aims to give you complete control over the hardware that runs your application (IT infrastructure servers and virtual machines (VMs), storage, networks, and operating systems). Instead of buying hardware, with IaaS, you rent it. It's an instant computing infrastructure, provisioned and managed over the internet.

 Note

When using IaaS, ensuring that a service is up and running is a shared responsibility: the cloud provider is responsible for ensuring the cloud infrastructure is functioning correctly; the cloud customer is responsible for ensuring the service they are using is configured correctly, is up to date, and is available to their customers. This is referred to as the **shared responsibility model**.

IaaS is commonly used in the following scenarios:

- **Migrating workloads.** Typically, IaaS facilities are managed in a similar way as on-premises infrastructure and provide an easy migration path for moving existing applications to the cloud.
- **Test and development.** Teams can quickly set up and dismantle test and development environments, bringing new applications to market faster. IaaS makes scaling development and testing environments, fast and economical.
- **Website hosting.** Running websites using IaaS can be less expensive compared to traditional web hosting.
- **Storage, backup, and recovery.** Organizations avoid the capital outlay and complexity of storage management, which typically requires skilled staff to manage data and meet legal and compliance requirements. IaaS is useful for managing unpredictable demand and steadily growing storage needs. IaaS can also simplify the planning and management of backup and recovery systems.

![PaaS icon](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/5-paas.png)

### Platform as a service (PaaS)

PaaS provides an environment for building, testing, and deploying software applications. The goal of PaaS is to help you create an application quickly without managing the underlying infrastructure. For example, when deploying a web application using PaaS, you don't have to install an operating system, web server, or even system updates.

PaaS is a complete development and deployment environment in the cloud, with resources that enable organizations to deliver everything from simple cloud-based apps to sophisticated cloud-enabled enterprise applications. Resources are purchased from a cloud service provider on a pay-as-you-go basis and accessed over a secure Internet connection.

PaaS is commonly used in the following scenarios:

- **Development framework.** PaaS provides a framework that developers can build upon to develop or customize cloud-based applications. Just like Microsoft Excel macro, PaaS lets developers create applications using built-in software components. Cloud features such as scalability, high-availability, and multi-tenant capability are included, reducing the amount of coding that developers must do.
- **Analytics or business intelligence.** Tools provided as a service with PaaS allow organizations to analyze and mine their data. They can find insights and patterns, and predict outcomes to improve business decisions such as forecasting, product design, and investment returns.

![SaaS icon](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/5-saas.png)

### Software as a service (SaaS)

SaaS is software that is centrally hosted and managed for the end customer. It is usually based on an architecture where one version of the application is used for all customers, and licensed through a monthly or annual subscription. Office 365, Skype, and Dynamics CRM Online are perfect examples of SaaS software.

## Cost and Ownership

|                          | IaaS                                                         | PaaS                                                         | SaaS                                                         |
| :----------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| Upfront costs            | There are no upfront costs. Users pay only for what they consume. | There are no upfront costs. Users pay only for what they consume. | Users have no upfront costs; they pay a subscription, typically on a monthly or annual basis. |
| User ownership           | The user is responsible for the purchase, installation, configuration, and management of their own software, operating systems, middleware, and applications. | The user is responsible for the development of their own applications. However, they are not responsible for managing the server or infrastructure. This allows the user to focus on the application or workload they want to run. | Users just use the application software; they are not responsible for any maintenance or management of that software. |
| Cloud provider ownership | The cloud provider is responsible for ensuring that the underlying cloud infrastructure (such as virtual machines, storage, and networking) is available for the user. | The cloud provider is responsible for operating system management, network, and service configuration. Cloud providers are typically responsible for everything apart from the application that a user wants to run. They provide a complete managed platform on which to run the application. | The cloud provider is responsible for the provision, management, and maintenance of the application software. |

## Management responsibilities

One thing to understand is that these categories are layers on top of each other. For example, PaaS adds a layer on top of IaaS by providing a level of abstraction. The abstraction has the benefit of hiding the details that you may not care about, so that you can get to coding quicker. However, one aspect of the abstraction is that you have less control over the underlying hardware. The following illustration shows a list of resources that you manage and that your service provider manages in each cloud service category.

![An illustration showing the level of abstraction in each category of cloud service.](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/5-layer-diagram.png)

- IaaS requires the most user management of all the cloud services. The user is responsible for managing the operating systems, data, and applications.
- PaaS requires less user management. The cloud provider manages the operating systems, and the user is responsible for the applications and data they run and store.
- SaaS requires the least amount of management. The cloud provider is responsible for managing everything, and the end user just uses the software.

## Summary

IaaS, PaaS, and SaaS each contain different levels of managed services. You may easily use a combination of these types of infrastructure. You could use Office 365 on your company’s computers (SaaS), and in Azure, you could host your VMs (IaaS) and use Azure SQL Database (PaaS) to store your data. With the cloud’s flexibility, you can use any combination that provides you with the maximum result.

------

## Next unit: Knowledge Check

[Continue](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/6-knowledge-check)







# Knowledge Check

- 3 minutes

## Check your knowledge

\1. 

Which term from the list below would be viewed as benefits of using cloud services?



Unpredictable costs



Elasticity



Local reach only

\2. 

Suppose you have two types of applications: legacy applications that require specialized mainframe hardware and newer applications that can run on commodity hardware. Which cloud deployment model would be best for you?



Public cloud



Private cloud



Hybrid cloud

\3. 

You're developing an application and want to focus on building, testing, and deploying. You don't want to worry about managing the underlying hardware or software. Which cloud service type is best for you?



Infrastructure as a Service (IaaS)



Platform as a Service (PaaS)



Software as a Service (SaaS)







# Summary

- 3 minutes

In this module, you've learned about cloud computing, what it is and what its key characteristics are. Here are some of the things you covered.

- Different types of cloud models that are available and the considerations of using those different models.
- Some of the key terms and concepts such as high availability, agility, elasticity, fault tolerance, and CapEx vs. OpEx.
- The different cloud services available, the benefits of using the different types, and the management responsibilities under each service type.
- Cloud models such as public, private and hybrid, and what the key characteristics of each model are.
- The different types of cloud service available: IaaS, PaaS, and SaaS; what the key characteristics of each service are and when you would choose one over the other.

![A connected plug to represent electricity being delivered](https://docs.microsoft.com/en-us/learn/modules/principles-cloud-computing/media/7-heading.png)

### Microsoft Azure

Azure is Microsoft's cloud computing platform. Azure provides over 100 services that enable you to do everything from running your existing applications on virtual machines to exploring new software paradigms such as intelligent bots and mixed reality.

Here are just a few kinds of services you'll find on Azure:

- **Compute** services such as VMs and containers that can run your applications
- **Database** services that provide both relational and NoSQL choices
- **Identity** services that help you authenticate and protect your users
- **Networking** services that connect your datacenter to the cloud, provide high availability or host your DNS domain
- **Storage** solutions that can accommodate massive amounts of both structured and unstructured data
- **AI and machine-learning** services can analyze data, text, images, comprehend speech, and make predictions using data — changing the world of agriculture, healthcare, and much more.
- And many more!

## Learn more

Stay on the [Azure Fundamentals Learning Path](https://docs.microsoft.com/learn/paths/azure-fundamentals/) to learn more about how Microsoft Azure can help you build more secure, reliable, performant applications in the cloud.

In addition, here are some places to go to learn more about what we've covered today:

- [Cloud Computing Terms](https://azure.microsoft.com/overview/cloud-computing-dictionary/)
- [What is Azure?](https://azure.microsoft.com/overview/)
- [Azure compliance offerings](https://www.microsoft.com/trustcenter/compliance/complianceofferings)

------

## Module complete:











# PART 2: Core Cloud Services - Introduction to Azure

# Introduction

- 1 minute

You've heard buzzwords about the cloud — *scale*, *elasticity*, *microservices*. Perhaps you've seen other companies be successful with the cloud and wondered how it can help you meet your business challenges or even grow your career. Did you know that more than 90% of Fortune 500 companies run on the Microsoft Cloud?

![The Azure logo representing the start of your learning journey](https://docs.microsoft.com/en-us/learn/modules/welcome-to-azure/media/1-heading.png)

The cloud helps power your everyday life, and it's often present in ways you don't even realize. In this new connected world, we believe technology creates opportunity. To keep up with today's ever-changing digital world, understanding cloud technology can help align your career to this exciting revolution.

In less than the time it takes to eat lunch, you'll create your first virtual machine on Azure and configure it to run a basic web site, a foundational building block of everything from digital transformation to the next big startup.

In this module, you will:

- Learn what Microsoft Azure is and how it relates to cloud computing
- Use Azure Cloud Shell to launch a Windows or Linux virtual machine
- Configure your virtual machine to run a basic web server
- Scale up your server to give you more compute power

------

## Next unit: What is Azure?

[Continue](https://docs.microsoft.com/en-us/learn/modules/welcome-to-azure/2-what-is-azure)







# What is Azure?

- 5 minutes

Azure is Microsoft's cloud computing platform. Azure is a continually expanding set of cloud services that help your organization meet your current and future business challenges. Azure gives you the freedom to build, manage, and deploy applications on a massive global network using your favorite tools and frameworks.

#### How does Azure work?

<iframe id="RWlzQ6-ax-4-id-oneplayer" src="https://www.microsoft.com/en-us/videoplayer/embed/RWlzQ6?pid=RWlzQ6-ax-4-id-oneplayer&amp;jsapi=true&amp;postJsllMsg=true&amp;autoplay=false&amp;mute=false&amp;loop=false&amp;market=en-us&amp;playFullScreen=false" class="oneplayer-iframe" allowfullscreen="true" frameborder="0" name="Oneplayer iframe" title="Video: RWlzQ6" style="width: 640px; box-sizing: inherit; position: absolute; top: 0px; left: 0px; right: 0px; bottom: 0px; height: 360px;"></iframe>

Before we go further, let's briefly define cloud computing.

![A web server and two databases](https://docs.microsoft.com/en-us/learn/modules/welcome-to-azure/media/2-cloud-computing.png)

**What is cloud computing?**

Cloud computing is the delivery of computing services over the Internet using a **pay-as-you-go** pricing model. Put another way, it's a way to rent compute power and storage from someone else's data center.

Instead of maintaining CPUs and storage in your data center, you rent them for the time that you need them. The cloud provider takes care of maintaining the underlying infrastructure for you.

You can treat cloud resources like you would your resources in your own data center. When you're done using them, you just give them back. You're billed only for what you use.

While this is all great, the real value of the cloud is that it enables you to quickly solve your toughest business challenges and bring cutting edge solutions to your users.

![A suitcase representing a move to the cloud](https://docs.microsoft.com/en-us/learn/modules/welcome-to-azure/media/2-why-cloud.png)

**Why should I move to the cloud?**

The cloud helps you move faster and innovate in ways that were once nearly impossible.

In our ever-changing digital world, two trends emerge:

- Teams are delivering new features to their users at record speeds.
- End users expect an increasingly rich and immersive experience with their devices and with software.

Software releases were once scheduled in terms of months or even years. Today, teams are releasing features in smaller batches. Releases are now often scheduled in terms of days or weeks. Some teams even deliver software updates continuously — sometimes with multiple releases within the same day.

Think of all the ways you interact with devices that you couldn't do just a few years ago. Many devices can recognize your face and respond to voice commands. Augmented reality changes the way you interact with the physical world. Household appliances are even beginning to act intelligently. These are just a few examples, many of which are powered by the cloud.

To power your services and deliver innovative and novel user experiences more quickly, the cloud provides on-demand access to:

- A nearly limitless pool of raw compute, storage, and networking components.
- Speech recognition and other cognitive services that help make your application stand out from the crowd.
- Analytics services that enable you to make sense of telemetry data coming back from your software and devices.

Let's see how Azure fits in with cloud computing.

![A cup containing an artist's tools](https://docs.microsoft.com/en-us/learn/modules/welcome-to-azure/media/2-azure.png)

**What can I do on Azure?**

Azure provides over 100 services that enable you to do everything from running your existing applications on virtual machines to exploring new software paradigms such as intelligent bots and mixed reality.

Many teams start exploring the cloud by moving their existing applications to virtual machines that run in Azure. While migrating your existing apps to virtual machines is a good start, the cloud is more than just "a different place to run your virtual machines".

For example, Azure provides AI and machine-learning services that can naturally communicate with your users through vision, hearing, and speech. It also provides storage solutions that dynamically grow to accommodate massive amounts of data. Azure services enable solutions that are simply not feasible without the power of the cloud.

------

## Next unit: Tour of Azure services

[Continue](https://docs.microsoft.com/en-us/learn/modules/welcome-to-azure/3-tour-of-azure-services)







# Tour of Azure services

- 10 minutes

Azure can help you tackle tough business challenges. You bring your requirements, creativity, and favorite software development tools. Azure brings a massive global infrastructure that's always available for you to build your applications on.

Let's take a quick tour of the high-level services Azure offers.

#### Azure: the big picture

<iframe id="RE2yuas-ax-5-id-oneplayer" src="https://www.microsoft.com/en-us/videoplayer/embed/RE2yuas?pid=RE2yuas-ax-5-id-oneplayer&amp;jsapi=true&amp;postJsllMsg=true&amp;autoplay=false&amp;mute=false&amp;loop=false&amp;market=en-us&amp;playFullScreen=false" class="oneplayer-iframe" allowfullscreen="true" frameborder="0" name="Oneplayer iframe" title="Video: RE2yuas" style="width: 640px; box-sizing: inherit; position: absolute; top: 0px; left: 0px; right: 0px; bottom: 0px; height: 360px;"></iframe>

## Azure services

Here's a big-picture view of the available services and features in Azure.

[![Diagram showing the big picture view of Azure services](https://docs.microsoft.com/en-us/learn/modules/welcome-to-azure/media/3-azure-services.png)](https://docs.microsoft.com/en-us/learn/modules/welcome-to-azure/media/3-azure-services.png#lightbox)

Let's take a closer look at the most commonly-used categories:

- Compute
- Networking
- Storage
- Mobile
- Databases

- Web
- Internet of Things
- Big Data
- Artificial Intelligence
- DevOps

### Compute

Compute services are often one of the primary reasons why companies move to the Azure platform. Azure provides a range of options for hosting applications and services. Here are some examples of compute services in Azure:

| Service name                     | Service function                                             |
| :------------------------------- | :----------------------------------------------------------- |
| Azure Virtual Machines           | Windows or Linux virtual machines (VMs) hosted in Azure      |
| Azure Virtual Machine Scale Sets | Scaling for Windows or Linux VMs hosted in Azure             |
| Azure Kubernetes Service         | Enables management of a cluster of VMs that run containerized services |
| Azure Service Fabric             | Distributed systems platform. Runs in Azure or on-premises   |
| Azure Batch                      | Managed service for parallel and high-performance computing applications |
| Azure Container Instances        | Run containerized apps on Azure without provisioning servers or VMs |
| Azure Functions                  | An event-driven, serverless compute service                  |

### Networking

Linking compute resources and providing access to applications is the key function of Azure networking. Networking functionality in Azure includes a range of options to connect the outside world to services and features in the global Microsoft Azure datacenters.

Azure networking facilities have the following features:

| Service name                   | Service function                                             |
| :----------------------------- | :----------------------------------------------------------- |
| Azure Virtual Network          | Connects VMs to incoming Virtual Private Network (VPN) connections |
| Azure Load Balancer            | Balances inbound and outbound connections to applications or service endpoints |
| Azure Application Gateway      | Optimizes app server farm delivery while increasing application security |
| Azure VPN Gateway              | Accesses Azure Virtual Networks through high-performance VPN gateways |
| Azure DNS                      | Provides ultra-fast DNS responses and ultra-high domain availability |
| Azure Content Delivery Network | Delivers high-bandwidth content to customers globally        |
| Azure DDoS Protection          | Protects Azure-hosted applications from distributed denial of service (DDOS) attacks |
| Azure Traffic Manager          | Distributes network traffic across Azure regions worldwide   |
| Azure ExpressRoute             | Connects to Azure over high-bandwidth dedicated secure connections |
| Azure Network Watcher          | Monitors and diagnoses network issues using scenario-based analysis |
| Azure Firewall                 | Implements high-security, high-availability firewall with unlimited scalability |
| Azure Virtual WAN              | Creates a unified wide area network (WAN), connecting local and remote sites |

### Storage

Azure provides four main types of storage services. These services are:

| Service name        | Service function                                             |
| :------------------ | :----------------------------------------------------------- |
| Azure Blob storage  | Storage service for very large objects, such as video files or bitmaps |
| Azure File storage  | File shares that you can access and manage like a file server |
| Azure Queue storage | A data store for queuing and reliably delivering messages between applications |
| Azure Table storage | A NoSQL store that hosts unstructured data independent of any schema |

These services all share several common characteristics:

- **Durable** and highly available with redundancy and replication.
- **Secure** through automatic encryption and role-based access control.
- **Scalable** with virtually unlimited storage.
- **Managed**, handling maintenance and any critical problems for you.
- **Accessible** from anywhere in the world over HTTP or HTTPS.

### Mobile

Azure enables developers to create mobile backend services for iOS, Android, and Windows apps quickly and easily. Features that used to take time and increase project risks, such as adding corporate sign-in and then connecting to on-premises resources such as SAP, Oracle, SQL Server, and SharePoint, are now simple to include.

Other features of this service include:

- Offline data synchronization.
- Connectivity to on-premises data.
- Broadcasting push notifications.
- Autoscaling to match business needs.

### Databases

Azure provides multiple database services to store a wide variety of data types and volumes. And with global connectivity, this data is available to users instantly.

| Service name                     | Service function                                             |
| :------------------------------- | :----------------------------------------------------------- |
| Azure Cosmos DB                  | Globally distributed database that supports NoSQL options    |
| Azure SQL Database               | Fully managed relational database with auto-scale, integral intelligence, and robust security |
| Azure Database for MySQL         | Fully managed and scalable MySQL relational database with high availability and security |
| Azure Database for PostgreSQL    | Fully managed and scalable PostgreSQL relational database with high availability and security |
| SQL Server on VMs                | Host enterprise SQL Server apps in the cloud                 |
| Azure SQL Data Warehouse         | Fully managed data warehouse with integral security at every level of scale at no extra cost |
| Azure Database Migration Service | Migrates your databases to the cloud with no application code changes |
| Azure Cache for Redis            | Caches frequently used and static data to reduce data and application latency |
| Azure Database for MariaDB       | Fully managed and scalable MariaDB relational database with high availability and security |

### Web

Having a great web experience is critical in today's business world. Azure includes first-class support to build and host web apps and HTTP-based web services. The Azure services focused on web hosting include:

| Service Name                          | Description                                                  |
| :------------------------------------ | :----------------------------------------------------------- |
| Azure App Service                     | Quickly create powerful cloud web-based apps                 |
| Azure Notification Hubs               | Send push notifications to any platform from any back end.   |
| Azure API Management                  | Publish APIs to developers, partners, and employees securely and at scale. |
| Azure Search                          | Fully managed search as a service.                           |
| Web Apps feature of Azure App Service | Create and deploy mission-critical web apps at scale.        |
| Azure SignalR Service                 | Add real-time web functionalities easily.                    |

### Internet of Things

People are able to access more information than ever before. It began with personal digital assistants (PDAs), then morphed into smartphones. Now there are smart watches, smart thermostats, even smart refrigerators. Personal computers used to be the norm. Now the internet allows any item that's online-capable to access valuable information. This ability for devices to garner and then relay information for data analysis is referred to as the Internet of Things (IoT).

There are a number of services that can assist and drive end-to-end solutions for IoT on Azure.

| Service Name  | Description                                                  |
| :------------ | :----------------------------------------------------------- |
| IoT Central   | Fully-managed global IoT software as a service (SaaS) solution that makes it easy to connect, monitor, and manage your IoT assets at scale |
| Azure IoT Hub | Messaging hub that provides secure communications and monitoring between millions of IoT devices |
| IoT Edge      | Push your data analysis onto your IoT devices instead of in the cloud allowing them to react more quickly to state changes. |

### Big Data

Data comes in all formats and sizes. When we talk about Big Data, we're referring to *large* volumes of data. Data from weather systems, communications systems, genomic research, imaging platforms, and many other scenarios generate hundreds of gigabytes of data. This amount of data makes it hard to analyze and make decisions around. It's often so large that traditional forms of processing and analysis are no longer appropriate.

Open source cluster technologies have been developed to deal with these large data sets. Microsoft Azure supports a broad range of technologies and services to provide big data and analytic solutions.

| Service Name               | Description                                                  |
| :------------------------- | :----------------------------------------------------------- |
| Azure SQL Data Warehouse   | Run analytics at a massive scale using a cloud-based Enterprise Data Warehouse (EDW) that leverages massive parallel processing (MPP) to run complex queries quickly across petabytes of data |
| Azure HDInsight            | Process massive amounts of data with managed clusters of Hadoop clusters in the cloud |
| Azure Databricks (preview) | Collaborative Apache Spark–based analytics service that can be integrated with other Big Data services in Azure. |

### Artificial Intelligence

Artificial Intelligence, in the context of cloud computing, is based around a broad range of services, the core of which is Machine Learning. Machine Learning is a data science technique that allows computers to use existing data to forecast future behaviors, outcomes, and trends. Using machine learning, computers learn without being explicitly programmed.

Forecasts or predictions from machine learning can make apps and devices smarter. For example, when you shop online, machine learning helps recommend other products you might like based on what you've purchased. Or when your credit card is swiped, machine learning compares the transaction to a database of transactions and helps detect fraud. And when your robot vacuum cleaner vacuums a room, machine learning helps it decide whether the job is done.

Some of the most common Artificial Intelligence and Machine Learning service types in Azure are:

| Service Name                   | Description                                                  |
| :----------------------------- | :----------------------------------------------------------- |
| Azure Machine Learning Service | Cloud-based environment you can use to develop, train, test, deploy, manage, and track machine learning models. It can auto-generate a model and auto-tune it for you. It will let you start training on your local machine, and then scale out to the cloud |
| Azure Machine Learning Studio  | Collaborative, drag-and-drop visual workspace where you can build, test, and deploy machine learning solutions using pre-built machine learning algorithms and data-handling modules |

A closely related set of products are the *cognitive services*. These are pre-built APIs you can leverage in your applications to solve complex problems.

| Service Name                | Description                                                  |
| :-------------------------- | :----------------------------------------------------------- |
| Vision                      | Image-processing algorithms to smartly identify, caption, index, and moderate your pictures and videos. |
| Speech                      | Convert spoken audio into text, use voice for verification, or add speaker recognition to your app. |
| Knowledge mapping           | Map complex information and data in order to solve tasks such as intelligent recommendations and semantic search. |
| Bing Search                 | Add Bing Search APIs to your apps and harness the ability to comb billions of webpages, images, videos, and news with a single API call. |
| Natural Language processing | Allow your apps to process natural language with pre-built scripts, evaluate sentiment and learn how to recognize what users want. |

### DevOps

DevOps (Development and Operations) brings together people, processes, and technology, automating software delivery to provide continuous value to your users. Azure DevOps Services allows you to create *build* and *release* pipelines that provide continuous integration, delivery, and deployment for your applications. You can integrate repositories and application tests, perform application monitoring, and work with build artifacts. You can also work with and backlog items for tracking, automate infrastructure deployment and integrate a range of third-party tools and services such as Jenkins and Chef. All of these functions and many more are closely integrated with Azure to allow for consistent, repeatable deployments for your applications to provide streamlined build and release processes.

Some of the main DevOps services available with Azure are Azure DevOps Services and Azure DevTest Labs.

| Service Name       | Description                                                  |
| :----------------- | :----------------------------------------------------------- |
| Azure DevOps       | Azure DevOps Services (formerly known as Visual Studio Team Services, or VSTS), provides development collaboration tools including high-performance pipelines, free private Git repositories, configurable Kanban boards, and extensive automated and cloud-based load testing |
| Azure DevTest Labs | Quickly create on-demand Windows and Linux environments you can use to test or demo your applications directly from your deployment pipelines |

------

## Next unit: Create a virtual machine

[Continue](https://docs.microsoft.com/en-us/learn/modules/welcome-to-azure/4-create-a-vm)





# Create a virtual machine

- 7 minutes

Sandbox activated! Time remaining:

 

58 min

Choose which platform you want to run in the cloud

WindowsLinux

As a technology professional, you likely have expertise in a specific area. Perhaps you're a storage admin or virtualization expert, or maybe you focus on the latest security practices. If you're a student, you may still be exploring what interests you most.

No matter your role, most people get started with the cloud by creating a virtual machine. Here you'll deploy a virtual machine running Ubuntu 18.04.

There are many ways to create a virtual machine on Azure. Here, you'll create a Windows or Linux virtual machine using an interactive terminal called Cloud Shell. If you work from the terminal on a daily basis, you know this is often the fastest way to get the job done.

 Tip

Prefer Windows or want to try something new? Select **Windows** from the top of this page to run a Windows Server virtual machine.

Let's review some basic terms and get your first virtual machine up and running.

## What is a virtual machine?

A virtual machine, or VM, is a software emulation of a physical computer. Because VMs exist as software, dozens, hundreds, or even thousands of Azure VMs can be generated in minutes, then deleted when you don't need them. With low-cost, per-minute billing, you pay only for the compute resources you use, for as long as you are using them. Plus, there are many ways to configure the VMs to fit your needs.

A snapshot of a running VM is called an *image*. Azure provides images for Windows and several flavors of Linux. You can also create your own preconfigured images to make deployments go faster. Here you'll bring up an Ubuntu 18.04 VM, provided by Canonical.

## What defines a virtual machine on Azure?

A virtual machine is defined by a number of factors, including its size and location. Before you bring up your VM, let's briefly cover what's involved.

**Size**

A VM's *size* defines its processor speed, amount of memory, initial amount of storage, and expected network bandwidth. Some sizes even include specialized hardware such as GPUs for heavy graphics rendering and video editing.

**Region**

Azure is made up of data centers distributed throughout the world. A *region* is a set of Azure data centers in a named geographic location. Every Azure resource, including virtual machines, is assigned a region. East US and North Europe are examples of regions.

**Network**

A *virtual network* is a logically isolated network on Azure. Each virtual machine on Azure is associated with a virtual network. Azure provides cloud-level firewalls for your virtual networks called *network security groups*.

**Resource groups**

Virtual machines and other cloud resources are grouped into logical containers called *resource groups*. Groups are typically used to organize sets of resources that are deployed together as part of an application or service. You refer to a resource group by its name.

## What is Azure Cloud Shell?

Azure Cloud Shell is a browser-based command-line experience for managing and developing Azure resources. Think of Cloud Shell as an interactive console that you run in the cloud.

Cloud Shell provides two experiences to choose from: Bash and PowerShell. Both include access to the Azure CLI, the command-line interface for Azure.

You can use any Azure management interface, including the Azure portal, Azure CLI, and Azure PowerShell, to manage any kind of VM. For learning purposes, here you'll use the Azure CLI to create and manage either a Windows or Linux VM.

 Note

Make sure you activate the sandbox before you continue.

## Creating resources in Azure

Normally, the first thing we'd do is to create a *resource group* to hold all the things that we need to create. This allows us to administer all the VMs, disks, network interfaces, and other elements that make up our solution as a unit. We can use the Azure CLI to create a resource group with the `az group create` command. It takes a `--name` to give it a unique name in our subscription, and a `--location` to tell Azure what area of the world we want the resources to be located by default.

Since we are in the free Azure sandbox environment, you don't need to do this step, instead, you will use the pre-created resource group **209bd267-09de-4896-86de-1bab8f5b8b98**.

## Choosing a location

The free sandbox allows you to create resources in a subset of Azure's global regions. Select a region from the following list when creating any resources:

- westus2
- southcentralus
- centralus
- eastus
- westeurope

- southeastasia
- japaneast
- brazilsouth
- australiasoutheast
- centralindia

## Create a Linux VM

Let's get your Linux VM up and running.

1. From Cloud Shell on the right side of this page, run the `az vm create` command to create your VM. The following command creates the VM in the "East US" location, you can change that to any of the locations listed above - we recommend you select one close to you.

   Azure CLICopy

   ```azurecli
   az vm create \
     --name myVM \
     --resource-group 209bd267-09de-4896-86de-1bab8f5b8b98 \
     --image UbuntuLTS \
     --location eastus \
     --size Standard_DS2_v2 \
     --admin-username azureuser \
     --generate-ssh-keys
   ```

    Tip

   You can use the **Copy** button to copy commands to the clipboard. To paste, right click on a new line in the Cloud Shell window and select **Paste** or use the Shift+Insert keyboard shortcut (⌘+V on macOS).

   Your VM will take about two minutes to come up. Compare that to the time it takes to purchase, rack, and configure a system in your data center. Quite a difference!

While you're waiting, let's review the command you just ran.

- The VM is named **myVM**. This name identifies the VM in Azure. It also becomes the VM's internal hostname, or computer name.
- The resource group, or the VM's logical container, is named **209bd267-09de-4896-86de-1bab8f5b8b98**.
- **UbuntuLTS** specifies the Ubuntu 18.04 LTS VM image.
- **Standard_DS2_v2** refers to the size of the VM. This size has two virtual CPUs and 7 GB of memory.
- The `--admin-username` option specifies **azureuser** as the username for the VM. The username can be whatever you want.
- The `--generate-ssh-keys` option creates an SSH key pair to enable you to log in to the VM.

 Note

Although you have everything you need to connect directly to your VM, don't do so quite yet. In the next unit, you'll see one way to connect to the VM to make changes to its configuration.

By default, Azure assigns a public IP address to your VM. You can configure a VM to be accessible from the Internet or only from the internal network.

You can also check out this short video about some of the options you have to create and manage VMs.

#### Options to create and manage VMs

<iframe id="RE2yJKx-ax-1-id-oneplayer" src="https://www.microsoft.com/en-us/videoplayer/embed/RE2yJKx?pid=RE2yJKx-ax-1-id-oneplayer&amp;jsapi=true&amp;postJsllMsg=true&amp;autoplay=false&amp;mute=false&amp;loop=false&amp;market=en-us&amp;playFullScreen=false" class="oneplayer-iframe" allowfullscreen="true" frameborder="0" name="Oneplayer iframe" style="width: 640px; box-sizing: inherit; position: absolute; top: 0px; left: 0px; right: 0px; bottom: 0px; height: 360px;"></iframe>

When the VM is ready, you see information about it. Here's an example.

JSONCopy

```json
{
  "fqdns": "",
  "id": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/myResourceGroup/providers/Microsoft.Compute/virtualMachines/myVM",
  "location": "eastus",
  "macAddress": "00-0D-3A-1D-EB-02",
  "powerState": "VM running",
  "privateIpAddress": "10.0.0.4",
  "publicIpAddress": "137.135.110.210",
  "resourceGroup": "myResourceGroup",
  "zones": ""
}
```

 Note

On Microsoft Learn, you'll often see sample output, like the output shown above. We show you these examples so you can compare them to the output you see. However, it's just an example, so don't enter it into the Cloud Shell session.

## Verify your VM is running

The `az vm create` command succeeded, but let's verify that your VM is up and running.

1. Run the following `az vm get-instance-view` command to verify that the VM was successfully created and is running.

   Azure CLICopy

   ```azurecli
   az vm get-instance-view \
     --name myVM \
     --resource-group 209bd267-09de-4896-86de-1bab8f5b8b98 \
     --output table
   ```

   The output you see resembles this.

   Azure CLICopy

   ```azurecli
   Name    ResourceGroup                         Location    ProvisioningState    PowerState
   ------  ------------------------------------  ----------  -------------------  ------------
   myVM    209bd267-09de-4896-86de-1bab8f5b8b98  eastus      Succeeded            VM running
   ```

   You see the VM's name, its resource group, and its location. You also see that the VM was provisioned, or created, successfully and that it's running.



Check your work







# Add a web server

- 5 minutes

Sandbox activated! Time remaining:

 

39 min

Choose which platform you want to run in the cloud

WindowsLinux

Here you'll install a web server in your VM and serve up a basic web page that displays the VM's hostname.

To configure a VM, you have several choices. You can connect directly and interactively configure your system. For example, on Windows systems you can create a Remote Desktop session to connect to the UI of your remote Windows computer as if you were seated at it. On Linux systems, you can create an SSH connection to securely work with your remote Linux system from the terminal.

Manual configuration is a good start, but as you add systems, you can automate your deployments. Automation involves running repeatable processes such as programs and scripts that take care of the heavy lifting for you.

Here, you'll configure IIS remotely from your Cloud Shell session using a feature of Windows-based Azure virtual machines called the Custom Script Extension.

## What is IIS?

Internet Information Services, or IIS, is a web server that runs on Windows. You can use IIS to serve standard web content (HTML, CSS, and JavaScript) or run ASP.NET and other kinds of web applications. IIS comes with Windows Server, but you need to activate it to start serving web pages.

## What's the Custom Script Extension?

The Custom Script Extension is an easy way to download and run scripts on your Azure VMs. It's just one of the many ways you can configure the system once your VM is up and running.

You can store your scripts in Azure storage or in a public location such as GitHub. You can run scripts manually or as part of a more automated deployment. Here, you'll run an Azure CLI command to download a PowerShell script from GitHub and execute it on your VM. The script configures IIS.

## Configure IIS

Here you'll use the Custom Script Extension to configure IIS remotely on your VM from Cloud Shell. You'll also configure the firewall to allow inbound network access on port 80 (HTTP).

1. From Cloud Shell, run this `az vm extension set` command to download and execute a PowerShell script that installs IIS and configures a basic home page.

   Azure CLICopy

   ```azurecli
   az vm extension set \
     --resource-group 14685a35-e230-4d3c-b364-8734fa03b79b \
     --vm-name myVM \
     --name CustomScriptExtension \
     --publisher Microsoft.Compute \
     --settings "{'fileUris':['https://raw.githubusercontent.com/MicrosoftDocs/mslearn-welcome-to-azure/master/configure-iis.ps1']}" \
     --protected-settings "{'commandToExecute': 'powershell -ExecutionPolicy Unrestricted -File configure-iis.ps1'}"
   ```

   The process to configure IIS, set the contents of the homepage, and start the service takes a couple minutes to complete.

   In the meantime, you can [examine the PowerShell script ](https://raw.githubusercontent.com/MicrosoftDocs/mslearn-welcome-to-azure/master/configure-iis.ps1) from a separate browser tab if you'd like. The script installs IIS and configures the home page to display a welcome message along with the VM's computer name, "myVM".

2. Run this `az vm open-port` command to open port 80 (HTTP) through the firewall.

   Azure CLICopy

   ```azurecli
   az vm open-port \
     --name myVM \
     --resource-group 14685a35-e230-4d3c-b364-8734fa03b79b \
     --port 80
   ```

## Verify the configuration

Now that IIS is set up, let's verify that it's running.

1. Run this `az vm show` command to list your VM's public IP address.

   Azure CLICopy

   ```azurecli
   az vm show \
     --name myVM \
     --resource-group 14685a35-e230-4d3c-b364-8734fa03b79b \
     --show-details \
     --query [publicIps] \
     --output tsv
   ```

   You see your VM's public IP address, for example, 104.211.9.245.

2. In a new browser tab, navigate to your VM's IP address (`http://` followed by the IP address). You'll see your welcome message and your VM's name.

   ![img](https://docs.microsoft.com/en-us/learn/modules/welcome-to-azure/media/5-iis-browser.png)

   If you don't see your welcome message:

   - Verify that you're using your VM's IP address and not the IP address shown in any of the examples.
   - Verify that you ran the `az vm open-port` command shown earlier to open port 80 (HTTP) through the firewall.
   - Wait a few moments and refresh the page. Although IIS is installed, the service may not yet have fully started.

------

## Next unit: Scale up

[Continue](https://docs.microsoft.com/en-us/learn/modules/welcome-to-azure/6-scale-up)







# Scale up

- 4 minutes

Sandbox activated! Time remaining:

 

39 min

Choose which platform you want to run in the cloud

WindowsLinux

Your web server is up and running, but you realize you need more computing power to make the experience great for your users. How can you make your VM run faster?

In your data center, you might move your web server to more powerful hardware to solve performance problems. The problem is you need to buy, rack, and power your new system. With Azure, the answer is much simpler.

Before you scale up your VM to a more powerful size, let's first define what scale means.

## What is scale?

*Scale* refers to adding network bandwidth, memory, storage, or compute power to achieve better performance.

You may have heard the terms *scaling up* and *scaling out*.

Scaling up, or vertical scaling, means to increase the memory, storage, or compute power on an existing virtual machine. For example, you can add additional memory to a web or database server to make it run faster.

Scaling out, or horizontal scaling, means to add extra virtual machines to power your application. For example, you might create many virtual machines configured in exactly the same way and use a load balancer to distribute work across them.

 Tip

The cloud is elastic. You can *scale down* or *scale in* your deployment if you needed to scale up or scale out only temporarily. Scaling down or scaling in can help you save money.

**Azure Advisor** and **Azure Cost Management** are two services that help you optimize cloud spend. You can use these services to identify where you're using more than you need, and then scale back to the capacity you're actually using.

## Scale up your VM

Recall that you specified the size **Standard_DS2_v2** when you created your VM. Your VM currently has two virtual CPUs and 7 GB of memory.

Let's bump up to the next size, **Standard_DS3_v2**. Your VM will then have four virtual CPUs and 14 GB of memory.

1. From Cloud Shell, run `az vm resize` to increase your VM's size to **Standard_DS3_v2**.

   Azure CLICopy

   ```azurecli
   az vm resize \
     --resource-group 14685a35-e230-4d3c-b364-8734fa03b79b \
     --name myVM \
     --size Standard_DS3_v2
   ```

   The update process takes about a minute. Your VM restarts during the process.

2. Run `az vm show` to verify that your VM is running the new size.

   Azure CLICopy

   ```azurecli
   az vm show \
     --resource-group 14685a35-e230-4d3c-b364-8734fa03b79b \
     --name myVM \
     --query "hardwareProfile" \
     --output tsv
   ```

   You see your new VM size, **Standard_DS3_v2**.

   outputCopy

   ```output
   Standard_DS3_v2
   ```



Check your work





# Knowledge Check

- 3 minutes

## Check your knowledge

\1. 

What is Azure?



Microsoft's cloud computing platform, which provides compute power, storage, and services over the Internet using a pay-as-you-go pricing model.



A single data center located in Redmond, Washington.



A hosting environment specifically for virtual machines

\2. 

Which of the following is an example of an Azure compute service?



Azure Virtual Machine



Azure Load Balancer



Azure Table Storage



Azure Cache for Redis

\3. 

When should you *scale out* your deployment?



When your application or service requires a more powerful CPU or more memory to run faster.



When you need additional virtual machines to speed up your application.



When you're using excess capacity that you don't need.







# Summary

- 1 minute

Nice work! With your first virtual machine under your belt, you now have a sense of how Azure works and how easy it is to bring up a system, configure some software, and tear everything down when it's no longer needed.

Azure provides services that can help transform the way your organization delivers new features to your users in ways you simply can't do without the power of the cloud.

![A graduation cap representing the successful start of your learning journey](https://docs.microsoft.com/en-us/learn/modules/welcome-to-azure/media/7-heading.png)

## Clean up

The sandbox automatically cleans up your resources when you're finished with this module.

When you're working in your own subscription, it's a good idea at the end of a project to identify whether you still need the resources you created. Resources left running can cost you money. You can delete resources individually or delete the resource group to delete the entire set of resources.

## Continue your Azure journey

Microsoft Learn provides learning paths based on your role and interests.

You've taken your first step on the [Azure fundamentals](https://docs.microsoft.com/en-us/learn/paths/azure-fundamentals/) learning path. Keep going to learn how Azure services such as compute, storage, networking, and security can help you unlock the power of the cloud and create that next great breakthrough idea.

------

## Module incomplete:

[Go back to finish](https://docs.microsoft.com/learn/modules/welcome-to-azure/6-scale-up)









 # PART 3: Core Cloud Services - Azure architecture and service guarantees

# Introduction

- 3 minutes

You're a small business owner with a great set of web-based services that your clients love. The one difficulty you face is some clients are experiencing a network lag accessing your services from distant locations. This problem used to be expensive to solve - requiring new data centers and costly networks to connect them. The emergence of cloud computing has made the solution easy.

Microsoft Azure provides a reliable, redundant, energy-efficient infrastructure that spans more than 100 highly secure facilities worldwide, linked by one of the largest networks on earth. Azure allows you to gain **global reach** with **local presence**, keep your data secure and compliant with local laws, and have a reduced carbon footprint with Microsoft's environment-friendly datacenters.

## Learning objectives

In this module, you will:

- Explore the physical structure of Azure infrastructure
- Understand the service level agreements provided by Azure
- Learn how to provide service level agreements for your apps

------

## Next unit: Datacenters and Regions in Azure

[Continue](https://docs.microsoft.com/en-us/learn/modules/explore-azure-infrastructure/2-azure-datacenter-locations)







# Datacenters and Regions in Azure

- 5 minutes

Microsoft Azure is made up of datacenters located around the globe. When you leverage a service or create a resource such as a SQL database or virtual machine, you are using physical equipment in one or more of these locations.

The specific datacenters aren't exposed to end users directly; instead, Azure organizes them into *regions*.

## What is a region?

A **region** is a geographical area on the planet containing at least one, but potentially multiple datacenters that are nearby and networked together with a low-latency network. Azure intelligently assigns and controls the resources within each region to ensure workloads are appropriately balanced.

When you deploy a resource in Azure, you will often need to choose the region where you want your resource deployed.

 Important

Some services or virtual machine features are only available in certain regions, such as specific virtual machine sizes or storage types. There are also some global Azure services that do not require you to select a particular region, such as Microsoft Azure Active Directory, Microsoft Azure Traffic Manager, and Azure DNS.

A few examples of regions are *West US*, *Canada Central*, *West Europe*, *Australia East*, and *Japan West*. Here's a view of all the available regions as of December 2018:

[![Map of available regions as of December 2018](https://docs.microsoft.com/en-us/learn/modules/explore-azure-infrastructure/media/2-regions-small.png)](https://docs.microsoft.com/en-us/learn/modules/explore-azure-infrastructure/media/2-regions-large.png#lightbox)

### Why is this important?

Azure has more global regions than any other cloud provider. This gives you the flexibility to bring applications closer to your users no matter where they are. It also provides better scalability, redundancy, and preserves data residency for your services.

### Special Azure regions

Azure has specialized regions that you might want to use when building out your applications for compliance or legal purposes. These include:

- *US DoD Central*, *US Gov Virginia*, *US Gov Iowa* and more: These are physical and logical network-isolated instances of Azure for US government agencies and partners. These datacenters are operated by screened US persons and include additional compliance certifications.
- *China East*, *China North* and more: These regions are available through a unique partnership between Microsoft and 21Vianet, whereby Microsoft does not directly maintain the datacenters.

Regions are what you use to identify the location for your resources, but there are two other terms you should also be aware of: *geographies* and *availability zones*.

------

## Next unit: Geographies

[Continue](https://docs.microsoft.com/en-us/learn/modules/explore-azure-infrastructure/3-geographies)







# Geographies

- 3 minutes

Azure divides the world into *geographies* that are defined by geopolitical boundaries or country borders. An Azure geography is a discrete market typically containing two or more regions that preserve data residency and compliance boundaries. This division has several benefits.

- Geographies allow customers with specific data residency and compliance needs to keep their data and applications close.
- Geographies ensure that data residency, sovereignty, compliance, and resiliency requirements are honored within geographical boundaries.
- Geographies are fault-tolerant to withstand complete region failure through their connection to dedicated high-capacity networking infrastructure.

 Tip

Data residency refers to the physical or geographic location of an organization's data or information. It defines the legal or regulatory requirements imposed on data based on the country or region in which it resides and is an important consideration when planning out your application data storage.

Geographies are broken up into the following areas:

- Americas
- Europe
- Asia Pacific
- Middle East and Africa

Each region belongs to a single geography and has specific service availability, compliance, and data residency/sovereignty rules applied to it. Check the documentation for more information (a link is available in the summary unit).

------

## Next unit: Availability Zones

[Continue](https://docs.microsoft.com/en-us/learn/modules/explore-azure-infrastructure/4-availability-zones)





  


  Availability Zones

- 5 minutes

You want to ensure your services and data are redundant so you can protect your information in case of failure. When you are hosting your infrastructure, this requires creating duplicate hardware environments. Azure can help make your app highly available through *Availability Zones*.

## What is an Availability Zone?

Availability Zones are physically separate datacenters within an Azure region.

Each Availability Zone is made up of one or more datacenters equipped with independent power, cooling, and networking. It is set up to be an *isolation boundary*. If one zone goes down, the other continues working. Availability Zones are connected through high-speed, private fiber-optic networks.

![Image showing three datacenters connected within a single region to represent an Availability Zone](https://docs.microsoft.com/en-us/learn/modules/explore-azure-infrastructure/media/4-availability-zones.png)

### Supported regions

Not every region has support for Availability Zones. The following regions have a minimum of three separate zones to ensure resiliency.

- Central US
- East US 2
- West US 2
- West Europe
- France Central
- North Europe
- Southeast Asia

 Tip

The list of supported regions is expanding - check the documentation for the latest information.

### Using Availability Zones in your apps

You can use Availability Zones to run mission-critical applications and build high-availability into your application architecture by co-locating your compute, storage, networking, and data resources within a zone and replicating in other zones. Keep in mind that there could be a cost to duplicating your services and transferring data between zones.

Availability Zones are primarily for VMs, managed disks, load balancers, and SQL databases. Azure services that support Availability Zones fall into two categories:

- **Zonal services** – you pin the resource to a specific zone (for example, virtual machines, managed disks, IP addresses)
- **Zone-redundant services** – platform replicates automatically across zones (for example, zone-redundant storage, SQL Database).

Check the documentation to determine which elements of your architecture you can associate with an Availability Zone.

------

## Next unit: Region Pairs

[Continue](https://docs.microsoft.com/en-us/learn/modules/explore-azure-infrastructure/5-region-pairs)







# Region Pairs

- 5 minutes

Availability zones are created using one or more datacenters, and there are a minimum of three zones within a single region. However, it's possible that a large enough disaster could cause an outage big enough to affect even two datacenters. That's why Azure also creates *region pairs*.

## What is a region pair?

Each Azure region is always paired with another region within the same geography (such as US, Europe, or Asia) at least **300 miles away**. This approach allows for the replication of resources (such as virtual machine storage) across a geography that helps reduce the likelihood of interruptions due to events such as natural disasters, civil unrest, power outages, or physical network outages affecting both regions at once.

Examples of region pairs in Azure are West US paired with East US, and SouthEast Asia paired with East Asia.

![Image showing the relationship between geography, region pair, region, and datacenter](https://docs.microsoft.com/en-us/learn/modules/explore-azure-infrastructure/media/5-region-pairs.png)

Since the pair of regions is directly connected and far enough apart to be isolated from regional disasters, you can use them to provide reliable services and data redundancy. Some services offer automatic geo-redundant storage using region pairs.

Additional advantages of region pairs include:

- If there's an extensive Azure outage, one region out of every pair is prioritized to help reduce the time it takes to restore them for applications.
- Planned Azure updates are rolled out to paired regions one region at a time to minimize downtime and risk of application outage.
- Data continues to reside within the same geography as its pair (except for Brazil South) for tax and law enforcement jurisdiction purposes.

Having a broadly distributed set of datacenters allows Azure to provide a high guarantee of availability. Let's explore what that means.

------

## Next unit: Service Level Agreements for Azure

[Continue](https://docs.microsoft.com/en-us/learn/modules/explore-azure-infrastructure/6-service-level-agreements)









# Service Level Agreements for Azure

- 6 minutes

Microsoft maintains its commitment to providing customers with high-quality products and services by adhering to comprehensive operational policies, standards, and practices. Formal documents called *Service-Level Agreements* (SLAs) capture the specific terms that define the performance standards that apply to Azure.

- SLAs describe Microsoft's commitment to providing Azure customers with specific performance standards.
- There are SLAs for individual Azure products and services.
- SLAs also specify what happens if a service or product fails to perform to a governing SLA's specification.

 Important

Azure does not provide SLAs for most services under the *Free* or *Shared* tiers. Also, free products such as Azure Advisor do not typically have an SLA.

## SLAs for Azure products and services

There are three key characteristics of SLAs for Azure products and services:

1. Performance Targets
2. Uptime and Connectivity Guarantees
3. Service credits

### Performance Targets

An SLA defines performance targets for an Azure product or service. The performance targets that an SLA defines are specific to each Azure product and service. For example, performance targets for some Azure services are expressed as uptime guarantees or connectivity rates.

### Uptime and Connectivity Guarantees

A typical SLA specifies performance-target commitments that range from 99.9 percent ("three nines") to 99.999 percent ("five nines"), for each corresponding Azure product or service. These targets can apply to such performance criteria as uptime or response times for services.

The following table lists the potential cumulative downtime for various SLA levels over different durations:

| SLA %  | Downtime per week | Downtime per month | Downtime per year |
| :----- | :---------------- | :----------------- | :---------------- |
| 99     | 1.68 hours        | 7.2 hours          | 3.65 days         |
| 99.9   | 10.1 minutes      | 43.2 minutes       | 8.76 hours        |
| 99.95  | 5 minutes         | 21.6 minutes       | 4.38 hours        |
| 99.99  | 1.01 minutes      | 4.32 minutes       | 52.56 minutes     |
| 99.999 | 6 seconds         | 25.9 seconds       | 5.26 minutes      |

For example, the SLA for the Azure Cosmos DB (Database) service SLA offers 99.99 percent uptime, which includes low-latency commitments of less than 10 milliseconds on DB read operations and less than 15 milliseconds on DB write operations.

### Service Credits

SLAs also describe how Microsoft will respond if an Azure product or service fails to perform to its governing SLA's specification.

For example, customers may have a discount applied to their Azure bill, as compensation for an under-performing Azure product or service. The table below explains this example in more detail.

The first column in the table below shows monthly uptime percentage SLA targets for a single instance Azure Virtual Machine. The second column shows the corresponding service credit amount you receive if the *actual* uptime is less than the specified SLA target for that month.

| MONTHLY UPTIME PERCENTAGE | SERVICE CREDIT PERCENTAGE |
| :------------------------ | :------------------------ |
| < 99.9                    | 10                        |
| < 99                      | 25                        |
| < 95                      | 100                       |

------

## Next unit: Composing SLAs across services

[Continue](https://docs.microsoft.com/en-us/learn/modules/explore-azure-infrastructure/7-composite-sla)







# Composing SLAs across services

- 5 minutes

When combining SLAs across different service offerings, the resultant SLA is a called a *Composite SLA*. The resulting composite SLA can provide higher or lower uptime values, depending on your application architecture.

## Calculating downtime

Consider an App Service web app that writes to Azure SQL Database. These Azure services currently have the following SLAs:

![Image representing Web app and its SLA uptime value of 99.95 percent and a SQL database and its SLA value of 99.99 percent.](https://docs.microsoft.com/en-us/learn/modules/explore-azure-infrastructure/media/7-sla-compositesla1.png)

In this example, if either service fails the whole application will fail. In general, the individual probability values for each service are independent. However, the composite SLA value for this application is:

```
99.95 percent × 99.99 percent = 99.94 percent
```

This means the **combined probability of failure** is higher than the individual SLA values. This isn't surprising, because an application that relies on multiple services has more potential failure points.

Conversely, you can improve the composite SLA by creating independent fallback paths. For example, if SQL Database is unavailable, you can put transactions into a queue for processing at a later time.

![Image representing Web app and its SLA uptime value of 99.95% and SQL database and its SLA value of 99.99%.](https://docs.microsoft.com/en-us/learn/modules/explore-azure-infrastructure/media/7-sla-compositesla2.png)

With this design, the application is still available even if it can't connect to the database. However, it fails if both the database *and* the queue fail simultaneously.

If the expected percentage of time for a simultaneous failure is **0.0001 × 0.001**, the composite SLA for this combined path of a database *or* queue would be:

```
1.0 − (0.0001 × 0.001) = 99.99999 percent
```

Therefore, if we add the queue to our web app, the total composite SLA is:

```
99.95 percent × 99.99999 percent = ~99.95 percent
```

Notice we've improved our SLA behavior. However, there are trade-offs to using this approach: the application logic is more complicated, you are paying more to add the queue support, and there may be data-consistency issues you'll have to deal with due to retry behavior.

------

## Next unit: Improve your app reliability

[Continue](https://docs.microsoft.com/en-us/learn/modules/explore-azure-infrastructure/8-improve-app-slas)







  Improve your app reliability

- 8 minutes

You can use SLAs to evaluate how your Azure solutions meet business requirements and the needs of your clients and users. By creating your own SLAs, you can set performance targets to suit your specific Azure application. This approach is known as an *Application SLA*.

## Understand your app requirements

Building an efficient and reliable Azure solution requires knowing your workload requirements. You can then select Azure products and services, and provision resources according to those requirements. It's important to understand the Azure SLAs that define performance targets for the Azure products and services within your solution. This understanding will help you create achievable Application SLAs.

In a distributed system, failures will happen. Hardware can fail. The network can have transient failures. It's rare for an entire service or region to experience a disruption, but even this must be planned for.

## Resiliency

*Resiliency* is the ability of a system to recover from failures and continue to function. It's not about avoiding failures, but responding to failures in a way that avoids downtime or data loss. The goal of resiliency is to return the application to a fully functioning state following a failure. High availability and disaster recovery are two crucial components of resiliency.

When designing your architecture you need to design for resiliency, and you should perform a *Failure Mode Analysis*(FMA). The goal of an FMA is to identify possible points of failure and to define how the application will respond to those failures.

## Cost and complexity vs. high availability

*Availability* refers to the time that a system is functional and working. Maximizing availability requires implementing measures to prevent possible service failures. However, devising preventative measures can be difficult and expensive, and often results in complex solutions.

As your solution grows in complexity, you will have more services depending on each other. Therefore, you might overlook possible failure points in your solution if you have several interdependent services.

 Tip

For example: A workload that requires 99.99 percent uptime shouldn't depend upon a service with a 99.9 percent SLA.

Most providers prefer to maximize the availability of their Azure solutions by minimizing downtime. However, as you increase availability, you also increase the cost and complexity of your solution.

 Tip

For example: An SLA that defines an *uptime of 99.99% only allows for about 5 minutes of total downtime per month.*

The risk of potential downtime is cumulative across various SLA levels, which means that complex solutions can face greater availability challenges. Therefore, how critical high-availability is to your requirements will determine how you handle the addition of complexity and cost to your application SLAs.

## Considerations for defining application SLAs

- If your application SLA defines four 9's (99.99%) performance targets, recovering from failures by manual intervention may not be enough to fulfill your SLA. Your Azure solution must be self-diagnosing and self-healing instead.
- It is difficult to respond to failures quickly enough to meet SLA performance targets above four 9's.
- Carefully consider the time window against which your application SLA performance targets are measured. The smaller the time window, the tighter the tolerances. If you define your application SLA as hourly or daily uptime, you need to understand these tighter tolerances might not allow for achievable performance targets.

------

## Next unit: Summary

[Continue](https://docs.microsoft.com/en-us/learn/modules/explore-azure-infrastructure/9-summary)





  


  Summary

- 5 minutes

Microsoft provides more global presence than any other cloud provider with over 54 regions distributed worldwide. This infrastructure gives you the scale needed to bring your applications closer to users around the world. Azure also has dedicated regions to support government use and applications that need to be deployed in China so you can ensure data security and residency and meet compliance and resilience requirements for your customers no matter what type of business requirements you have.

## Learn more

Visit the following links to learn more about some of the topics we explored in this module.

- [Azure regions](https://azure.microsoft.com/global-infrastructure/regions/)
- [Azure geographies](https://azure.microsoft.com/global-infrastructure/geographies/)
- [Azure Service Level Agreements](https://azure.microsoft.com/support/legal/sla/summary/)
- [Designing resilient applications for Azure](https://docs.microsoft.com/azure/architecture/resiliency/)

## Check your knowledge

\1. 

True or False. You can select the specific datacenter you want to deploy your app into.



True



False

\2. 

True or False. Every region has an availability zone.



True



False

\3. 

Application availability refers to what?



The service level agreement of the associated resource.



Whether the application supports an availability zone.



The overall time that a system is functional and working.













# PART 4: Create an Azure account

# Introduction

- 2 minutes

To create and use Azure services, you will need an Azure *account*. The account is free, and it allows you to build and deploy cloud-based applications, utilize sophisticated artificial intelligence services, and extract essential insights from your data.

With an Azure account, you can use a variety of free and paid services to create the next-generation architecture for your product and users.

## Learning objectives

In this module, you will:

- Learn about the different types of Azure accounts and subscriptions
- Understand how billing works in Azure
- Create a free Azure account
- Learn how to get help when you need it

## Prerequisites

- Knowledge of basic cloud computing terms and concepts

- A valid credit card to register with Azure

   Note

  An Azure Account is not required to take the free training provided by Microsoft Learn. Creating an Azure account is optional; you can complete this Learn module without creating an account.

------

## Next unit: Azure accounts and subscriptions

[Continue](https://docs.microsoft.com/en-us/learn/modules/create-an-azure-account/2-azure-accounts-and-subscriptions)







# Azure accounts and subscriptions

- 4 minutes

With a free Azure account and subscription, you can build, test, and deploy enterprise applications, create custom web and mobile experiences, and gain insights from your data through machine learning and powerful analytics.

## What is an Azure account?

An *Azure account* is tied to a specific identity and holds information like:

- Name, email, and contact preferences
- Billing information such as a credit card

An Azure account is what you use to sign in to the Azure website and administer or deploy services. Every Azure account is associated with one or more *subscriptions*.

## What is an Azure subscription?

An *Azure subscription* is a logical container used to provision resources in Microsoft Azure. It holds the details of all your resources like virtual machines, databases, etc.

### Subscription types

Azure offers free and paid subscription options to suit different needs and requirements. The most commonly used subscriptions are:

- Free
- Pay-As-You-Go
- Enterprise Agreement
- Student

#### Azure free subscription

An Azure free subscription includes a **$200 credit** to spend on any service for the first 30 days, free access to the most popular Azure products for 12 months, and access to more than 25 products that are always free. This is an excellent way for new users to get started. To set up a free subscription, you need a phone number, a credit card, and a Microsoft account.

 Note

Credit card information is used for identity verification only. You won’t be charged for any services until you upgrade.

#### Azure Pay-As-You-Go subscription

A Pay-As-You-Go (PAYG) subscription charges you monthly for the services you used in that billing period. This subscription type is appropriate for a wide range of users, from individuals to small businesses, and many large organizations as well.

#### Azure Enterprise Agreement

An Enterprise Agreement provides flexibility to buy cloud services and software licenses under one agreement, with discounts for new licenses and Software Assurance. It's targeted at enterprise-scale organizations.

#### Azure for Students subscription

An Azure for Students subscription includes **$100 in Azure credits** to be used within the first 12 months plus select free services without requiring a credit card at sign-up. You must verify your student status through your organizational email address.

## Summary

Whether you are an individual, a small business, an enterprise, or a student, you need a subscription to use Azure services. The typical sequence is to start with a free subscription so that you can evaluate Azure services. When your trial period expires, you will convert from the free subscription to Pay-As-You-Go.

------

## Next unit: Using multiple Azure subscriptions

[Continue](https://docs.microsoft.com/en-us/learn/modules/create-an-azure-account/3-multiple-subscriptions)







# Using multiple Azure subscriptions

- 5 minutes

You can create multiple subscriptions under a single Azure account. This is particularly useful for businesses because *access control* and *billing* occur at the **subscription level**, not the account level.

![Conceptual image showing a single account with multiple subscriptions](https://docs.microsoft.com/en-us/learn/modules/create-an-azure-account/media/3-accounts-and-subscriptions.png)

## Access management

You can create separate subscriptions on your Azure account to reflect different organizational structures. For example, you could limit engineering to lower-cost resources, while allowing the IT department a full range. This design allows you to manage and control access to the resources that users provision within each subscription.

 Important

Subscriptions are also bound to some hard limitations. For example, the maximum number of Express Route circuits per subscription is 10. Those limits should be considered as you create subscriptions on your account. If there is a need to go over those limits in particular scenarios, then additional subscriptions may be needed.

## Billing

One bill is generated for every Azure subscription on a monthly basis. The payment is charged automatically to the associated account credit or debit card within 10 days after the billing period ends. On your credit card statement, the line item would say **MSFT Azure**.

 Note

Subscriptions are billed independently, but the *account owner* is responsible for payment. In the case of "Pay-as-you-go" subscriptions, the account credit card will be charged for all associated subscriptions.

You can analyze your bill in the Azure portal - this will provide access to all your invoices, as well as a cost analysis breakdown of what got charged each month.

![Image showing the cost analysis section of the Azure portal for a subscription billing period](https://docs.microsoft.com/en-us/learn/modules/create-an-azure-account/media/3-understand-your-bill.png)

You can set spending limits on each subscription to ensure you aren't surprised at the end of the month. Reports can be generated by subscriptions, if you have multiple internal departments and need to do "chargeback," a possible scenario is to create subscriptions by department or project.

------

## Next unit: Authenticate access with Azure Active Directory

[Continue](https://docs.microsoft.com/en-us/learn/modules/create-an-azure-account/4-azure-tenants)








# Authenticate access with Azure Active Directory

- 5 minutes

As you've seen, your Azure account is a globally unique entity that gives you access to your Azure subscriptions and services. Authentication for your account is performed using Azure Active Directory (Azure AD). Azure AD is a modern identity provider that supports multiple authentication protocols to secure applications and services in the cloud.

 Important

Azure AD is *not* the same as Windows Active Directory. Windows Active Directory is focused on securing Windows desktops and servers. In contrast, Azure AD is all about web-based authentication standards such as OpenID and OAuth.

Users, applications, and other entities registered in Azure AD aren't all lumped into a single global service. Instead, Azure AD is partitioned into separate *tenants*. A tenant is a dedicated, isolated instance of the Azure Active Directory service, owned and managed by an organization. When you sign up for a Microsoft cloud service subscription such as Microsoft Azure, Microsoft Intune, or Office 365, a dedicated instance of Azure AD is automatically created for your organization.

When it comes to Azure AD tenants, there is no concrete definition of "organization" — tenants can be owned by individuals, teams, companies, or any other group of people. Tenants are commonly associated with companies. If you sign up for Azure with an email address that's not associated with an existing tenant, the sign-up process will walk you through creating a tenant, owned entirely by you.

 Tip

The email address you use to sign in to Azure can be associated with more than one tenant. You might see this if you have an Azure account and you use Microsoft Learn's Azure Sandbox to complete exercises. In the Azure portal, you can only view resources belonging to one tenant at a time. To switch the tenant, you're viewing resources for select the **Book and filter** icon at the top of the portal and choose a different tenant in the **Switch directory** section.

Azure AD tenants and subscriptions have a many-to-one trust relationship: A tenant can be associated with multiple Azure subscriptions, but every subscription is associated with only one tenant. This structure allows organizations to manage multiple subscriptions and set security rules across all the resources contained within them.

Here's a simple representation of how accounts, subscriptions, tenants, and resources work together.

![An illustration showing two different Azure AD tenants. One tenant has two subscriptions, and each subscription is linked to a set of Azure resources. The other tenant has one subscription that is linked to a different set of Azure resources.](https://docs.microsoft.com/en-us/learn/modules/create-an-azure-account/media/4-azure-ad-tenant.png)

Notice that each Azure AD tenant has an *account owner*. This is the original Azure account that is responsible for billing. You can add additional users to the tenant, and even invite guests from other Azure AD tenants to access resources in subscriptions.

------

## Next unit: Exercise - Create an Azure account

[Continue](https://docs.microsoft.com/en-us/learn/modules/create-an-azure-account/5-exercise-create-an-azure-account)







  

# Azure support options

- 8 minutes

One final thing to know about subscriptions is how to get support when you need it. Every Azure subscription includes free access to the following essential support services:

- Billing and subscription support
- Azure products and services documentation
- Online self-help documentation
- Whitepapers
- Community support forums

## Paid Azure support plans

Microsoft offers four paid Azure support plans for customers who require technical and operational support: Developer, Standard, Professional Direct, and Premier.

|                              | Developer                                            | Standard                                             | Professional Direct                                          | Premier                                                      |
| :--------------------------- | :--------------------------------------------------- | :--------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| Scope                        | Trial and non-production environments                | Production workload environments                     | Business-critical dependence                                 | Substantial dependence across multiple products              |
| Technical Support            | Business hours access to Support Engineers via email | 24x7 access to Support Engineers via email and phone | 24x7 access to Support Engineers via email and phone         | 24x7 access to Support Engineers via email and phone         |
| Case Severity/Response Times | Minimal business impact (Sev C): <8 business hours   | Critical business impact (Sev A): <1 hour            | Critical business impact (Sev A): <1 hour                    | Critical business impact (Sev A): <1 hour <15 minutes (with Azure Rapid Response or Azure Event Management) |
| Architecture Support         | General guidance                                     | General guidance                                     | Architectural guidance based on best practice delivered by ProDirect Delivery Manager | Customer-specific architectural support such as design reviews, performance tuning, configuration, and more |
| Operations Support           |                                                      |                                                      | Onboarding services, service reviews, Azure Advisor consultations | Technical account manager-led service reviews and reporting  |
| Training                     |                                                      |                                                      | Azure Engineering-led web seminars                           | Azure Engineering-led web seminars, on-demand training       |
| Proactive Guidance           |                                                      |                                                      | ProDirect Delivery Manager                                   | Designated Technical Account Manager                         |
| Launch Support               |                                                      |                                                      |                                                              | Azure Event Management (available for additional fee)        |

Providing different Azure support options allows Azure customers to choose a plan that best fits their needs.

## Support-plan availability and billing

The support plans available and how you're charged depends on the type of Azure customer you are, and the type of Azure subscription you have.

For example, Developer support isn't available to Enterprise customers. Enterprise customers can purchase Standard, Professional Direct, and Premier support plans, and be billed for support as part of an Enterprise Agreement (EA). Alternatively, if you purchase a support plan within a pay-as-you-go subscription, your support plan is charged to your monthly Azure subscription bill.

## Other support options

Several additional support channels are available outside Azure's official support plans.

| Channel                                       | Description                                                  |
| :-------------------------------------------- | :----------------------------------------------------------- |
| **Azure Knowledge Center**                    | The [Azure Knowledge Center](https://azure.microsoft.com/resources/knowledge-center/) is a searchable database that contains answers to common support questions, from a community of Azure experts, developers, customers, and users. You can browse through all responses within the Azure Knowledge Center. Find specific solutions by entering keyword search terms into the text-entry field and further refine your search results by selecting products or tags from the lists provided by two dropdown lists. |
| **Microsoft Developer Network (MSDN) Forums** | Get support by reading responses to Azure technical questions from Microsoft's developers and testers on the [MSDN Azure discussion forums](https://social.msdn.microsoft.com/Forums/home?category=windowsazureplatform). |
| **Stack Overflow**                            | You can review answers to questions from the development community on [StackOverflow](https://stackoverflow.com/questions/tagged/azure/). |
| **Server Fault**                              | Review community responses to questions about System and Network Administration in Azure on [ServerFault](https://serverfault.com/questions/tagged/azure). |
| **Azure Feedback Forums**                     | Read ideas and suggestions for improving Azure made by Azure users and customers on the [Azure feedback forums](https://feedback.azure.com/forums/34192--general-feedback). |
| **Twitter**                                   | Tweet `@AzureSupport` to get answers and support from the [official Microsoft Azure Twitter channel](https://twitter.com/azuresupport). |

------

## Next unit: Summary

[Continue](https://docs.microsoft.com/en-us/learn/modules/create-an-azure-account/7-summary)










# PART 5: Core Cloud Services - Manage services with the Azure portal

# Introduction

- 3 minutes

Azure is a cloud platform that provides the compute, storage, and networking resources needed to build cloud-hosted applications. As a new user, the Azure Portal is likely to be the primary way you will interact with Azure. The Azure Portal lets you create and manage all your Azure resources. For example, you can set up a new database, increase the compute power of your virtual machines, and monitor your monthly costs. It's also a great learning tool since you can survey all available resources and use guided wizards to create the ones you need.

Here you will learn how to sign in to the portal and navigate the portal interface. You will also learn how to customize the dashboard, so it is convenient to locate and monitor your most essential services.

## Learning objectives

In this module, you will:

- Learn about Azure management options
- Navigate the Azure portal
- Customize the dashboard

------

## Next unit: Azure management options

[Continue](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/2-azure-management)









# Azure management options

- 7 minutes

You can configure and manage Azure using a broad range of tools and platforms. There are tools available for the command line, language-specific Software Development Kits (SDKs), developer tools, tools for migration, and many others.

Tools that are commonly used for day-to-day management and interaction include:

- **Azure portal** for interacting with Azure via a Graphical User Interface (GUI)
- **Azure PowerShell** and **Azure Command-Line Interface** (CLI) for command line and automation-based interactions with Azure
- **Azure Cloud Shell** for a web-based command-line interface
- **Azure mobile app** for monitoring and managing your resources from your mobile device

## Azure portal

The [Azure portal](https://portal.azure.com/) is a public website that you can access with any web browser. Once you sign in with your Azure account, you can create, manage and monitor any available Azure services. You can identify a service you're looking for, get links for help on a topic, and deploy, manage, and delete resources. It also guides you through complex administrative tasks using wizards and tooltips.

![Screenshot of the Azure portal](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/media/2-azure-portal.png)

The dashboard view provides high-level details about your Azure environment. You can customize the dashboard by moving and resizing tiles, and displaying services you're interested in.

The portal doesn't provide any way to automate repetitive tasks. For example, to set up multiple VMs, you would need to create them one at a time by completing the wizard for each VM. This makes the portal approach time-consuming and error-prone for complex tasks.

## Azure PowerShell

Azure PowerShell is a module that you can install for Windows PowerShell, or PowerShell Core, which is a cross-platform version of PowerShell that runs on Windows, Linux or macOS. Azure PowerShell enables you to connect to your Azure subscription and manage resources. Windows PowerShell and PowerShell Core provide services such as the shell window and command parsing. Azure PowerShell then adds the Azure-specific commands.

For example, Azure PowerShell provides the `New-AzureRmVM` command that creates a virtual machine for you inside your Azure subscription. To use it, you would launch PowerShell, install the Azure PowerShell module, sign in to your Azure account using the command `Connect-AzureRMAccount`, and then issue a command such as:

PowerShellCopy

```powershell
New-AzureRmVm `
    -ResourceGroupName "MyResourceGroup" `
    -Name "TestVm" `
    -Image "UbuntuLTS"
    ...
```

Creating administration scripts and using automation tools is a powerful way to optimize your workflow. You can automate repetitive tasks. Once a script is verified, it runs consistently, which can reduce errors. Another scripting environment is the Azure CLI.

## Azure CLI

Azure CLI is a cross-platform command-line program that connects to Azure and executes administrative commands on Azure resources. *Cross-platform* means that it can be run on Windows, Linux, or macOS. For example, to create a VM, you would open a command prompt window, sign in to Azure using the command `az login`, create a resource group, then use a command such as:

Azure CLICopy

```azurecli
az vm create \
  --resource-group MyResourceGroup \
  --name TestVm \
  --image UbuntuLTS
  --generate-ssh-keys
  ...
```

## Azure Cloud Shell

[Azure Cloud Shell](https://shell.azure.com/) is a browser-based scripting environment for command-line administration of Azure resources. It provides support for two shell environments. Linux users can opt for a Bash experience, while Windows users can use PowerShell.

![Screenshot of Azure Cloud Shell](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/media/2-cloud-shell.png)

Both environments support the Azure CLI and Azure PowerShell CLIs. Linux defaults to the Azure CLI (with the `az`command pre-installed), but you can switch to PowerShell for Linux by typing `pwsh`. The Windows-based environment has both CLI tools pre-installed. In addition to these administrative tools, the Cloud Shell has a suite of developer tools, text editors, and other tools available including:

**Developer Tools**

- .NET Core
- Python
- Java
- Node.js
- Go

**Editors**

- code (Cloud Shell Editor)
- vim
- nano
- emacs

**Other tools**

- git
- maven
- make
- npm
- [and more...](https://docs.microsoft.com/azure/cloud-shell/features#tools)

You can create, build, and deploy apps right from this browser-based environment. It's all persistent as well - you're prompted to create an Azure Storage Account when you access the Azure Cloud Shell. This storage area is used as your $HOME folder and any scripts or data you place here is kept across sessions. Each subscription has a unique storage account associated with it so you can keep the data and tools you need right for each account you manage.

We'll use the Cloud Shell in Microsoft Learn for many of the interactive exercises to try out Azure features.

## Azure mobile app

![Screenshot of the Azure mobile app](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/media/2-azure-mobile-app.png)

The [Microsoft Azure mobile app](https://aka.ms/azuremobileapp/) allows you to access, manage, and monitor all your Azure accounts and resources from your iOS or Android phone or tablet. Once installed, you can:

- Check the current status and important metrics of your services
- Stay informed with notifications and alerts about important health issues
- Quickly diagnose and fix issues anytime, anywhere
- Review the latest Azure alerts
- Start, stop, and restart virtual machines or web apps
- Connect to your virtual machines
- Manage permissions with role-based access control (RBAC)
- Use the Azure Cloud Shell to run saved scripts or perform ad hoc administrative tasks
- and more...

## Other options

There are also Azure SDKs for a range of languages and frameworks, and REST APIs that you can use to manage and control Azure resources programmatically. For a full list of tools available, see the [Downloads](https://azure.microsoft.com/downloads/) page.

When starting with Azure, you'll most often use the Azure portal. Let's take a closer look at the portal approach.

------

## Next unit: Navigate the portal

[Continue](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/3-navigate-the-portal)


​    

  



# Navigate the portal

- 10 minutes

With an Azure account, we can sign into the **Azure portal**. The portal is a web-based administration site that lets you interact with all of your subscriptions and resources you have created. Almost everything you do with Azure can be done through this web interface.

## Azure portal layout

The Azure portal is the primary graphical user interface (GUI) for controlling Microsoft Azure. You can carry out the majority of management actions in the portal, and it is typically the best interface for carrying out single tasks or where you want to look at the configuration options in detail.

![Screenshot of the Azure portal](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/media/3-portal.png)

![Screenshot of the resources and favorites blade](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/media/3-favorites.png)

**Resource Panel**

In the left-hand sidebar of the portal is the resource pane, which lists the main resource types. Note that Azure has more resource types than just those shown. The resources listed are part of your *favorites*.

You can customize this with the specific resource types you tend to create or administer most often.

You can also collapse this pane; with the **<<** caret. This will minimize it to just icons which can be convenient if you are working with limited screen real-estate.

The remainder of the portal view is for the specific elements you are working with. The default (main) page is the *dashboard*. We'll cover later, but this represents a customizable birds-eye-view of your resources. You can use it to jump into specific resources you want to manage or search for resources with the **All resources** entry in the resource panel. When you are managing a resource, such as a virtual machine or a web app, you will work with a *blade* that presents specific information about the resource.

## What is a blade?

The Azure portal uses a blades model for navigation. A *blade* is a slide-out panel containing the UI for a single level in a navigation sequence. For example, each of these elements in this sequence would be represented by a blade: **Virtual machines** > **Compute** > **Ubuntu Server**.

Each blade contains some information and configurable options. Some of these options generate another blade, which reveals itself to the right of any existing blade. On the new blade, any further configurable options will spawn another blade, and so on. Soon, you can end up with several blades open at the same time. You can maximize blades as well so that they fill the entire screen.

Since new blades are always added to the right of the owner, you can use the scrollbar at the bottom of the window to go backward to see how you got to this spot in the configuration. Alternatively, you can close blades individually by clicking the `X` button in the top corner of the blade. If you have unsaved changes, Azure will prompt you to let you know that the changes will be lost if you continue.

## What is the Azure Marketplace?

One of the blades you can access in the portal is the *Azure Marketplace*. This blade is often where you will start when creating new resources in Azure. The Marketplace allows customers to find, try, purchase, and provision applications and services from hundreds of leading service providers, all certified to run on Azure.

The solution catalog spans several industry categories, including but not limited to open-source container platforms, virtual machine images, databases, application build and deployment software, developer tools, threat detection, and blockchain. Using Azure Marketplace, you can provision end-to-end solutions quickly and reliably, hosted in your own Azure environment. At the time of writing, this includes over 8,000 listings.

 Note

While Azure Marketplace is designed for IT professionals and cloud developers interested in commercial and IT software, Microsoft Partners also use it as a launch point for all joint Go-To-Market activities.

## Configuring settings in the Azure portal

The Azure portal displays several configuration options, mostly in the status bar at the top-right of the screen.

### Notifications

Clicking the bell icon displays the **Notifications** pane. This pane lists the last actions that have been carried out, along with their status.

### Cloud Shell

If you click the **Cloud Shell** icon (>_), you will create a new Azure Cloud Shell session. Recall that Azure Cloud Shell is an interactive, browser-accessible shell for managing Azure resources. It provides the flexibility of choosing the shell experience that best suits the way you work. Linux users can opt for a Bash experience, while Windows users can opt for PowerShell. This browser-based terminal lets you control and administer all of your Azure resources in the current subscription through a command-line interface built right into the portal.

### Settings

Click the **gear** icon to change the Azure portal settings. These settings include:

- Sign out time
- Color and contrast themes
- Toast notifications (to a mobile device)
- Language and regional format

![Screenshot of the Portal settings blade](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/media/3-settings-blade.png)

When you have changed settings, click **Apply** to accept your changes.

### Feedback blade

The **smiley face** icon opens the **Send us feedback** blade. Here you can send feedback to Microsoft about Azure. You can decide as part of your feedback whether Microsoft can respond to your feedback by email.

### Help blade

Click the **question mark** icon to show the **Help** blade. Here you choose from several options, including:

- Help + Support
- What's new
- Azure roadmap
- Launch guided tour
- Keyboard shortcuts
- Show diagnostics
- Privacy + terms

#### Help + Support options

This opens the main support area for the Azure portal and includes documentation options for a variety of common questions. One of the hidden areas here is the **New support request** link which is on this page. This is how you can open a support ticket with the Azure team.

 Note

All Azure customers can access billing, quota, and subscription-management support. *The availability of support for other issues depends on the support plan you have*.

When you open a support ticket, you will complete the **Problem** section of the form by using provided dropdown lists and text-entry fields. - In the **Title** text-entry field, describe your issue briefly. Provide additional information about your issue in the **Details** text-entry field. - Provide your contact information by choosing your **preferred contact method** and entering your contact details, as prompted by the form.

Once you've filled out the form, select **Create** to submit your support request. The Azure support team will contact you after you submit your request.

You can then check the status and details of your support request, through the **All support requests** from the **Help + support** blade.

### Directory and subscription

Click the **Book and Filter** icon to show the **Directory + subscription** blade.

Azure allows you to have more than one subscription associated with one directory. On the **Directory + subscription**blade, you can change between subscriptions. Here, you can change your subscription or change to another directory.

![Screenshot of the Directory and subscription blade.](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/media/3-directory-blade.png)

### Profile settings

If you click on your name in the top right-hand corner, a menu opens with a few options:

- Sign in with another account, or sign out entirely
- View your account profile, where you can change your password
- Check your permissions
- View your bill (click the "..." button on the right-hand side)
- Update your contact information (click the "..." button on the right-hand side)

If you click "..." and then **View my bill**, Azure takes you to the **Cost Management + Billing - Invoices** page, which helps you analyze where Azure is generating costs.

Azure is a large product, and the Azure portal user interface (UI) reflects this. The sliding blade approach allows you to navigate back and forth through the various administrative tasks with ease. Let's experiment a bit with this UI so you get some practice.

### Azure Advisor

Finally, the Azure Advisor is a free service built into Azure that provides recommendations on high availability, security, performance, and cost. Advisor analyzes your deployed services and looks for ways to improve your environment across those four areas. You can view recommendations in the portal or download them in PDF or CSV format.

With Azure Advisor, you can:

- Get proactive, actionable, and personalized best practices recommendations.
- Improve the performance, security, and high availability of your resources as you identify opportunities to reduce your overall Azure costs.
- Get recommendations with proposed actions inline.

You can access Azure Advisor by selecting **Advisor** from the navigation menu, or search for it in the **All Services** menu.

![Azure Advisor Dashboard displayed in the Azure Portal displaying recommendations for High Availability, Security, Performance and Cost](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/media/3-advisordashboard.png)

Let's try some of these features out!

------

## Next unit: Exercise - Work with blades

[Continue](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/4-exercise-work-with-blades)










# Exercise - Work with blades

- 10 minutes

This module requires a sandbox to complete. A sandbox gives you access to Azure resources. Your Azure subscription will not be charged.

Activate sandbox

In this unit, you will learn how to work with blades in the Azure portal user interface (UI).

## Activate the Azure sandbox

1. Start by **activating the Azure sandbox above**.
2. Once it's activated, sign into the [Azure portal for sandbox ](https://portal.azure.com/learn.docs.microsoft.com). Make sure to use the same account you activated the sandbox with.

## Working with blades

Once you are logged into the Azure portal, we can start exploring things. In these sections, you will get a tour of the "blades" user interface element (windows within the Azure portal window), but you will not actually create any Azure resources.

1. Let's start by touring how to create a resource. In the left-hand portion of the portal click **Create a resource**.
2. A blade labeled **New** appears and displays a list of categories on the left-hand side, labeled Azure Marketplace. This is somewhat like a "Popular Categories" menu, with some of the most common categories visible. If you'd like, you can expand this list to see everything in the **Marketplace** blade with the **See all** link next to the heading. If you do, you can get back to the New blade by clicking the X icon in the upper right of any blades you have opened.
3. Selecting any of items in the Azure Marketplace list will show popular services for that category on the right of the **New** blade. This list is a subset of the entire range of computing resources available for that category. As with the Azure Marketplace, you can click on the **See all** link for a more comprehensive list. We will talk more about this list in subsequent sections.
4. Returning to the **New** blade, click on **Get started** and you should see a list on the right side of the blade that includes services such as Windows Server 2016 VM, Ubuntu Server VM, SQL Database, and so on. Most of these items include a **Quickstart tutorial** link directly below the name. Clicking this link will open a new browser tab with the quickstart Microsoft documentation for that item, if you need it.
5. Optional: Click **Quickstart tutorial** under **Windows Server 2016 VM** and, in the new browser window, look through the Windows VM tutorials. When you are finished, close this new tab to return to the Azure portal.

## Viewing resources

1. Under Azure Marketplace, click **Compute** to show more compute options on the right side of the blade, such as Red Hat Enterprise, Reserved VM Instances, Web app for Containers, and so on.
2. To the right of **Featured**, click **See all**. The full list of available VM services now appears.
3. Under **Recommended**, click **Windows Server**. A new **Windows Server** blade appears to the right.
4. To the right of the **Pin blade to dashboard** icon in the blade's title bar, click the **Maximize** icon (it looks like a simple empty square or box). The Windows Server blade now fills the screen, except for the left-hand pane. Scroll down the list to see all of the Windows Server images available.
5. Optionally, you can click the **Restore** icon (similar to the Maximize icon, a simple empty square or box with another one on top) to return to the previous blade view.
6. Click the **X** at the top right-hand corner to close the **Windows Server** blade. You should now see the **New** blade again.

## Filtering results

1. Another way to locate services is to refine the list with filters and search terms. On the **New** blade, you may have noticed the search box at the top. This is the quickest way to filter what services you see, but this search checks every Azure service to get its results. If you'd like to learn how to filter after selecting a category, continue to the next steps.
2. On the **Compute** blade, you can see these various options at the top, a search box and some labeled dropdown boxes.
3. Type `virtual machine images` into the search box and press ENTER. You should now see a filtered list of Compute services related to virtual machine images.
4. Explore the available dropdown filter boxes by clicking on the down arrow (it looks a bit like a chevron) and try some of them out. When you are satisfied, move on to the next step.
5. Click the **X** in the right-hand end of the search box. This will erase your search term but does not reset any of the drop-down filters you've set. You can either reset those manually, or simply close the **Compute** blade with the X icon in the upper right corner and re-open it. When you are finished trying out the search and filtering options, move on to the next step.
6. Click the **X** at the top right-hand corner to close the **Compute** blade.
7. Click the **X** at the top right-hand corner to close the **Marketplace** blade. Now you will see the **New** blade once again.
8. Click the **X** at the top right-hand corner to close the **New** blade.

The default dashboard now appears.

Many of the principles you have learned in this exercise will apply throughout the Azure portal UI experience. In the next unit, you will continue your journey in the Azure portal and configure additional settings in Azure.

------

## Next unit: Exercise - Use the Azure portal

[Continue](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/5-exercise-navigate-the-portal)











# Exercise - Use the Azure portal

- 10 minutes

Sandbox activated! Time remaining:

 

3 hr 54 min

The Azure Portal has a lot of features and services available; let's look at some of the more common areas you'll tend to use. First, take a moment to hover your mouse pointer over each of the icons in the top menu bar for a few seconds each. You should see a tooltip label pop up for each one. This is the name of the menu item. You will use these icons later.

![Screenshot of the Azure portal icon bar](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/media/5-portal-icon-bar.png)

## Services blade

1. In the left-hand pane, click **All services**. Take a couple of minutes to scroll down the list to see how many services Azure offers.

   ![Screenshot of the services blade](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/media/5-services.blade.png)

2. You can search for services through the *filter* box.

3. Select **Virtual machines**. If you don't see it, use the filter box. The **Virtual Machines** blade appears. There is nothing currently showing because you have not defined any virtual machines.

4. Click the **+ Add** button. The **Create a virtual machine** blade appears, as in the previous exercise.

5. Click the **X** in the top right-hand corner to close the **Create a virtual machine** blade.

6. Click the **X** in the top right-hand corner to close the **Virtual machines** blade.

7. You should now be back at the Dashboard page. If not, you can always click on **Dashboard** in the left-most pane.

## Notifications blade

1. On the icon bar menu bar, click the **Notifications** (bell) icon. This will list any pending notifications.

   ![Screenshot of notifications window](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/media/5-notifications-blade.png)

2. If any notifications appear, hover your mouse over one of them. Click the **X** that appears in that notification to dismiss it.

3. To the right of **Dismiss**, click **All**. You should have no notifications showing.

4. Click the **X** in the top right-hand corner to close the **Notifications** pane.

## Azure Cloud Shell

![Icon representing the Azure Cloud Shell](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/media/5-cloud-shell-icon.png)

The Azure Cloud Shell allows you to use a command-line interface (CLI) to execute commands in your Azure subscription. You can access it by clicking the (`>_`) icon in the toolbar. However, it isn't available in the Sandbox environment - so you will only be able to do this in your own active subscriptions. You can also navigate to [https://shell.azure.com](https://shell.azure.com/) to launch a Cloud Shell in the browser independent of the portal.

When you launch the shell, you will see a Welcome window. You can choose either a **Bash** or **PowerShell** environment, depending on your personal preferences. You can also change the shell at anytime through the language drop-down on the left side of the shell.

Finally, there are a variety of management and programming tools included in the created environment.

- Azure command-line tools (Azure CLI, AzCopy, etc.)
- Languages / Frameworks including .NET Core, Python, and Java
- Container management support for Docker, Kubernetes, etc.
- Code editors such as vim, emacs, code, and nano
- Build tools (make, maven, npm, etc.)
- Database query tools such as `sqlcmd`

## Settings

![Icon representing the settings panel](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/media/5-settings-icon.png)

1. Click the **Settings** (cog) icon to open the **Portal settings** pane.
2. Drop down the **Log me out when inactive** setting, and select **After one hour**.
3. Under **Choose a theme**, select the different colored themes and observe the changes to the portal UI. Leave it set to the one you like the best.
4. Under **High contrast theme**, try the three different options.
5. Disable Toast notifications. This means notifications will not appear as pop-up "toast"-style notifications, but will still show up in the Notifications (bell) icon as always.
6. Note the **Allow double-click on dashboard to change theme** setting, enabled by default. When enabled, you can use the mouse to cycle through the various color themes without opening this Settings menu by double-clicking the left mouse button in the Dashboard view's background area. Disable this option to avoid accidentally changing your color theme.
7. Click **Apply** to accept your changes.
8. Click the **Settings** (cog) icon in the top menu bar and, under **Language**, select **Español**, and then click the **Refresh**button. If a **Translate this page** dialog box appears, close the box. Note that the whole portal is now in Spanish.
9. Click the **Settings** (cog) icon in the top menu bar and, under **Language**, select **English**. Click the **Actualizar** button. The portal returns to English.

## Feedback blade

![Icon representing the feedback panel](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/media/5-feedback-icon.png)

1. Click the **Feedback** (smiley face) icon to open the **Send us feedback** blade.
2. Type your impressions of Azure in the **Tell us about your experience** box, click the box that says **Microsoft can email you about your feedback**, and click **Submit Feedback**.
3. A **Feedback sent** message will appear, and then close. You should now be back at the Dashboard.

## Help blade

![Icon representing the feedback panel](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/media/5-help-icon.png)

1. Click the **Help** (`?`) icon to show the **Help** blade.
2. Click the **Help + Support** button.
3. In the **Help + Support** blade, under **Support**, click **New support request**. To create a new support request, you would fill in the information in each of the following sections, and then click **Create** to lodge the issue.
   - **Basics:** the issue type
   - **Problem:** severity of the problem, a summary and description, and any additional information
   - **Contact information:** preferred contact method and the information associated with this contact method
4. You can view the status of your support requests by clicking on **All support requests**.

 Note

Support requests can only be created using an active paid subscription. Creating support requests from a free Microsoft Learn sandbox is not supported.

### What's new and other information

1. Click the **Help** icon and click **What's new**.
2. Review the features that have recently been released. Also note and explore the other **Help** menu options, such as:

- Azure roadmap
- Launch guided tour
- Keyboard shortcuts
- Show diagnostics
- Privacy + terms

1. Click the **X** in the top right-hand corner to close the **Help** blade.
2. Close the **What's new** blade. You should now be back to the Dashboard.

## Directory and subscription

![Icon representing the subscription panel](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/media/5-subscription-icon.png)

1. Click the **Directory + Subscription** (book and filter) icon to show the **Directory + subscription** blade.

   This is where you can switch between multiple subscriptions or directories. You should see the Concierge subscription here, and if you have an Azure account tied to the same email address, your own subscription.

   There is also a link to learn more about directories and subscriptions.

2. Click the **X** in the top right-hand corner to close the **Directory + subscription** blade.

## Profile settings

1. Click on your name in the top right-hand corner of the portal. Options include:

   - Sign in with another account, or sign out entirely
   - View your account profile, where you can change your password
   - Submit an idea
   - Check your permissions
   - View your bill
   - Update your contact information

   Note that some items do not appear unless you click the "..." icon.

2. Click "..." then **View my bill** to navigate to the **Cost Management + Billing - Invoices** page, which helps you analyze where Azure is generating costs.

3. If you're using your own account and not sandbox, you can select a subscription from the drop-down list.

4. Click a billing period.

5. Note the service costs and check them against what you expect for your current subscription.

6. Click the **X** in the top right-hand corner to close the **Costs by service** blade.

7. Click the **X** in the top right-hand corner to close the **Cost Management + Billing - Invoices** page.

8. You should now be back at the Dashboard.

Now that we've explored all the main areas of the Azure portal, let's look at one of the most useful features - Dashboards.

------

## Next unit: Azure Portal dashboards

[Continue](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/6-customize-the-dashboard)







# PART 6: Core Cloud Services - Azure compute options

  Introduction

- 1 minute

Imagine that you've landed your dream job as a developer at a new space technology firm. On your first day, you're assigned to help researchers analyze a large dataset being generated for a cutting-edge research project to explore water on Mars — and time is of the essence. But there's a problem; you don't have any free servers to do the work. And even if they did appear, you'd need to invest a lot of time to set them up and install software.

![Concept of the sun being center of our solar system](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-compute/media/1-heading.png)

Of course you could ask to buy new equipment, but your department's budget is tight. Plus, you don't want to buy more hardware than needed, not only because you want to make a good impression with leadership, but also because you just don't know how much data will be generated by this project.

Ideally, you'd obtain the resources you need to do the work without too much administration — and simply configure them to do the work. And you'd pay only for the compute resources you need while you're using them.

This is exactly what we can do in Azure. We can create compute resources, configure them to do the work we need, and pay only for what we use.

## Learning objectives

In this module, you will:

- Identify compute options in Azure
- Select compute options that are appropriate for your business

------

## Next unit: Essential Azure compute concepts

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-compute/2-essential-azure-compute-concepts)









# Essential Azure compute concepts

- 7 minutes

Your research team has collected massive amounts of image data that might lead to a discovery on Mars. They need to perform computationally intense data processing but don't have the equipment to do the work. Let's see why Azure is a good choice to do the data analysis.

## What is Azure compute?

Azure compute is an on-demand computing service for running cloud-based applications. It provides computing resources like multi-core processors and supercomputers via virtual machines and containers. It also provides serverless computing to run apps without requiring infrastructure setup or configuration. The resources are available on-demand and can typically be created in minutes or even seconds. You pay only for the resources you use and only for as long as you're using them.

There are four common techniques for performing compute in Azure:

- Virtual machines
- Containers
- Azure App Service
- Serverless computing

## What are virtual machines?

**Virtual machines**, or VMs, are software emulations of physical computers. They include a virtual processor, memory, storage, and networking resources. They host an operating system (OS), and you're able to install and run software just like a physical computer. And by using a remote desktop client, you can use and control the virtual machine as if you were sitting in front of it.

## What are containers?

Containers are a virtualization environment for running applications. Just like virtual machines, containers are run on top of a host operating system but unlike VMs, they don't include an operating system for the apps running *inside* the container. Instead, containers bundle the libraries and components needed to run the application and use the existing host OS running the container. For example, if five containers are running on a server with a specific Linux kernel, all five containers and the apps within them share that same Linux kernel.

## What is Azure App Service?

Azure App Service is a platform-as-a-service (PaaS) offering in Azure that is designed to host enterprise-grade web-oriented applications. You can meet rigorous performance, scalability, security, and compliance requirements while using a fully managed platform to perform infrastructure maintenance.

## What is Serverless Computing?

Serverless computing is a cloud-hosted execution environment that runs your code but completely abstracts the underlying hosting environment. You create an instance of the service, and you add your code; no infrastructure configuration or maintenance is required, or even allowed.

## Which computing strategy is right for me?

You don't need to take an "all or nothing" approach when choosing a cloud computing strategy. Virtual machines, containers, App Service, and serverless computing each provide benefits as well as tradeoffs against other options.

For example, although serverless computing removes the need for you to manage infrastructure, serverless computing expects work to be completed quickly; usually within seconds or less. Therefore, you might run your core application on a virtual machine or container but offload some of the data processing onto a serverless app.

Let's look at each option more closely to help you decide when to use each service.

------

## Next unit: Explore Azure Virtual Machines

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-compute/3-virtual-machines)


​    



  

# Explore Azure Virtual Machines

- 5 minutes

![Image representing Azure virtual machines](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-compute/media/3-azure-vms.png)

Azure Virtual Machines (VMs) let you create and use virtual machines in the cloud. They provide infrastructure as a service (IaaS) in the form of a virtualized server and can be used in many ways. Just like a physical computer, you can customize all of the software running on the VM. VMs are an ideal choice when you need:

- Total control over the operating system (OS)
- The ability to run custom software, or
- To use custom hosting configurations

You can create and provision a VM in minutes when you select a pre-configured VM image. Selecting an image is one of the most important decisions you'll make when creating a VM. An image is a template used to create a VM. These templates already include an OS and often other software, like development tools or web hosting environments.

## Moving to the cloud with VMs

VMs are also an excellent choice when moving from a physical server to the cloud ("lift and shift"). You can create an image of the physical server and host it within a VM with little or no changes. Just like a physical on-premises server, you must maintain the VM. Update the OS and the software it runs.

## Scaling VMs in Azure

You can run single VMs for testing, development, or minor tasks, or group VMs together to provide high availability, scalability, and redundancy. Azure has several features so that no matter what your uptime requirements are, Azure can meet them. These features include:

- Availability sets
- Virtual Machine Scale Sets
- Azure Batch

### What are availability sets?

An **availability set** is a logical grouping of two or more VMs that help keep your application available during planned or unplanned maintenance.

A *planned maintenance event* is when the underlying Azure fabric that hosts VMs is updated by Microsoft. A planned maintenance event is done to patch security vulnerabilities, improve performance, and add or update features. Most of the time these updates are done without any impact to the guest VMs. But sometimes VMs require a reboot to complete an update. When the VM is part of an availability set, the Azure fabric updates are sequenced so not all of the associated VMs are rebooted at the same time. VMs are put into different *update domains*. Update domains indicate groups of VMs and underlying physical hardware that can be rebooted at the same time. Update domains are a logical part of each data center and are implemented with software and logic.

*Unplanned maintenance events* involve a hardware failure in the data center, such as a power outage or disk failure. VMs that are part of an availability set automatically switch to a working physical server so the VM continues to run. The group of virtual machines that share common hardware are in the same *fault domain*. A fault domain is essentially a rack of servers. It provides the physical separation of your workload across different power, cooling, and network hardware that support the physical servers in the data center server racks. In the event the hardware that supports a server rack becomes unavailable, only that rack of servers is affected by the outage.

With an availability set, you get:

- Up to three fault domains that each have a server rack with dedicated power and network resources
- Five logical update domains

Your VMs are then sequentially placed across the fault and update domains. The following diagram shows an example where you have six VMs in an availability set distributed across the two fault domains and five update domains.

![Diagram that shows availability sets update and fault domains that are duplicated across servers](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-compute/media/3-availability-sets.png)

There's no cost for an availability set. You only pay for the VMs within the availability set. We highly recommend that you place each workload in an availability set to avoid a single point of failure in your VM architecture.

### What are virtual machine scale sets?

Azure Virtual Machine Scale Sets let you create and manage a group of identical, load balanced VMs. Imagine you're running a website that enables scientists to upload astronomy images that need to be processed. If you duplicated the VM, you'd normally need to configure an additional service to route requests between multiple instances of the website. VM Scale Sets could do that work for you.

Scale sets allow you to centrally manage, configure, and update a large number of VMs in minutes to provide highly available applications. The number of VM instances can automatically increase or decrease in response to demand or a defined schedule. With VM Scale Sets, you can build large-scale services for areas such as compute, big data, and container workloads.

### What is Azure Batch?

Azure Batch enables large-scale job scheduling and compute management with the ability to scale to tens, hundreds, or thousands of VMs.

When you're ready to run a job, Batch:

- Starts a pool of compute VMs for you
- Installs applications and staging data
- Runs jobs with as many tasks as you have
- Identifies failures
- Requeues work
- Scales down the pool as work completes

There may be situations in which you need raw computing power or supercomputer level compute power. Azure provides these capabilities.

------

## Next unit: Explore Containers in Azure

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-compute/4-containers)








# Explore Containers in Azure

- 10 minutes

![Image representing Azure containers](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-compute/media/4-azure-containers.png)

If you wish to run multiple instances of an application on a single virtual machine, containers are an excellent choice. The container orchestrator can start, stop, and scale out application instances as needed.

Containers are meant to be lightweight, created, scaled out, and stopped dynamically. This design allows you to respond quickly to changes in demand or failure.

Another benefit of containers is you can run multiple isolated applications on a single VM host. Since containers are secured and isolated, you don't need separate VMs for each app.

#### VMs versus containers

<iframe id="RE2yuaq-ax-0-id-oneplayer" src="https://www.microsoft.com/en-us/videoplayer/embed/RE2yuaq?pid=RE2yuaq-ax-0-id-oneplayer&amp;jsapi=true&amp;postJsllMsg=true&amp;autoplay=false&amp;mute=false&amp;loop=false&amp;market=en-us&amp;playFullScreen=false" class="oneplayer-iframe" allowfullscreen="true" frameborder="0" name="Oneplayer iframe" title="Video: RE2yuaq" style="width: 640px; box-sizing: inherit; position: absolute; top: 0px; left: 0px; right: 0px; bottom: 0px; height: 360px;"></iframe>

## Containers in Azure

Azure supports Docker containers, and there are several ways to manage containers in Azure.

- Azure Container Instances (ACI)
- Azure Kubernetes Service (AKS)

### Azure Container Instances

Azure Container Instances (ACI) offers the fastest and simplest way to run a container in Azure. You don't have to manage any virtual machines or configure any additional services. It is a PaaS offering that allows you to upload your containers and execute them directly.

### Azure Kubernetes Service

The task of automating and managing and interacting with a large number of containers is known as orchestration. Azure Kubernetes Service (AKS) is a complete orchestration service for containers with distributed architectures with multiple containers.

#### What is Kubernetes?

<iframe id="RE2yEuX-ax-1-id-oneplayer" src="https://www.microsoft.com/en-us/videoplayer/embed/RE2yEuX?pid=RE2yEuX-ax-1-id-oneplayer&amp;jsapi=true&amp;postJsllMsg=true&amp;autoplay=false&amp;mute=false&amp;loop=false&amp;market=en-us&amp;playFullScreen=false" class="oneplayer-iframe" allowfullscreen="true" frameborder="0" name="Oneplayer iframe" style="width: 640px; box-sizing: inherit; position: absolute; top: 0px; left: 0px; right: 0px; bottom: 0px; height: 360px;"></iframe>

### Using containers in your solutions

Containers are often used to create solutions using a *microservice architecture*. This is where you break solutions into smaller, independent pieces. For example, you may split a website into a container hosting your front end, another hosting your back end, and a third for storage. This allows you to separate portions of your app into logical sections that can be maintained, scaled, or updated independently.

#### What is a microservice?

<iframe id="RE2yual-ax-2-id-oneplayer" src="https://www.microsoft.com/en-us/videoplayer/embed/RE2yual?pid=RE2yual-ax-2-id-oneplayer&amp;jsapi=true&amp;postJsllMsg=true&amp;autoplay=false&amp;mute=false&amp;loop=false&amp;market=en-us&amp;playFullScreen=false" class="oneplayer-iframe" allowfullscreen="true" frameborder="0" name="Oneplayer iframe" style="width: 640px; box-sizing: inherit; position: absolute; top: 0px; left: 0px; right: 0px; bottom: 0px; height: 360px;"></iframe>

Imagine your website backend has reached capacity but the front end and storage aren't being stressed. You could scale the back end separately to improve performance, or you could decide to use a different storage service. Or you could even replace the storage container without affecting the rest of the application.

------

## Next unit: Explore Azure App Service

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-compute/5-appservice)








# Explore Azure App Service

- 5 minutes

![Image representing Azure App Service](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-compute/media/5-appservice.png)

Azure App Service enables you to build and host web apps, background jobs, mobile backends, and RESTful APIs in the programming language of your choice without managing infrastructure. It offers auto-scaling and high availability, supports both Windows and Linux, and enables automated deployments from GitHub, Azure DevOps, or any Git repo to support a continuous deployment model.

This platform as a service (PaaS) allows you to focus on the website and API logic while Azure takes care of the infrastructure to run and scale your web applications.

## App Service costs

You pay for the Azure compute resources your app uses while it processes requests based on the App Service Plan you choose. The App Service plan determines how much hardware is devoted to your host - for example, whether it's dedicated or shared hardware, and how much memory is reserved for it. There is even a *free* tier you can use to host small, low-traffic sites.

## Types of web apps

With Azure App Service, you can host most common web app styles including:

- Web Apps
- API Apps
- WebJobs
- Mobile Apps

Azure App Service handles most of the infrastructure decisions you deal with in hosting web apps: deployment and management are integrated into the platform, endpoints can be secured, sites can be scaled quickly to handle high traffic loads, and the built-in load balancing and traffic manager provide high availability. All of these app styles are hosted in the same infrastructure and share these benefits. This makes App Service the ideal choice to host web-oriented applications.

### Web Apps

App Service includes full support for hosting web apps using ASP.NET, ASP.NET Core, Java, Ruby, Node.js, PHP, or Python. You can choose either Windows or Linux as the host operating system.

### API Apps

Much like hosting a website, you can build REST-based Web APIs using your choice of language and framework. You get full Swagger support, and the ability to package and publish your API in the Azure Marketplace. The produced apps can be consumed from any HTTP(s) based client.

### Web Jobs

WebJobs allows you to run a program (.exe, Java, PHP, Python or Node.js) or script (.cmd, .bat, PowerShell, or Bash) in the same context as a web app, API app, or mobile app. They can be scheduled, or run by a trigger. This is often used to run background tasks as part of your application logic.

### Mobile Apps

Use the Mobile Apps feature of Azure App Service to quickly build a back-end for iOS and Android apps. With just a few clicks in the Azure portal you can:

- Store mobile app data in a cloud-based SQL database
- Authenticate customers against common social providers such as MSA, Google, Twitter and Facebook
- Send push notifications
- Execute custom back-end logic in C# or Node.js

On the mobile app side, there is SDK support for native iOS & Android, Xamarin, and React native apps.

------

## Next unit: Explore Serverless computing in Azure

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-compute/6-serverless-computing)







# Explore Serverless computing in Azure

- 7 minutes

![Image representing serverless computing](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-compute/media/6-serverless.png)

With *serverless* computing, Azure takes care of managing the server infrastructure and allocation/deallocation of resources based on demand. Infrastructure isn't your responsibility. Scaling and performance are handled automatically, and you are billed only for the exact resources you use. There's no need to even reserve capacity.

You focus solely on the logic you need to execute and the *trigger* that is used to run your code. You configure your serverless apps to respond to *events*. This could be a REST endpoint, a periodic timer, or even a message received from another Azure service. The serverless app runs only when it's triggered by an event.

#### Serverless computing in Azure

<iframe id="RE2yzjL-ax-3-id-oneplayer" src="https://www.microsoft.com/en-us/videoplayer/embed/RE2yzjL?pid=RE2yzjL-ax-3-id-oneplayer&amp;jsapi=true&amp;postJsllMsg=true&amp;autoplay=false&amp;mute=false&amp;loop=false&amp;market=en-us&amp;playFullScreen=false" class="oneplayer-iframe" allowfullscreen="true" frameborder="0" name="Oneplayer iframe" title="Video: RE2yzjL" style="width: 640px; box-sizing: inherit; position: absolute; top: 0px; left: 0px; right: 0px; bottom: 0px; height: 360px;"></iframe>

Azure has two implementations of serverless compute:

- **Azure Functions** which can execute code in almost any modern language.
- **Azure Logic Apps** which are designed in a web-based designer and can execute logic triggered by Azure services without writing any code.

## Azure Functions

When you're concerned only about the code running your service, and not the underlying platform or infrastructure, Azure Functions are ideal. They're commonly used when you need to perform work in response to an event, often via a REST request, timer, or message from another Azure service and when that work can be completed quickly, within seconds or less.

Azure Functions scale automatically based on demand, so they're a solid choice when demand is variable. For example, you may be receiving messages from an IoT solution used to monitor a fleet of delivery vehicles. You'll likely have more data arriving during business hours.

Using a VM-based approach, you'd incur costs even when the VM is idle. With functions, Azure runs your code when it's triggered and automatically deallocates resources when the function is finished. In this model, you're only charged for the CPU time used while your function runs.

Furthermore, Azure Functions can be either stateless (the default) where they behave as if they're restarted every time they respond to an event), or stateful (called "Durable Functions") where a context is passed through the function to track prior activity.

## Azure Logic Apps

Azure Logic Apps are similar to Functions - both enable you to trigger logic based on an event. Where Functions execute code, Logic Apps execute *workflows* built from predefined logic blocks. They are specifically designed to automate your business processes.

You create Logic App workflows using a visual designer on the Azure Portal or in Visual Studio. The workflows are persisted as a JSON file with a known workflow schema.

Azure provides over 200 different connectors and processing blocks to interact with different services - including most popular enterprise apps. You can also build custom connectors and workflow steps if the service you need to interact with isn't covered. You then use the visual designer to link connectors and blocks together, passing data through the workflow to do custom processing - often all without writing any code.

As an example, let's say a ticket arrives in ZenDesk. You could:

1. Detect the intent of the message with cognitive services
2. Create an item in Sharepoint to track the issue
3. If the customer isn't in your database, add them to your Dynamics 365 CRM system
4. Send a follow-up email to acknowledge their request

All of that could be designed in a visual designer making it easy to see the logic flow which is ideal for a business analyst role.

## Functions vs. Logic Apps

Functions and Logic Apps can both create complex orchestrations. An orchestration is a collection of functions or steps, that are executed to accomplish a complex task. With Azure Functions, you write code to complete each step, with Logic Apps, you use a GUI to define the actions and how they relate to one another.

You can mix and match services when you build an orchestration, calling functions from logic apps and calling logic apps from functions. Here are some common differences between the two.

| -                 | Functions                                                    | Logic Apps                                                   |
| :---------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| State             | Normally stateless, but Durable Functions provide state      | Stateful                                                     |
| Development       | Code-first (imperative)                                      | Designer-first (declarative)                                 |
| Connectivity      | About a dozen built-in binding types, write code for custom bindings | Large collection of connectors, Enterprise Integration Pack for B2B scenarios, build custom connectors |
| Actions           | Each activity is an Azure function; write code for activity functions | Large collection of ready-made actions                       |
| Monitoring        | Azure Application Insights                                   | Azure portal, Log Analytics                                  |
| Management        | REST API, Visual Studio                                      | Azure portal, REST API, PowerShell, Visual Studio            |
| Execution context | Can run locally or in the cloud                              | Runs only in the cloud.                                      |

------

## Next unit: Summary

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-compute/7-summary)











# PART 7: Core Cloud Services - Azure data storage options

# Introduction

- 1 minute

Suppose you manage an online sales learning portal for your organization. The majority of your sales team are often in different geographical areas, so the online learning portal is an essential requirement. It's even more important as your organization continues to increase the skills and knowledge enhancement training for the sales staff.

![An empty bag on a map of the world representing the need for a storage solution](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/1-heading.png)

Your training data includes high-quality video, detailed sales simulations, and large repositories for maintaining student data and progress. Currently, all the training content is stored in your on-premises storage. You have an aggressive plan to add new courses and would like to avoid the need to continuously increase the local storage capacity. You're looking for a storage solution that is secure, durable, scalable, and easily accessible from across the globe.

Azure provides storage features that will meet all of your business needs.

## Learning objectives

In this module, you will:

- Survey the data storage options in Azure
- Discover how Azure data storage can meet your business demands
- Compare Azure data storage with on-premises storage

------

## Next unit: Benefits of using Azure to store data

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/2-benefits-of-using-azure-to-store-data)








# Benefits of using Azure to store data

- 6 minutes

To address the storage problem for your online learning portal, you're considering storing your data in the cloud. But you're concerned about security, backup, and disaster recovery. On top of that, you're worried about how difficult it could be to manage cloud-hosted data. So, here's what you need to know.

The Azure data storage options are cloud-based, secure, and scalable. Its features address the key challenges of cloud storage and provide you with a reliable and durable storage solution.

#### Why store your data in the cloud?

<iframe id="RE2yzjI-ax-1-id-oneplayer" src="https://www.microsoft.com/en-us/videoplayer/embed/RE2yzjI?pid=RE2yzjI-ax-1-id-oneplayer&amp;jsapi=true&amp;postJsllMsg=true&amp;autoplay=false&amp;mute=false&amp;loop=false&amp;market=en-us&amp;playFullScreen=false" class="oneplayer-iframe" allowfullscreen="true" frameborder="0" name="Oneplayer iframe" title="Video: RE2yzjI" style="width: 640px; box-sizing: inherit; position: absolute; top: 0px; left: 0px; right: 0px; bottom: 0px; height: 360px;"></iframe>

## Benefits of using Azure to store data

Here are some of the important benefits of Azure data storage:

- **Automated backup and recovery**: mitigates the risk of losing your data if there is any unforeseen failure or interruption.
- **Replication across the globe**: copies your data to protect it against any planned or unplanned events, such as scheduled maintenance or hardware failures. You can choose to replicate your data at multiple locations across the globe.
- **Support for data analytics**: supports performing analytics on your data consumption.
- **Encryption capabilities**: data is encrypted to make it highly secure; you also have tight control over who can access the data.
- **Multiple data types**: Azure can store almost any type of data you need. It can handle video files, text files, and even large binary files like virtual hard disks. It also has many options for your relational and NoSQL data.
- **Data storage in virtual disks**: Azure also has the capability of storing up to 8 TB of data in its virtual disks. This is a significant capability when you're storing heavy data such as videos and simulations.
- **Storage tiers**: storage tiers to prioritize access to data based on frequently used versus rarely used information.

## Types of data

There are three primary types of data that Azure Storage is designed to hold.

1. **Structured data**. Structured data is data that adheres to a schema, so all of the data has the same fields or properties. Structured data can be stored in a database table with rows and columns. Structured data relies on keys to indicate how one row in a table relates to data in another row of another table. Structured data is also referred to as *relational data*, as the data's schema defines the table of data, the fields in the table, and the clear relationship between the two. Structured data is straightforward in that it's easy to enter, query, and analyze. All of the data follows the same format. Examples of structured data include sensor data or financial data.
2. **Semi-structured data**. Semi-structured data doesn't fit neatly into tables, rows, and columns. Instead, semi-structured data uses *tags* or *keys* that organize and provide a hierarchy for the data. Semi-structured data is also referred to as *non-relational* or *NoSQL* data.
3. **Unstructured data**. Unstructured data encompasses data that has no designated structure to it. This also means that there are no restrictions on the kinds of data it can hold. For example, a blob can hold a PDF document, a JPG image, a JSON file, video content, etc. As such, unstructured data is becoming more prominent as businesses try to tap into new data sources.

------

## Next unit: How Azure data storage can meet your business storage needs

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/3-how-azure-storage-meets-your-business-storage-needs)










# How Azure data storage can meet your business storage needs

- 8 minutes

Looking at the benefits of Azure data storage, you understand that it offers the best options for storing your learning portal. Now let's explore the benefits and options in detail to see how it fits your business needs.

## How Azure data storage can meet your business storage needs

Azure provides several storage options that accommodate specific types of data storage needs.

![Azure SQL Database](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/3-azure-sql-db.png)

**Azure SQL Database**

Azure SQL Database is a relational database as a service (DaaS) based on the latest stable version of the Microsoft SQL Server database engine. SQL Database is a high-performance, reliable, fully managed and secure database. You can use it to build data-driven applications and websites in the programming language of your choice without needing to manage infrastructure.

You can migrate your existing SQL Server databases with minimal downtime using the Azure Database Migration Service. The service uses the *Microsoft Data Migration Assistant*to generate assessment reports that provide recommendations to help guide you through required changes prior to performing a migration. Once you assess and perform any remediation required, you're ready to begin the migration process. The Azure Database Migration Service performs all of the required steps. You just change the connection string in your apps.

The following illustration shows the types of data from the online learning portal scenario that would be stored in an Azure SQL database.

![An illustration showing Azure SQL used to store student information such as transcripts, certifications, and study materials.](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/3-azure_sql.png)

![Azure Cosmos DB](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/3-cosmos-db.png)

**Azure Cosmos DB**

Azure Cosmos DB is a globally distributed database service. It supports schema-less data that lets you build highly responsive and **Always On** applications to support constantly changing data. You can use this feature to store data that is updated and maintained by users around the world. The following illustration shows a sample Azure Cosmos DB database that's used to store data that's accessed by people located across the globe.

![An illustration showing usage of Azure Cosmos DB in the online training scenario to store the course catalog. Azure Cosmos DB is a good choice here because the catalog is updated by administrators and accessed by students all over the world.](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/3-azure_cosmos_db.png)

![Azure Blob storage](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/3-azure-blob-storage.png)

**Azure Blob storage**

Azure Blob Storage is *unstructured*, meaning that there are no restrictions on the kinds of data it can hold. Blobs are highly scalable and apps work with blobs in much the same way as they would work with files on a disk, such as reading and writing data. Blob Storage can manage thousands of simultaneous uploads, massive amounts of video data, constantly growing log files, and can be reached from anywhere with an internet connection.

Blobs aren't limited to common file formats. A blob could contain gigabytes of binary data streamed from a scientific instrument, an encrypted message for another application, or data in a custom format for an app you're developing.

Azure Blob storage lets you stream large video or audio files directly to the user's browser from anywhere in the world. Blob storage is also used to store data for backup, disaster recovery, and archiving. It has the ability to store up to 8 TB of data for virtual machines. The following illustration shows an example usage of Azure blob storage.

![An illustration showing Azure blob storage used to store and stream video or audio files.](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/3-azure_blob.png)

![Azure Data Lake Storage Gen2](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/3-azure-data-lake.png)

**Azure Data Lake Storage Gen2**

The Data Lake feature allows you to perform analytics on your data usage and prepare reports. Data Lake is a large repository that stores both structured and unstructured data.

**Azure Data Lake Storage Gen2** combines the scalability and cost benefits of object storage with the reliability and performance of the Big Data file system capabilities. The following illustration shows how Azure Data Lake stores all your business data and makes it available for analysis.

![An illustration showing the role of Azure Data Lake in preparing and storing your data for use by analysis tools. Azure Data Lake can handle a variety of input types such as relational, video, or sensor data.](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/3-data_lake_store_concept.png)

![Azure Files](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/3-azure-files.png)

**Azure Files**

Azure Files offers fully managed file shares in the cloud that are accessible via the industry standard Server Message Block (SMB) protocol. Azure file shares can be mounted concurrently by cloud or on-premises deployments of Windows, Linux, and macOS. Applications running in Azure virtual machines or cloud services can mount a file storage share to access file data, just as a desktop application would mount a typical SMB share. Any number of Azure virtual machines or roles can mount and access the file storage share simultaneously. Typical usage scenarios would be to share files anywhere in the world, diagnostic data, or application data sharing.

The following illustration shows Azure Files being used to share data between two geographical locations. Azure Files uses the Server Message Block (SMB) protocol that ensures the data is encrypted at rest and in transit.

![An illustration showing the file sharing capabilities of Azure Files. ](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/3-azure_files.png)

![Azure Queue](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/3-azure-queue.png)

**Azure Queue**

Azure Queue storage is a service for storing large numbers of messages that can be accessed from anywhere in the world.

Azure Queue Storage can be used to help build flexible applications and separate functions for better durability across large workloads. When application components are decoupled, they can scale independently. Queue storage provides asynchronous message queueing for communication between application components, whether they are running in the cloud, on the desktop, on-premises, or on mobile devices.

Typically, there are one or more sender components and one or more receiver components. Sender components add messages to the queue, while receiver components retrieve messages from the front of the queue for processing. The following illustration shows multiple sender applications adding messages to the Azure Queue and one receiver application retrieving the messages.

![An illustration showing a high-level architecture of Azure Queue storage](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/3-azure_queue.png)

You can use queue storage to:

- Create a backlog of work and to pass messages between different Azure web servers.
- Distribute load among different web servers/infrastructure and to manage bursts of traffic.
- Build resilience against component failure when multiple users access your data at the same time.

![Disk Storage](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/3-azure-standard-storage.png)

**Disk Storage**

Disk storage provides disks for virtual machines, applications, and other services to access and use as they need, similar to how they would in on-premises scenarios. Disk storage allows data to be persistently stored and accessed from an attached virtual hard disk. The disks can be managed or unmanaged by Azure, and therefore managed and configured by the user. Typical scenarios for using disk storage are if you want to lift and shift applications that read and write data to persistent disks, or if you are storing data that is not required to be accessed from outside the virtual machine to which the disk is attached.

Disks come in many different sizes and performance levels, from solid-state drives (SSDs) to traditional spinning hard disk drives (HDDs), with varying performance abilities.

When working with VMs, you can use standard SSD and HDD disks for less critical workloads, and premium SSD disks for mission-critical production applications. Azure Disks have consistently delivered enterprise-grade durability, with an industry-leading ZERO% annualized failure rate. The following illustration shows an Azure virtual machine using separate disks to store different data.

![An illustration showing two disks inside a virtual machine, one that stores the operating system and one that stores data.](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/3-azure_disks.png)

![Storage tiers](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/3-storage-tiers.png)

**Storage tiers**

Azure offers three storage tiers for blob object storage:

1. **Hot storage tier**: optimized for storing data that is accessed frequently.
2. **Cool storage tier**: optimized for data that is infrequently accessed and stored for at least 30 days.
3. **Archive storage tier**: for data that is rarely accessed and stored for at least 180 days with flexible latency requirements.

![Encryption and replication](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/3-azure-storage-encryption.png)

**Encryption and replication**

Azure provides security and high availability to your data through encryption and replication features.

#### Encryption for storage services

The following encryption types are available for your resources:

1. **Azure Storage Service Encryption (SSE)** for data at rest helps you secure your data to meet the organization's security and regulatory compliance. It encrypts the data before storing it and decrypts the data before retrieving it. The encryption and decryption are transparent to the user.
2. **Client-side encryption** is where the data is already encrypted by the client libraries. Azure stores the data in the encrypted state at rest, which is then decrypted during retrieval.

#### Replication for storage availability

A replication type is set up when you create a storage account. The replication feature ensures that your data is durable and always available. Azure provides regional and geographic replications to protect your data against natural disasters and other local disasters like fire or flooding.

------

## Next unit: Comparison between Azure data storage and on-premises storage

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/4-comparison-azure-and-on-prem-storage)










# Comparison between Azure data storage and on-premises storage

- 4 minutes

Now that you know about the benefits and features of Azure data storage, let's see how it differs from on-premises storage.

The term "on-premises" refers to the storage and maintenance of data on local hardware and servers. There are several factors to consider when comparing on-premises to Azure data storage.

![Paper bill and a cloud representing cost effectiveness](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/4-cost-effectiveness.png)

**Cost effectiveness**

An on-premises storage solution requires dedicated hardware that needs to be purchased, installed, configured, and maintained. This can be a significant up-front expense (or capital cost). Change in requirements can require investment in new hardware. Your hardware needs to be capable of handling peak demand which means it may sit idle or be under-utilized in off-peak times.

Azure data storage provides a pay-as-you-go pricing model which is often appealing to businesses as an operating expense instead of an upfront capital cost. It's also scalable, allowing you to scale up or scale out as demand dictates and scale back when demand is low. You are charged for data services only as you need them.

![A certificate representing reliability](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/4-reliability.png)

**Reliability**

On-premises storage requires data backup, load balancing, and disaster recovery strategies. These can be challenging and expensive as they often each need dedicated servers requiring a significant investment in both hardware and IT resources.

Azure data storage provides data backup, load balancing, disaster recovery, and data replication as services to ensure data safety and high availability.

![A uniquely shaped building representing different storage types](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/4-storage-types.png)

**Storage types**

Sometimes multiple different storage types are required for a solution, such as file and database storage. An on-premises approach often requires numerous servers and administrative tools for each storage type.

Azure data storage provides a variety of different storage options including distributed access and tiered storage. This makes it possible to integrate a combination of storage technologies providing the best storage choice for each part of your solution.

![A sports playbook representing agility](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/4-agility.png)

**Agility**

Requirements and technologies change. For an on-premises deployment this may mean provisioning and deploying new servers and infrastructure pieces, which is a time consuming and expensive activity.

Azure data storage gives you the flexibility to create new services in minutes. This flexibility allows you to change storage back-ends quickly without needing a significant hardware investment.

The following illustration shows differences between on-premises storage and Azure data storage.

![An illustration showing comparison between on-premises storage and Azure data storage for several common business needs.](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/media/4-comparison.png)

------

## Next unit: Knowledge check

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/5-knowledge-check)









# PART 8: Core Cloud Services - Azure networking options

# Introduction

- 1 minute

You just started working at startup that's fundamentally disrupting the vitamin industry with simple customization and affordable monthly subscriptions. While business is booming on the e-commerce site, your data center is starting to struggle to keep up with user demand. Your service fails when too many users login at the same time, and you're facing more scheduled and unscheduled maintenance windows than you'd like.

![An overloaded server in your data center](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/1-heading.png)

Your site is based in Silicon Valley, so you also find that a network delay is especially bad for users located in other regions, such as Europe and Asia.

Therefore, you convince your team to move the site to the cloud to help save costs. But how can Azure, specifically, help your site run better?

As it turns out, managing networks on Azure isn't entirely different from managing on-premises networks. Let's discover why.

## Learning objectives

In this module, you will learn:

- How an Azure virtual network provides secure network communication among resources such as virtual machines and other networks
- What high availability and resiliency mean and how Azure Load Balancer can increase resiliency within a single geographic region
- What latency is and how Traffic Manager helps reduce network latency and provides resiliency across geographic locations

------

## Next unit: Deploy your site to Azure

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/2-deploy-to-azure)











# Deploy your site to Azure

- 12 minutes

Your first step will likely be to re-create your on-premises configuration in the cloud.

This basic configuration will give you a sense of how networks are configured, and how network traffic moves in and out of Azure.

## Your e-commerce site at a glance

Larger enterprise systems are often composed of multiple inter-connected applications and services that work together. You might have a front-end web system that displays inventory and allows customers to create an order. That might talk to a variety of web services to provide the inventory data, manage user profiles, process credit cards, and request fulfillment of processed orders.

There are several strategies and patterns employed by software architects and designers to make these complex systems easier to design, build, manage, and maintain. Let's look at a few of them, starting with *loosely coupled architectures*.

### Benefits of Loosely Coupled Architectures

<iframe id="RE2yHrc-ax-4-id-oneplayer" src="https://www.microsoft.com/en-us/videoplayer/embed/RE2yHrc?pid=RE2yHrc-ax-4-id-oneplayer&amp;jsapi=true&amp;postJsllMsg=true&amp;autoplay=false&amp;mute=false&amp;loop=false&amp;market=en-us&amp;playFullScreen=false" class="oneplayer-iframe" allowfullscreen="true" frameborder="0" name="Oneplayer iframe" title="Video: RE2yHrc" style="width: 640px; box-sizing: inherit; position: absolute; top: 0px; left: 0px; right: 0px; bottom: 0px; height: 360px;"></iframe>

### Using an N-tier architecture

An architectural pattern that can be used to build loosely coupled systems is *N-tier*.

An [N-tier architecture](https://docs.microsoft.com/azure/architecture/guide/architecture-styles/n-tier) divides an application into two or more logical tiers. Architecturally, a higher tier can access services from a lower tier, but a lower tier should never access a higher tier.

Tiers help separate concerns and are ideally designed to be reusable. Using a tiered architecture also simplifies maintenance. Tiers can be updated or replaced independently, and new tiers can be inserted if needed.

*Three-tier* refers to an n-tier application that has three tiers. Your e-commerce web application follows this three-tier architecture:

- The **web tier** provides the web interface to your users through a browser.
- The **application tier** runs business logic.
- The **data tier** includes databases and other storage that hold product information and customer orders.

The following illustration shows the flow of a request from the user to the data tier.

![An illustration showing a three-tier architecture where each tier is hosted in a dedicated virtual machine.](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/2-three-tier.png)

When the user clicks the button to place the order, the request is sent to the web tier, along with the user's address and payment information. The web tier passes this information to the application tier, which would validate payment information and check inventory. The application tier might then store the order in the data tier, to be picked up later for fulfillment.

## Your e-commerce site running on Azure

Azure provides many different ways to host your web applications, from fully pre-configured environments that host your code, to virtual machines that you configure, customize, and manage.

Let's say you choose to run your e-commerce site on virtual machines. Here's what that might look like in your test environment running on Azure. The following illustration shows a three-tier architecture running on virtual machines with security features enabled to restrict inbound requests.

![An illustration showing a three-tier architecture where each tier is running on a separate virtual machine. Each virtual machine is labeled with its IP address and is inside its own virtual network. Each virtual network has a network security group that lists the open ports.](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/2-test-deployment.png)

Let's break this down.

![A pinned location on the Earth representing an Azure region](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/2-azure-region.png)

**What's an Azure region?**

A *region* is one or more Azure data centers within a specific geographic location. East US, West US, and North Europe are examples of regions. In this instance, you see that the application is running in the East US region.

![Two virtual machines running on a virtual network](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/2-azure-vnet.png)

**What's a virtual network?**

A *virtual network* is a logically isolated network on Azure. Azure virtual networks will be familiar to you if you've set up networks on Hyper-V, VMware, or even on other public clouds. A virtual network allows Azure resources to securely communicate with each other, the internet, and on-premises networks. A virtual network is scoped to a single region; however, multiple virtual networks from different regions can be connected together using virtual network peering.

Virtual networks can be segmented into one or more *subnets*. Subnets help you organize and secure your resources in discrete sections. The web, application, and data tiers each have a single VM. All three VMs are in the same virtual network but are in separate subnets.

Users interact with the web tier directly, so that VM has a public IP address along with a private IP address. Users don't interact with the application or data tiers, so these VMs each have a private IP address only.

You can also keep your service or data tiers in your on-premises network, placing your web tier into the cloud, but keeping tight control over other aspects of your application. A *VPN gateway* (or virtual network gateway), enables this scenario. It can provide a secure connection between an Azure Virtual Network and an on-premises location over the internet.

Azure manages the physical hardware for you. You configure virtual networks and gateways through software, which enables you to treat a virtual network just like your own network. You choose which networks your virtual network can reach, whether that's the public internet or other networks in the private IP address space.

![Two virtual machines with a shared network security group](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/2-azure-nsg.png)

**What's a network security group?**

A *network security group*, or NSG, allows or denies inbound network traffic to your Azure resources. Think of a network security group as a cloud-level firewall for your network.

For example, notice that the VM in the web tier allows inbound traffic on ports 22 (SSH) and 80 (HTTP). This VM's network security group allows inbound traffic over these ports from all sources. You can configure a network security group to accept traffic only from known sources, such as IP addresses that you trust.

 Note

Port 22 enables you to connect directly to Linux systems over SSH. Here we show port 22 open for learning purposes. In practice, you might configure VPN access to your virtual network to increase security.

## Summary

Your three-tier application is now running on Azure in the East US region. A *region* is an Azure data center within a specific geographic location.

Each tier can access services only from a lower tier. The VM running in the web tier has a public IP address because it receives traffic from the internet. The VMs in the lower tiers, the application and data tiers, each have private IP addresses because they don't communicate directly over the internet.

*Virtual networks* enable you to group and isolate related systems. You define *network security groups* to control what traffic can flow through a virtual network.

The configuration you saw here is a good start. But when you deploy your e-commerce site to production in the cloud, you'll likely run into the same problems as you did in your on-premises deployment.

## Check your knowledge

\1. 

What is an Azure *region*?



One or more Azure data centers within a specific geographical location.



A way of breaking networks into smaller networks.



Firewall rules which define the flow of traffic in and out of Azure.

\2. 

Which of the following is true about virtual networks?



You configure virtual networks through software.



A virtual network accepts network traffic on all ports. You configure the firewall through virtual machines.



Virtual networks are always reachable from the internet.



------

## Next unit: Scale with Azure Load Balancer

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/3-scale-load-balancer)









# Scale with Azure Load Balancer

- 7 minutes

You now have your site up and running on Azure. But how can you help ensure your site is running 24/7?

For instance, what happens when you need to do weekly maintenance? Your service will still be unavailable during your maintenance window. And because your site reaches users all over the world, there's no good time to take down your systems for maintenance. You may also run into performance issues if too many users connect at the same time.

## What are availability and high availability?

![A speed train representing high availability](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/3-availability.png)

*Availability* refers to how long your service is up and running without interruption. *High availability*, or *highly available*, refers to a service that's up and running for a long period of time.

You know how frustrating it is when you can't access the information you need. Think of a social media or news site that you visit daily. Can you always access the site, or do you often see error messages like "503 Service Unavailable"?

You may have heard terms like "five nines availability." Five nines availability means that the service is guaranteed to be running 99.999 percent of the time. Although it's difficult to achieve 100 percent availability, many teams strive for at least five nines.

## What is resiliency?

![A health chart representing resiliency](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/3-resiliency.png)

*Resiliency* refers to a system's ability to stay operational during abnormal conditions.

These conditions include:

- Natural disasters
- System maintenance, both planned and unplanned, including software updates and security patches.
- Spikes in traffic to your site
- Threats made by malicious parties, such as distributed denial of service, or DDoS, attacks

Imagine your marketing team wants to have a flash sale to promote a new line of vitamin supplements. You might expect a huge spike in traffic during this time. This spike could overwhelm your processing system, causing it to slow down or halt, disappointing your users. You may have experienced this disappointment for yourself. Have you ever tried to access an online sale only to find the website wasn't responding?

## What is a load balancer?

![A scale representing load balancing](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/3-lb.png)

A *load balancer* distributes traffic evenly among each system in a pool. A load balancer can help you achieve both high availability and resiliency.

Say you start by adding additional VMs, each configured identically, to each tier. The idea is to have additional systems ready, in case one goes down, or is serving too many users at the same time.

The problem here is that each VM would have its own IP address. Plus, you don't have a way to distribute traffic in case one system goes down or is busy. How do you connect your VMs so that they appear to the user as one system?

The answer is to use a *load balancer* to distribute traffic. The load balancer becomes the entry point to the user. The user doesn't know (or need to know) which system the load balancer chooses to receive the request.

The following illustration shows the role of a load balancer.

![An illustration showing the web tier of a three-tier architecture. The web tier has multiple virtual machines to service user requests. There is a load balancer that distributes user requests among the virtual machines.](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/3-load-balancer.png)

The load balancer receives the user's request and directs the request to one of the VMs in the web tier. If a VM is unavailable or stops responding, the load balancer stops sending traffic to it. The load balancer then directs traffic to one of the responsive servers.

Load balancing enables you to run maintenance tasks without interrupting service. For example, you can stagger the maintenance window for each VM. During the maintenance window, the load balancer detects that the VM is unresponsive, and directs traffic to other VMs in the pool.

For your e-commerce site, the app and data tiers can also have a load balancer. It all depends on what your service requires.

## What is Azure Load Balancer?

Azure Load Balancer is a load balancer service that Microsoft provides that helps take care of the maintenance for you. Load Balancer supports inbound and outbound scenarios, provides low latency and high throughput, and scales up to millions of flows for all Transmission Control Protocol (TCP) and User Datagram Protocol (UDP) applications. You can use Load Balancer with incoming internet traffic, internal traffic across Azure services, port forwarding for specific traffic, or outbound connectivity for VMs in your virtual network.

When you manually configure typical load balancer software on a virtual machine, there's a downside: you now have an additional system that you need to maintain. If your load balancer goes down or needs routine maintenance, you're back to your original problem.

If instead, however, you use Azure Load Balancer, there's no infrastructure or software for you to maintain. You define the forwarding rules based on the source IP and port to a set of destination IP/ports.

The following illustration shows the role of Azure load balancers in a multi-tier architecture.

![An illustration showing the web tier of a three-tier architecture. The web tier has multiple virtual machines to service user requests. There is a load balancer that distributes user requests among the virtual machines.](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/3-azure-load-balancer.png)

## Azure Application Gateway

If all your traffic is HTTP, a potentially better option is to use Azure Application Gateway. Application Gateway is a load balancer designed for web applications. It uses Azure Load Balancer at the transport level (TCP) and applies sophisticated URL-based routing rules to support several advanced scenarios.

![Conceptual image showing the Application Gateway product routing HTTP traffic between server groups based on the URL](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/3-appgateway.png)

This type of routing is known as application layer (OSI layer 7) load balancing since it understands the structure of the HTTP message.

Here are some of the benefits of using Azure Application Gateway over a simple load balancer:

- **Cookie affinity**. Useful when you want to keep a user session on the same backend server.
- **SSL termination**. Application Gateway can manage your SSL certificates and pass unencrypted traffic to the backend servers to avoid encryption/decryption overhead. It also supports full end-to-end encryption for applications that require that.
- **Web application firewall**. Application gateway supports a sophisticated firewall (WAF) with detailed monitoring and logging to detect malicious attacks against your network infrastructure.
- **URL rule-based routes**. Application Gateway allows you to route traffic based on URL patterns, source IP address and port to destination IP address and port. This is helpful when setting up a *content delivery network*.
- **Rewrite HTTP headers**. You can add or remove information from the inbound and outbound HTTP headers of each request to enable important security scenarios, or scrub sensitive information such as server names.

### What is a Content Delivery Network?

A content delivery network (CDN) is a distributed network of servers that can efficiently deliver web content to users. It is a way to get content to users in their local region to minimize latency. CDN can be hosted in Azure or any other location. You can cache content at strategically placed physical nodes across the world and provide better performance to end users. Typical usage scenarios include web applications containing multimedia content, a product launch event in a particular region, or any event where you expect a high-bandwidth requirement in a region.

## What about DNS?

![A pin on a map representing DNS](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/3-map-pin.png)

DNS, or Domain Name System, is a way to map user-friendly names to their IP addresses. You can think of DNS as the phonebook of the internet.

For example, your domain name, contoso.com, might map to the IP address of the load balancer at the web tier, 40.65.106.192.

You can bring your own DNS server or use Azure DNS, a hosting service for DNS domains that runs on Azure infrastructure.

The following illustration shows Azure DNS. When the user navigates to **contoso.com**, Azure DNS routes traffic to the load balancer.

![An illustration showing the Azure domain name system positioned in front of the load balancer.](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/3-dns.png)

## Summary

With load balancing in place, your e-commerce site is now more highly available and resilient. When you perform maintenance or receive an uptick in traffic, your load balancer can distribute traffic to another available system.

Although you can configure your own load balancer on a VM, Azure Load Balancer reduces upkeep because there's no infrastructure or software to maintain.

DNS maps user-friendly names to their IP addresses, much like how a phonebook maps names of people or businesses to phone numbers. You can bring your own DNS server, or use Azure DNS.

## Check your knowledge

\1. 

Which is true about Azure Load Balancer?



You must use Azure Load Balancer if you want to distribute traffic among your virtual machines running in Azure.



Azure Load Balancer works with internet-facing traffic only.



Azure Load Balancer distributes traffic among similar systems, making your services more highly available.










# Reduce latency with Azure Traffic Manager

- 7 minutes

Previously, you saw how **Azure Load Balancer** helps you achieve high availability and minimize downtime.

Although your e-commerce site is more highly available, it doesn't solve the issue of latency or create resiliency across geographic regions.

How can you make your site, which is located in the United States, load faster for users located in Europe or Asia?

## What is network latency?

![A stopwatch representing latency](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/4-latency.png)

*Latency* refers to the time it takes for data to travel over the network. Latency is typically measured in milliseconds.

Compare latency to bandwidth. Bandwidth refers to the amount of data that can fit on the connection. Latency refers to the time it takes for that data to reach its destination.

Factors such as the type of connection you use and how your application is designed can affect latency. But perhaps the biggest factor is distance.

Think about your e-commerce site on Azure, which is in the East US region. It would typically take less time to transfer data to Atlanta (a distance of around 400 miles) than to transfer data to London (a distance of around 4,000 miles).

Your e-commerce site delivers standard HTML, CSS, JavaScript, and images. The network latency for many files can add up. How can you reduce latency for users located far away geographically?

## Scale out to different regions

Recall that Azure provides data centers in regions across the globe.

![A globe representing region scale-out](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/4-scale-out-regions.png)

Think about the cost of building a data center. Equipment costs aren't the only factor. You need to provide the power, cooling, and personnel to keep your systems running at each location. It might be prohibitively expensive to replicate your entire data center. But doing so with Azure can cost much less, because Azure already has the equipment and personnel in place.

One way to reduce latency is to provide exact copies of your service in more than one region. The following illustration shows an example of global deployment.

![An illustration showing a world map with three Azure data centers highlighted. Each data center is labelled with a unique domain name.](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/4-global-deployment.png)

The diagram shows your e-commerce site running in three Azure regions: East US, North Europe, and East Asia. Notice the DNS name for each. How can you connect users to the service that's closest geographically, but under the contoso.com domain?

## Use Traffic Manager to route users to the closest endpoint

![A sign post representing Azure Traffic Manager](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/4-sign-post.png)

One answer is **Azure Traffic Manager**. Traffic Manager uses the DNS server that's closest to the user to direct user traffic to a globally distributed endpoint.

The following illustration shows the role of the Traffic Manager.

![An illustration showing Azure Traffic Manager routing a user request to the nearest data center. ](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/4-traffic-manager.png)

Traffic Manager doesn't see the traffic that's passed between the client and server. Rather, it directs the client web browser to a preferred endpoint. Traffic Manager can route traffic in a few different ways, such as to the endpoint with the lowest latency.

Although not shown here, this setup could also include your on-premises deployment running in California. You can connect Traffic Manager to your own on-premises networks, enabling you to maintain your existing data center investments. Or you can move your application entirely to the cloud. The choice is yours.

## Compare Load Balancer to Traffic Manager

![A magnifying glass](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/4-magnifying-glass.png)

Azure Load Balancer distributes traffic within the same region to make your services more highly available and resilient. Traffic Manager works at the DNS level, and directs the client to a preferred endpoint. This endpoint can be to the region that's closest to your user.

Load Balancer and Traffic Manager both help make your services more resilient, but in slightly different ways. When Load Balancer detects an unresponsive VM, it directs traffic to other VMs in the pool. Traffic Manager monitors the health of your endpoints. In contrast, when Traffic Manager finds an unresponsive endpoint, it directs traffic to the next closest endpoint that is responsive.

## Summary

Geographic distance is one of the biggest factors that contributes to latency. With Traffic Manager in place, you can host exact copies of your service in multiple geographic regions. That way, users in the United States, Europe, and Asia will all have a good experience using your e-commerce site.

## Check your knowledge

\1. 

What is network latency?



The amount of data that can fit on the connection.



The distance data must travel to reach its destination.



The time it takes for data to travel over the network.

\2. 

How does Azure Traffic Manager reduce latency?



It chooses only the fastest networks between endpoints.



It chooses the endpoint that's closest to the user's DNS server.



It caches content, similar to how content delivery networks work.









# Summary

- 1 minute

You learned just a few ways Azure networking can help reduce latency and make your apps and services more highly available.

![Load balanced servers running in Azure](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-networking/media/5-heading.png)

With load balancing and global distribution in place, your e-commerce site is ready for the world. Users reach the domain that's closest geographically. Each domain has failover built in, helping every user have a great experience. The numbers are already showing increased traffic, and business is booming.

------

## Module complete:











# PART 9: Security, responsibility and trust in Azure

# Introduction

- 3 minutes

Every system, architecture, and application needs to be designed with security in mind. There's just too much at risk. For instance, a denial of service attack could prevent your customer from reaching your web site or services and block you from doing business. Defacement of your website damages your reputation. And a data breach is perhaps worst of all — as it can ruin hard-earned trust, while causing significant personal and financial harm. As administrators, developers, and IT management, we all must work to guarantee the security of our systems.

Let's say you work at a company called Contoso Shipping, and you're spearheading the development of drone deliveries in rural areas—while having truck drivers leverage mobile apps to deliver to urban areas. You're in the process of moving a lot of Contoso Shipping's infrastructure to the cloud to maximize efficiency, as well as moving several physical servers in the company's data center to Azure virtual machines. Your team plans on creating a hybrid solution, with some of the servers remaining on-premises, so you'll need a secure, high-quality connection between the new virtual machines and the existing network.

![An illustration demonstrating the concept of security with a shield placed between on-premises and cloud networks.](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/1-heading.png)

Additionally, Contoso Shipping has some out-of-network devices that are part of your operations. You are using network-enabled sensors in your drones that send data to Azure Event Hubs, while delivery drivers use mobile apps to get route maps and record signatures for receipt of shipments. These devices and apps must be securely authenticated before data can be sent to or from them.

So how do you keep your data secure?

## Learning objectives

In this module, you will learn how:

- Security responsibility is shared with Azure
- Identity management provides protection, even outside your network
- Encryption capabilities built into Azure can protect your data
- To protect your network and virtual networks

## Prerequisites

None

------

## Next unit: Cloud security is a shared responsibility

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/2-shared-responsibility)









# Cloud security is a shared responsibility

- 11 minutes

As computing environments move from customer-controlled data centers to cloud data centers, the responsibility of security also shifts. Security is now a concern shared both by cloud providers and customers. For every application and solution, it's important to understand what's your responsibility and what's Azure's responsibility.

#### Understand security threats

<iframe id="RWkotg-ax-2-id-oneplayer" src="https://www.microsoft.com/en-us/videoplayer/embed/RWkotg?pid=RWkotg-ax-2-id-oneplayer&amp;jsapi=true&amp;postJsllMsg=true&amp;autoplay=false&amp;mute=false&amp;loop=false&amp;market=en-us&amp;playFullScreen=false" class="oneplayer-iframe" allowfullscreen="true" frameborder="0" name="Oneplayer iframe" title="Video: RE2yEvj" style="width: 640px; box-sizing: inherit; position: absolute; top: 0px; left: 0px; right: 0px; bottom: 0px; height: 360px;"></iframe>

#### Azure security: you versus the cloud

<iframe id="RE2yEvj-ax-3-id-oneplayer" src="https://www.microsoft.com/en-us/videoplayer/embed/RE2yEvj?pid=RE2yEvj-ax-3-id-oneplayer&amp;jsapi=true&amp;postJsllMsg=true&amp;autoplay=false&amp;mute=false&amp;loop=false&amp;market=en-us&amp;playFullScreen=false" class="oneplayer-iframe" allowfullscreen="true" frameborder="0" name="Oneplayer iframe" style="width: 640px; box-sizing: inherit; position: absolute; top: 0px; left: 0px; right: 0px; bottom: 0px; height: 360px;"></iframe>

## Share security responsibility with Azure

The first shift you’ll make is from on-premises data centers to infrastructure as a service (IaaS). With IaaS, you are leveraging the lowest-level service and asking Azure to create virtual machines (VMs) and virtual networks. At this level, it's still your responsibility to patch and secure your operating systems and software, as well as configure your network to be secure. At Contoso Shipping, you are taking advantage of IaaS when you start using Azure VMs instead of your on-premises physical servers. In addition to the operational advantages, you receive the security advantage of having outsourced concern over protecting the physical parts of the network.

Moving to platform as a service (PaaS) outsources a lot of security concerns. At this level, Azure is taking care of the operating system and of most foundational software like database management systems. Everything is updated with the latest security patches and can be integrated with Azure Active Directory for access controls. PaaS also comes with a lot of operational advantages. Rather than building whole infrastructures and subnets for your environments by hand, you can "point and click" within the Azure portal or run automated scripts to bring complex, secured systems up and down, and scale them as needed. Contoso Shipping uses Azure Event Hubs for ingesting telemetry data from drones and trucks — as well as a web app with an Azure Cosmos DB back end with its mobile apps — which are all examples of PaaS.

With software as a service (SaaS), you outsource almost everything. SaaS is software that runs with an internet infrastructure. The code is controlled by the vendor but configured to be used by the customer. Like so many companies, Contoso Shipping uses Office 365, which is a great example of SaaS!

![An illustration showing how cloud providers and customers share security responsibilities under different types of compute service implementation: on-premises, infrastructure as a service, platform as a service, and software as a service.](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/shared_responsibilities.png)

## A layered approach to security

*Defense in depth* is a strategy that employs a series of mechanisms to slow the advance of an attack aimed at acquiring unauthorized access to information. Each layer provides protection so that if one layer is breached, a subsequent layer is already in place to prevent further exposure. Microsoft applies a layered approach to security, both in physical data centers and across Azure services. The objective of defense in depth is to protect and prevent information from being stolen by individuals who are not authorized to access it.

Defense in depth can be visualized as a set of concentric rings, with the data to be secured at the center. Each ring adds an additional layer of security around the data. This approach removes reliance on any single layer of protection and acts to slow down an attack and provide alert telemetry that can be acted upon, either automatically or manually. Let's take a look at each of the layers.

![An illustration showing Defense in depth with Data at the center. The rings of security around data are: application, compute, network, perimeter, identity and access, and physical security.](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/defense_in_depth_layers_small.png)

![Image representing data](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/2-data.png)

**Data**

In almost all cases, attackers are after data:

- Stored in a database
- Stored on disk inside virtual machines
- Stored on a SaaS application such as Office 365
- Stored in cloud storage

It's the responsibility of those storing and controlling access to data to ensure that it's properly secured. Often, there are regulatory requirements that dictate the controls and processes that must be in place to ensure the confidentiality, integrity, and availability of the data.

![Image of a file on the network](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/2-application.png)

**Application**

- Ensure applications are secure and free of vulnerabilities.
- Store sensitive application secrets in a secure storage medium.
- Make security a design requirement for all application development.

Integrating security into the application development life cycle will help reduce the number of vulnerabilities introduced in code. We encourage all development teams to ensure their applications are secure by default, and that they're making security requirements non-negotiable.

![A terminal representing compute](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/2-compute.png)

**Compute**

- Secure access to virtual machines.
- Implement endpoint protection and keep systems patched and current.

Malware, unpatched systems, and improperly secured systems open your environment to attacks. The focus in this layer is on making sure your compute resources are secure, and that you have the proper controls in place to minimize security issues.

![Three connected systems representing networking](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/2-networking.png)

**Networking**

- Limit communication between resources.
- Deny by default.
- Restrict inbound internet access and limit outbound, where appropriate.
- Implement secure connectivity to on-premises networks.

At this layer, the focus is on limiting the network connectivity across all your resources to allow only what is required. By limiting this communication, you reduce the risk of lateral movement throughout your network.

![A physical barrier representing the network perimeter](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/2-perimeter.png)

**Perimeter**

- Use distributed denial of service (DDoS) protection to filter large-scale attacks before they can cause a denial of service for end users.
- Use perimeter firewalls to identify and alert on malicious attacks against your network.

At the network perimeter, it's about protecting from network-based attacks against your resources. Identifying these attacks, eliminating their impact, and alerting you when they happen are important ways to keep your network secure.

![A badge representing a secure access](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/2-policies-and-access.png)

**Identity and access**

- Control access to infrastructure and change control.
- Use single sign-on and multi-factor authentication.
- Audit events and changes.

The identity and access layer is all about ensuring identities are secure, access granted is only what is needed, and changes are logged.

![A security camera representing physical security](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/2-physical-security.png)

**Physical security**

- Physical building security and controlling access to computing hardware within the data center is the first line of defense.

With physical security, the intent is to provide physical safeguards against access to assets. This ensures that other layers can't be bypassed, and loss or theft is handled appropriately.

## Summary

We've seen here that Azure helps a lot with your security concerns. But security is still a **shared responsibility**. How much of that responsibility falls on us depends on which model we use with Azure.

We use the *defense in depth* rings as a guideline for considering what protections are adequate for our data and environments.

------

## Next unit: Get tips from Azure Security Center

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/2a-azure-security-center)









# Get tips from Azure Security Center

- 10 minutes

A great place to start when examining the security of your Azure-based solutions is **Azure Security Center**. Security Center is a monitoring service that provides threat protection across all of your services both in Azure, and on-premises. Security Center can:

- Provide security recommendations based on your configurations, resources, and networks.
- Monitor security settings across on-premises and cloud workloads, and automatically apply required security to new services as they come online.
- Continuously monitor all your services, and perform automatic security assessments to identify potential vulnerabilities before they can be exploited.
- Use machine learning to detect and block malware from being installed on your virtual machines and services. You can also define a list of allowed applications to ensure that only the apps you validate are allowed to execute.
- Analyze and identify potential inbound attacks, and help to investigate threats and any post-breach activity that might have occurred.
- Provide just-in-time access control for ports, reducing your attack surface by ensuring the network only allows traffic that you require.

Azure Security Center is part of the [Center for Internet Security (CIS) recommendations](https://www.cisecurity.org/cis-benchmarks/).

![Image representing Azure Security Center](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/2a-securitycenter.png)

## Available tiers

Azure Security Center is available in two tiers:

1. *Free*. Available as part of your Azure subscription, this tier is limited to assessments and recommendations of Azure resources only.
2. *Standard*. This tier provides a full suite of security-related services including continuous monitoring, threat detection, just-in-time access control for ports, and more.

To access the full suite of Azure Security Center services, you will need to upgrade to a Standard tier subscription. You can access the 60-day free trial from within the Azure Security Center dashboard in the Azure portal. After the 60-day trial period is over, Azure Security Center is $15 per node per month.

## Usage scenarios

You can integrate Security Center into your workflows and use it in many ways. Here are two examples.

1. Use Security Center for incident response.

   Many organizations learn how to respond to security incidents only after suffering an attack. To reduce costs and damage, it’s important to have an incident response plan in place before an attack occurs. You can use Azure Security Center in different stages of an incident response.

   ![Circular arrows point from the words detect, to assess, to diagnose, to stabilize, to close](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/2a-security-center-incident-response.png)

   You can use Security Center during the detect, assess, and diagnose stages. Here are examples of how Security Center can be useful during the three initial incident response stages:

   - *Detect*. Review the first indication of an event investigation. For example, you can use the Security Center dashboard to review the initial verification that a high-priority security alert was raised.
   - *Assess*. Perform the initial assessment to obtain more information about the suspicious activity. For example, obtain more information about the security alert.
   - *Diagnose*. Conduct a technical investigation and identify containment, mitigation, and workaround strategies. For example, follow the remediation steps described by Security Center in that particular security alert.

2. Use Security Center recommendations to enhance security.

   You can reduce the chances of a significant security event by configuring a security policy, and then implementing the recommendations provided by Azure Security Center.

   - A *security policy* defines the set of controls that are recommended for resources within that specified subscription or resource group. In Security Center, you define policies according to your company's security requirements.
   - Security Center analyzes the security state of your Azure resources. When Security Center identifies potential security vulnerabilities, it creates recommendations based on the controls set in the security policy. The recommendations guide you through the process of configuring the needed security controls. For example, if you have workloads that do not require the *Azure SQL Database Transparent Data Encryption* (TDE) policy, turn off the policy at the subscription level and enable it only in the resources groups where SQL TDE is required.

 Important

To upgrade a subscription to the Standard tier, you must be assigned the role of *Subscription Owner*, *Subscription Contributor*, or *Security Admin*.

------

## Next unit: Identity and access

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/3-identity-and-access)


  





# Identity and access

- 10 minutes

Network perimeters, firewalls, and physical access controls used to be the primary protection for corporate data. But network perimeters have become increasingly porous with the explosion of bring your own device (BYOD), mobile apps, and cloud applications.

Identity has become the new primary security boundary. Therefore, proper authentication and assignment of privileges is critical to maintaining control of your data.

Your company, Contoso Shipping, is focused on addressing these concerns right away. Your team's new hybrid cloud solution needs to account for mobile apps that have access to secret data when an authorized user is signed in — in addition to having shipping vehicles constantly send a stream of telemetry data that is critical to optimizing the company's business.

## Authentication and authorization

Two fundamental concepts that need to be understood when talking about identity and access control are authentication and authorization. They underpin everything else that happens and occur sequentially in any identity and access process:

- *Authentication* is the process of establishing the identity of a person or service looking to access a resource. It involves the act of challenging a party for legitimate credentials, and provides the basis for creating a security principal for identity and access control use. It establishes if they are who they say they are.
- *Authorization* is the process of establishing what level of access an authenticated person or service has. It specifies what data they're allowed to access and what they can do with it.

 Note

Authentication is sometimes shortened to *AuthN*, and authorization is sometimes shortened to *AuthZ*.

Azure provides services to manage both authentication and authorization through Azure Active Directory (Azure AD).

## What is Azure Active Directory?

Azure AD is a cloud-based identity service. It has built in support for synchronizing with your existing on-premises Active Directory or can be used stand-alone. This means that all your applications, whether on-premises, in the cloud (including Office 365), or even mobile can share the same credentials. Administrators and developers can control access to internal and external data and applications using centralized rules and policies configured in Azure AD.

Azure AD provides services such as:

- **Authentication.** This includes verifying identity to access applications and resources, and providing functionality such as self-service password reset, multi-factor authentication (MFA), a custom banned password list, and smart lockout services.
- **Single-Sign-On (SSO).** SSO enables users to remember only one ID and one password to access multiple applications. A single identity is tied to a user, simplifying the security model. As users change roles or leave an organization, access modifications are tied to that identity, greatly reducing the effort needed to change or disable accounts.
- **Application management.** You can manage your cloud and on-premises apps using Azure AD Application Proxy, SSO, the My apps portal (also referred to as Access panel), and SaaS apps.
- **Business to business (B2B) identity services.** Manage your guest users and external partners while maintaining control over your own corporate data Business-to-Customer (B2C) identity services. Customize and control how users sign up, sign in, and manage their profiles when using your apps with services.
- **Device Management.** Manage how your cloud or on-premises devices access your corporate data.

Let's explore of a few of these in more detail.

## Single sign-on

The more identities a user has to manage, the greater the risk of a credential-related security incident. More identities mean more passwords to remember and change. Password policies can vary between applications and, as complexity requirements increase, it becomes increasingly difficult for users to remember them.

Now, consider the logistics of managing all those identities. Additional strain is placed on help desks as they deal with account lockouts and password reset requests. If a user leaves an organization, tracking down all those identities and ensuring they are disabled can be challenging. If an identity is overlooked, this could allow access when it should have been eliminated.

With single sign-on (SSO), users need to remember only one ID and one password. Access across applications is granted to a single identity tied to a user, simplifying the security model. As users change roles or leave an organization, access modifications are tied to the single identity, greatly reducing the effort needed to change or disable accounts. Using single sign-on for accounts will make it easier for users to manage their identities and will increase the security capabilities in your environment.

![A thumbprint representing Azure Active Directory](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/3-sso-with-azure-ad.png)

**SSO with Azure Active Directory**

By leveraging Azure AD for SSO you'll also have the ability to combine multiple data sources into an intelligent security graph. This security graph enables the ability to provide threat analysis and real-time identity protection to all accounts in Azure AD, including accounts that are synchronized from your on-premises AD. By using a centralized identity provider, you'll have centralized the security controls, reporting, alerting, and administration of your identity infrastructure.

As Contoso Shipping integrates its existing Active Directory instance with Azure AD, you will make controlling access consistent across the organization. Doing so will also greatly simplify the ability to sign into email and Office 365 documents without having to reauthenticate.

## Multi-factor authentication

Multi-factor authentication (MFA) provides additional security for your identities by requiring two or more elements for full authentication. These elements fall into three categories:

- *Something you know*
- *Something you possess*
- *Something you are*

**Something you know** would be a password or the answer to a security question. **Something you possess** could be a mobile app that receives a notification or a token-generating device. **Something you are** is typically some sort of biometric property, such as a fingerprint or face scan used on many mobile devices.

Using MFA increases security of your identity by limiting the impact of credential exposure. An attacker who has a user's password would also need to have possession of their phone or their face in order to fully authenticate. Authentication with only a single factor verified is insufficient, and the attacker would be unable to use those credentials to authenticate. The benefits this brings to security are huge, and we can't emphasize enough the importance of enabling MFA wherever possible.

Azure AD has MFA capabilities built in and will integrate with other third-party MFA providers. It's provided free of charge to any user who has the Global Administrator role in Azure AD, because these are highly sensitive accounts. All other accounts can have MFA enabled by purchasing licenses with this capability — as well as assigning a license to the account.

For Contoso Shipping, you decide to enable MFA any time a user is signing in from a non-domain-connected computer — which includes the mobile apps your drivers use.

## Providing identities to services

It's usually valuable for services to have identities. Often, and against best practices, credential information is embedded in configuration files. With no security around these configuration files, anyone with access to the systems or repositories can access these credentials and risk exposure.

Azure AD addresses this problem through two methods: service principals and managed identities for Azure services.

![Image representing various roles](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/3-service-principals.png)

**Service principals**

To understand service principals, it's useful to first understand the words **identity** and **principal**, because of how they are used in the identity management world.

An **identity** is just a thing that can be authenticated. Obviously, this includes users with a user name and password, but it can also include applications or other servers, which might authenticate with secret keys or certificates. As a bonus definition, an **account** is data associated with an identity.

A **principal** is an identity acting with certain roles or claims. Usually, it is not useful to consider identity and principal separately, but think of using `sudo` on a Bash prompt in Linux or on Windows using "run as Administrator." In both those cases, you are still logged in as the same identity as before, but you've changed the role under which you are executing. Groups are often also considered principals because they can have rights assigned.

A **service principal** is an identity that is used by a service or application. And like other identities, it can be assigned roles.

![Image representing managed identities](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/3-managed-service-identities.png)

**Managed identities for Azure services**

The creation of service principals can be a tedious process, and there are a lot of touch points that can make maintaining them difficult. Managed identities for Azure services are much easier and will do most of the work for you.

A managed identity can be instantly created for any Azure service that supports it—and the list is constantly growing. When you create a managed identity for a service, you are creating an account on the Azure AD tenant. The Azure infrastructure will automatically take care of authenticating the service and managing the account. You can then use that account like any other Azure AD account, including securely letting the authenticated service access other Azure resources.

## Role-based access control

Roles are sets of permissions, like "Read-only" or "Contributor", that users can be granted to access an Azure service instance.

Identities are mapped to roles directly or through group membership. Separating security principals, access permissions, and resources provides simple access management and fine-grained control. Administrators are able to ensure the minimum necessary permissions are granted.

Roles can be granted at the individual service instance level, but they also flow down the Azure Resource Manager hierarchy.

Here's a diagram that shows this relationship. Roles assigned at a higher scope, like an entire subscription, are inherited by child scopes, like service instances.

![An illustration showing the hierarchal representation of role-based access in a management group.](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/3-role-assignment-scope.png)

### Privileged Identity Management

In addition to managing Azure resource access with role-based access control (RBAC), a comprehensive approach to infrastructure protection should consider including the ongoing auditing of role members as their organization changes and evolves. Azure AD Privileged Identity Management (PIM) is an additional, paid-for offering that provides oversight of role assignments, self-service, and just-in-time role activation and Azure AD and Azure resource access reviews.

![Screenshot of Privileged identity management dashboard](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/pim_dashboard.png)

## Summary

Identity allows us to maintain a security perimeter, even outside our physical control. With single sign-on and appropriate role-based access configuration, we can always be sure who has the ability to see and manipulate our data and infrastructure.

------

## Next unit: Encryption

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/4-encryption)


  





# Encryption

- 8 minutes

For most organizations, data is the most valuable and irreplaceable asset. Encryption serves as the last and strongest line of defense in a layered security strategy.

Contoso Shipping knows that encryption is the only protection its data has once it leaves the data center and is stored on mobile devices that could potentially be hacked or stolen.

## What is encryption?

Encryption is the process of making data unreadable and unusable to unauthorized viewers. To use or read the encrypted data, it must be *decrypted*, which requires the use of a secret key. There are two top-level types of encryption: **symmetric**and **asymmetric**.

**Symmetric encryption** uses the same key to encrypt and decrypt the data. Consider a desktop password manager application. You enter your passwords and they are encrypted with your own personal key (your key is often derived from your master password). When the data needs to be retrieved, the same key is used, and the data is decrypted.

**Asymmetric encryption** uses a public key and private key pair. Either key can encrypt but a single key can't decrypt its own encrypted data. To decrypt, you need the paired key. Asymmetric encryption is used for things like Transport Layer Security (TLS) (used in HTTPS) and data signing.

Both symmetric and asymmetric encryption play a role in properly securing your data. Encryption is typically approached in two ways:

1. Encryption at rest
2. Encryption in transit

## Encryption at rest

Data at rest is the data that has been stored on a physical medium. This could be data stored on the disk of a server, data stored in a database, or data stored in a storage account. Regardless of the storage mechanism, encryption of data at rest ensures that the stored data is unreadable without the keys and secrets needed to decrypt it. If an attacker was to obtain a hard drive with encrypted data and did not have access to the encryption keys, the attacker would not compromise the data without great difficulty.

The actual data that is encrypted could vary in its content, usage, and importance to the organization. This could be financial information critical to the business, intellectual property that has been developed by the business, personal data about customers or employees that the business stores, and even the keys and secrets used for the encryption of the data itself.

Here's a diagram that shows what encrypted customer data might look like as it sits in a database.

![An illustration showing an example of encryption at rest. The data is saved in the storage in an encrypted form accessed only through a key.](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/encryption-at-rest.png)

## Encryption in transit

Data in transit is the data actively moving from one location to another, such as across the internet or through a private network. Secure transfer can be handled by several different layers. It could be done by encrypting the data at the application layer prior to sending it over a network. HTTPS is an example of application layer in transit encryption.

You can also set up a secure channel, like a virtual private network (VPN), at a network layer, to transmit data between two systems.

Encrypting data in transit protects the data from outside observers and provides a mechanism to transmit data while limiting risk of exposure.

This diagram shows the process. Here, customer data is encrypted as it's sent over the network. Only the receiver has the secret key that can decrypt the data to a usable form.

![An illustration showing an example of encryption in transit. The data is encrypted before it is transferred. Once it reaches the destination, the data is then decrypted.](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/encryption-in-transit.png)

## Encryption on Azure

Let's take a look at some ways that Azure enables you to encrypt data across services.

![Image representing encrypted storage](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/4-encrypt-raw-storage.png)

**Encrypt raw storage**

**Azure Storage Service Encryption** for data at rest helps you protect your data to meet your organizational security and compliance commitments. With this feature, the Azure storage platform automatically encrypts your data before persisting it to Azure Managed Disks, Azure Blob storage, Azure Files, or Azure Queue storage, and decrypts the data before retrieval. The handling of encryption, encryption at rest, decryption, and key management in Storage Service Encryption is transparent to applications using the services.

![Image representing an encrypted virtual machine](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/4-encrypt-virtual-machines.png)

**Encrypt virtual machine disks**

Storage Service Encryption provides low-level encryption protection for data written to physical disk, but how do you protect the virtual hard disks (VHDs) of virtual machines? If malicious attackers gained access to your Azure subscription and got the VHDs of your virtual machines, how would you ensure they would be unable to access the stored data?

**Azure Disk Encryption** is a capability that helps you encrypt your Windows and Linux IaaS virtual machine disks. Azure Disk Encryption leverages the industry-standard BitLocker feature of Windows and the dm-crypt feature of Linux to provide volume encryption for the OS and data disks. The solution is integrated with Azure Key Vault to help you control and manage the disk encryption keys and secrets (and you can use managed service identities for accessing Key Vault).

For Contoso Shipping, using VMs was one of the first moves toward the cloud. Having all the VHDs encrypted is a very easy, low-impact way to ensure that you are doing all you can to secure your company's data.

![Image representing an encrypted database](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/4-encrypt-databases.png)

**Encrypt databases**

**Transparent data encryption (TDE)** helps protect Azure SQL Database and Azure Data Warehouse against the threat of malicious activity. It performs real-time encryption and decryption of the database, associated backups, and transaction log files at rest without requiring changes to the application. By default, TDE is enabled for all newly deployed Azure SQL Database instances.

TDE encrypts the storage of an entire database by using a symmetric key called the database encryption key. By default, Azure provides a unique encryption key per logical SQL Server instance and handles all the details. Bring your own key (BYOK) is also supported with keys stored in Azure Key Vault (see below).

Because TDE is enabled by default, you are confident that Contoso Shipping has the proper protections in place for data stored in the company's databases.

![Image representing an encrypted secret](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/4-encrypt-secrets.png)

**Encrypt secrets**

We've seen that the encryption services all use keys to encrypt and decrypt data, so how do we ensure that the keys themselves are secure? Corporations may also have passwords, connection strings, or other sensitive pieces of information that they need to securely store. In Azure, we can use **Azure Key Vault** to protect our secrets.

Azure Key Vault is a centralized cloud service for storing your application secrets. Key Vault helps you control your applications' secrets by keeping them in a single, central location and by providing secure access, permissions control, and access logging capabilities. It is useful for a variety of scenarios:

- *Secrets management*. You can use Key Vault to securely store and tightly control access to tokens, passwords, certificates, *Application Programming Interface* (API) keys, and other secrets.
- *Key management*. You also can use Key Vault as a key management solution. Key Vault makes it easier to create and control the encryption keys used to encrypt your data.
- *Certificate management*. Key Vault lets you provision, manage, and deploy your public and private *Secure Sockets Layer/ Transport Layer Security* (SSL/ TLS) certificates for your Azure, and internally connected, resources more easily.
- *Store secrets backed by hardware security modules* (HSMs). The secrets and keys can be protected either by software, or by FIPS 140-2 Level 2 validated HSMs.

The benefits of using Key Vault include:

- *Centralized application secrets*. Centralizing storage for application secrets allows you to control their distribution, and reduces the chances that secrets may be accidentally leaked.
- *Securely stored secrets and keys*. Azure uses industry-standard algorithms, key lengths, and HSMs, and access requires proper authentication and authorization.
- *Monitor access and use*. Using Key Vault, you can monitor and control access to company secrets.
- *Simplified administration of application secrets*. Key Vault makes it easier to enroll and renew certificates from public Certificate Authorities (CAs). You can also scale up and replicate content within regions, and use standard certificate management tools.
- *Integrate with other Azure services*. You can integrate Key Vault with storage accounts, container registries, event hubs and many more Azure services.

Because Azure AD identities can be granted access to use Azure Key Vault secrets, applications with managed service identities enabled can automatically and seamlessly acquire the secrets they need.

## Summary

As you may know, encryption is often the last layer of defense from attackers and is an important piece of a layered approach to securing your systems. Azure provides built-in capabilities and services to encrypt and protect data from unintended exposure. Protection of customer data stored within Azure services is of paramount importance to Microsoft and should be included in any design. Foundational services such as Azure Storage, Azure Virtual Machines, Azure SQL Database, and Azure Key Vault can help secure your environment through encryption.

------

## Next unit: Protect your network

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/5-network-security)


  





# Protect your network

- 8 minutes

Securing your network from attacks and unauthorized access is an important part of any architecture. Here, we'll take a look at what network security looks like, how to integrate a layered approach into your architecture, and how Azure can help you provide network security for your environment.

## A layered approach to network security

You've probably noticed that a common theme throughout this module is the emphasis of a layered approach to security, and this is no different at the network layer. It's not enough to just focus on securing the network perimeter, or focusing on the network security between services inside a network. A layered approach provides multiple levels of protection, so that if an attacker gets through one layer, there are further protections in place to limit further attack.

Let's take a look at how Azure can provide the tools for a layered approach to securing your network footprint.

![Image representing a secure internet](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/5-internet-protection.png)

**Internet protection**

If we start on the perimeter of the network, we're focused on limiting and eliminating attacks from the internet. We suggest first assessing the resources that are internet-facing, and to only allow inbound and outbound communication where necessary. Make sure you identify all resources that are allowing inbound network traffic of any type, and then ensure they are restricted to only the ports and protocols required. Azure Security Center is a great place to look for this information, because it will identify internet-facing resources that don't have network security groups associated with them, as well as resources that are not secured behind a *firewall*.

### What is a Firewall?

A firewall is a service that grants server access based on the originating IP address of each request. You create firewall rules that specify ranges of IP addresses. Only clients from these granted IP addresses will be allowed to access the server. Firewall rules, generally speaking, also include specific network protocol and port information.

To provide inbound protection at the perimeter, you have several choices.

- **Azure Firewall** is a managed, cloud-based, network security service that protects your Azure Virtual Network resources. It is a fully stateful firewall as a service with built-in high availability and unrestricted cloud scalability. Azure Firewall provides inbound protection for non-HTTP/S protocols. Examples of non-HTTP/S protocols include: Remote Desktop Protocol (RDP), Secure Shell (SSH), and File Transfer Protocol (FTP). It also provides outbound, network-level protection for all ports and protocols, and application-level protection for outbound HTTP/S.
- **Azure Application Gateway** is a load balancer that includes a Web Application Firewall (WAF) that provides protection from common, known vulnerabilities in websites. It is specifically designed to protect HTTP traffic.
- **Network virtual appliances (NVAs)** are ideal options for non-HTTP services or advanced configurations, and are similar to hardware firewall appliances.

### Stopping Distributed Denial of Service (DDos) attacks

Any resource exposed on the internet is at risk of being attacked by a denial of service attack. These types of attacks attempt to overwhelm a network resource by sending so many requests that the resource becomes slow or unresponsive.

When you combine **Azure DDoS Protection** with application design best practices, you help provide defense against DDoS attacks. DDoS Protection leverages the scale and elasticity of Microsoft’s global network to bring DDoS mitigation capacity to every Azure region. The Azure DDoS Protection service protects your Azure applications by scrubbing traffic at the Azure network edge before it can impact your service's availability. Within a few minutes of attack detection, you are notified using Azure Monitor metrics.

This diagram shows network traffic flowing into Azure from both customers and an attacker. Azure DDoS protection identifies the attacker's attempt to overwhelm the network and blocks further traffic from reaching Azure services. Legitimate traffic from customers still flows into Azure without any interruption of service.

![An illustration showing Azure DDoS protection installed between virtual network and external user requests. The Azure DDoS protection blocks malicious traffic attack but forwards the legitimate traffic to the intended destination.](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/ddos.png)

Azure DDoS Protection provides the following service tiers:

- **Basic.** The Basic service tier is automatically enabled as part of the Azure platform. Always-on traffic monitoring and real-time mitigation of common network-level attacks provide the same defenses that Microsoft’s online services use. Azure’s global network is used to distribute and mitigate attack traffic across regions.

- Standard.

   

  The Standard service tier provides additional mitigation capabilities that are tuned specifically to Microsoft Azure Virtual Network resources. DDoS Protection Standard is simple to enable and requires no application changes. Protection policies are tuned through dedicated traffic monitoring and machine learning algorithms. Policies are applied to public IP addresses which are associated with resources deployed in virtual networks, such as Azure Load Balancer and Application Gateway. DDoS standard protection can mitigate the following types of attacks:

  - Volumetric attacks. The attackers goal is to flood the network layer with a substantial amount of seemingly legitimate traffic.
  - Protocol attacks. These attacks render a target inaccessible, by exploiting a weakness in the layer 3 and layer 4 protocol stack.
  - Resource (application) layer attacks. These attacks target web application packets to disrupt the transmission of data between hosts.

## Controlling the traffic inside your virtual network

![Image representing a secure virtual network](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/5-vnet-security.png)

**Virtual network security**

Once inside a virtual network (VNet), it's crucial that you limit communication between resources to only what is required.

For communication between virtual machines, *Network Security Groups* (NSGs) are a critical piece to restrict unnecessary communication.

Network Security Groups allow you to filter network traffic to and from Azure resources in an Azure virtual network. An NSG can contain multiple inbound and outbound security rules that enable you to filter traffic to and from resources by source and destination IP address, port, and protocol. They provide a list of allowed and denied communication to and from network interfaces and subnets, and are fully customizable.

You can completely remove public internet access to your services by restricting access to service endpoints. With service endpoints, Azure service access can be limited to your virtual network.

![Image representing a secure network](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/5-network-integration.png)

**Network integration**

It's common to have existing network infrastructure that needs to be integrated to provide communication from on-premises networks or to provide improved communication between services in Azure. There are a few key ways to handle this integration and improve the security of your network.

Virtual private network (VPN) connections are a common way of establishing secure communication channels between networks. Connection between Azure Virtual Network and an on-premises VPN device is a great way to provide secure communication between your network and your VNet on Azure.

To provide a dedicated, private connection between your network and Azure, you can use Azure ExpressRoute. ExpressRoute lets you extend your on-premises networks into the Microsoft cloud over a private connection facilitated by a connectivity provider. With ExpressRoute, you can establish connections to Microsoft cloud services, such as Microsoft Azure, Office 365, and Dynamics 365. This improves the security of your on-premises communication by sending this traffic over the private circuit instead of over the public internet. You don't need to allow access to these services for your end users over the public internet, and you can send this traffic through appliances for further traffic inspection.

## Summary

A layered approach to network security helps reduce your risk of exposure through network-based attacks. Azure provides several services and capabilities to secure your internet-facing resource, internal resources, and communication between on-premises networks. These features make it possible to create secure solutions on Azure.

You can also combine multiple Azure networking and security services to manage your network security and provide increased layered protection. For example, you can use Azure Firewall to protect inbound and outbound traffic to the Internet, and Network Security Groups to limit traffic to resources inside your virtual networks.

------

## Next unit: Protect your shared documents

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/6-azure-information-protection)







# Protect your shared documents

- 3 minutes

**Microsoft Azure Information Protection** (MSIP or sometimes referred to as AIP) is a cloud-based solution that helps organizations classify and optionally protect documents and emails by applying labels.

Labels can be applied automatically based on rules and conditions, manually, or a combination of both where users are guided by recommendations.

The following screen capture is an example of MSIP in action on a user's computer. In this example, the administrator has configured a label with rules that detect sensitive data. When a user saves a Microsoft Word document containing a credit card number, a custom tooltip is displayed. The tooltip recommends labeling the file as *Confidential - All Employees*, which is a label that the administrator has configured. This label classifies the document and protects it.

![Screenshot of a Microsoft Word window with the previously described message displaying](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/6-info-protect-recommend-callout.png)

After your content is classified, you can track and control how the content is used. For example, you can:

- Analyze data flows to gain insight into your business
- Detect risky behaviors and take corrective measures
- Track access to documents
- Prevent data leakage or misuse of confidential information

 Note

You can purchase MSIP either as a standalone solution, or through one of the following Microsoft licensing suites: Enterprise Mobility + Security, or Microsoft 365 Enterprise.

------

## Next unit: Azure Advanced Threat Protection

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/7-advanced-threat-protection)









# Azure Advanced Threat Protection

- 5 minutes

**Azure Advanced Threat Protection** (Azure ATP) is a cloud-based security solution that identifies, detects, and helps you investigate advanced threats, compromised identities, and malicious insider actions directed at your organization.

Azure ATP is capable of detecting known malicious attacks and techniques, security issues, and risks against your network.

## Azure ATP components

Azure ATP consists of several components.

**Azure ATP portal**

Azure ATP has its own portal, through which you can monitor and respond to suspicious activity. The Azure ATP portal allows you to create your Azure ATP instance, and view the data received from Azure ATP sensors. You can also use the portal to monitor, manage, and investigate threats in your network environment. You can sign in to the Azure ATP portal at [https://portal.atp.azure.com](https://portal.atp.azure.com/). You must sign in with a user account that is assigned to an Azure AD security group that has access to the Azure ATP portal.

**Azure ATP sensor**

Azure ATP sensors are installed directly on your domain controllers. The sensor monitors domain controller traffic without requiring a dedicated server or configuring port mirroring.

**Azure ATP cloud service**

Azure ATP cloud service runs on Azure infrastructure and is currently deployed in the United States, Europe, and Asia. Azure ATP cloud service is connected to Microsoft's intelligent security graph.

![Screenshot of Azure Advanced Threat Protection dashboard and event timeline, showing security events such as HoneyToken activity, remote execution attempt detected, and suspicious service created](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/7-atp-sa-timeline.png)

## Purchasing Azure Advanced Threat Protection

Azure ATP is available as part of the Enterprise Mobility + Security E5 suite (EMS E5) and as a standalone license. You can acquire a license directly from the [Enterprise Mobility + Security Pricing Options](https://www.microsoft.com/cloud-platform/enterprise-mobility-security-pricing) page or through the Cloud Solution Provider (CSP) licensing model. It is not available to purchase via the Azure portal.

------

## Next unit: Summary

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/8-summary)


  





# Summary

- 5 minutes

In this module, we discussed the basic concepts for protecting your infrastructure and data when you work in the cloud.

**Defense in depth** is the overriding theme - think about security as a multi-layer, multi-vector concern. Threats come from places we don't expect, and they can come with strength that will surprise us.

![Concept of being safe from security threats](https://docs.microsoft.com/en-us/learn/modules/intro-to-security-in-azure/media/6-heading.png)

Azure has out-of-the-box help for a great deal of the security issues we face. One of the first steps we should take is assessing how much help from Azure we can use based on whether we're leveraging IaaS, PaaS, or SaaS.

Azure Security Center centralizes much of the help Azure has to offer. It provides a single dashboard, with a view into many of your services, and helps make sure you are following best practices. Continuously updated machine learning algorithms help identify whether the latest threats are aimed at your resources. And it helps your organization mitigate threats.

Of course, this module is introductory. Security is a deep and complex topic, so whatever your cloud approach, an ongoing security education is necessary. But this module should get you started in the right direction, so you know what you need to learn next.

## Learn More

Here are some places to go to learn more about what we've covered today:

- [Azure Security (Trust Center)](https://www.microsoft.com/trustcenter/security/azure-security)
- [Azure Security Center planning and operations guide](https://docs.microsoft.com/azure/security-center/security-center-planning-and-operations-guide)
- [What is Microsoft Azure Information Protection?](https://docs.microsoft.com/azure/information-protection/what-is-information-protection/)
- [Azure Advanced Threat Protection](https://azure.microsoft.com/features/azure-advanced-threat-protection/)

## Check your knowledge

\1. 

Cloud security is a shared responsibility between you and your cloud provider. Which category of cloud services requires the greatest security effort on your part?



Infrastructure as a service (IaaS)



Platform as a service (PaaS)



Software as a service (SaaS)

\2. 

Which of these helps you most easily disable an account when an employee leaves your company?



Enforce multi-factor authentication (MFA)



Monitor sign-on attempts



Use single sign-on (SSO)

\3. 

Which of these is the *strongest* way to protect sensitive customer data?



Encrypt data as it sits in your database



Encrypt data as it travels over the network



Encrypt data both as it sits in your database and as it travels over the network

\4. 

There has been an attack on your public-facing website, and the application's resources have been overwhelmed and exhausted, and are now unavailable to users. What service should you use to prevent this type of attack?



DDoS protection



Azure Firewall



Network Security Group



Application Gateway

\5. 

You want to store certificates in Azure to centrally manage them for your services. Which Azure service should you use?



MSIP



Azure AD



Azure Key Vault



Azure ATP









# PART 10: Apply and monitor infrastructure standards with Azure Policy

# Introduction

- 2 minutes

Good IT governance involves planning your initiatives and setting priorities on a strategic level to help manage and prevent issues.

You need good governance when:

- You have multiple engineering teams working in Azure
- You have multiple subscriptions in your tenant
- You have regulatory requirements which must be enforced
- You want to ensure standards are followed for all IT allocated resources

You could enforce standards by not allowing teams to directly create Azure resources - and instead have the IT team define and deploy all cloud-based assets. This is often the solution in on-premises solutions, but this reduces the team agility and ability to innovate. Instead, Azure provides several tools you can use to enforce and validate your standards, while still allowing your engineering teams to create and own their own resources in the cloud.

In addition to providing IT standards, you need to be able to monitor your resources to make sure they are responsive and performing properly. Azure provides several built-in features to track and analyze your resource utilization and performance.

In this module, you will:

- Apply policies to control and audit resource creation
- Learn how role-based security can fine-tune access to your resources
- Understand Microsoft's policies and privacy guarantees
- Learn how to monitor your resources

------

## Next unit: Define IT compliance with Azure Policy

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/2-azure-policy)







# Define IT compliance with Azure Policy

- 8 minutes

Planning out a consistent cloud infrastructure starts with setting up policy. Your policies will enforce your rules for created resources, so your infrastructure stays compliant with your corporate standards, cost requirements, and service-level agreements (SLAs) you have with your customers.

![Icon representing Azure Blueprint](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/media/2-azurepolicy.png)

**Azure Policy** is a service in Azure that you use to define, assign, and, manage standards for resources in your environment. It can prevent the creation of disallowed resources, ensure new resources have specific settings applied, and run evaluations of your existing resources to scan for non-compliance.

Azure Policy comes with many built-in policy and initiative definitions that you can use, under categories such as Storage, Networking, Compute, Security Center, and Monitoring.

Imagine we allow anyone in our organization to create virtual machines (VMs). We want to control costs, so the administrator of our Azure tenant defines a policy that prohibits the creation of any VM with more than 4 CPUs. Once the policy is implemented, Azure Policy will stop anyone from creating a new VM outside the list of allowed stock keeping units (SKUs). Also, if you try to *update* an existing VM, it will be checked against policy. Finally, Azure Policy will audit all the existing VMs in our organization to ensure our policy is enforced. It can audit non-compliant resources, alter the resource properties, or stop the resource from being created.

 Tip

Azure Policy can integrate with Azure DevOps, by applying any continuous integration and delivery pipeline policies that affect the pre-deployment and post-deployment of your applications.

## Creating a policy

The process of creating and implementing an Azure Policy begins with creating a *policy definition*. Every policy definition has conditions under which it is enforced. And, it has an accompanying effect that takes place if the conditions are met. To apply a policy, you will:

1. Create a policy definition
2. Assign a definition to a scope of resources
3. View policy evaluation results

### What is a policy definition?

A *policy definition* expresses what to evaluate and what action to take. For example, you could ensure all public websites are secured with HTTPS, prevent a particular storage type from being created, or force a specific version of SQL Server to be used.

Here are some of the most common policy definitions you can apply.

| Policy definition            | Description                                                  |
| :--------------------------- | :----------------------------------------------------------- |
| Allowed Storage Account SKUs | This policy definition has a set of conditions/rules that determine whether a storage account that is being deployed is within a set of SKU sizes. Its effect is to deny all storage accounts that do not adhere to the set of defined SKU sizes. |
| Allowed Resource Type        | This policy definition has a set of conditions/rules to specify the resource types that your organization can deploy. Its effect is to deny all resources that are not part of this defined list. |
| Allowed Locations            | This policy enables you to restrict the locations that your organization can specify when deploying resources. Its effect is used to enforce your geographic compliance requirements. |
| Allowed Virtual Machine SKUs | This policy enables you to specify a set of VM SKUs that your organization can deploy. |
| Not allowed resource types   | Prevents a list of resource types from being deployed.       |

The policy definition itself is represented as a JSON file - you can use one of the pre-defined definitions in the portal or create your own (either modifying an existing one or starting from scratch). There are [hundreds of samples available on GitHub](https://github.com/Azure/azure-policy).

Here is an example of a Compute policy that only allows specific virtual machine sizes:

JSONCopy

```json
{
  "if": {
    "allOf": [
      {
        "field": "type",
        "equals": "Microsoft.Compute/virtualMachines"
      },
      {
        "not": {
          "field": "Microsoft.Compute/virtualMachines/sku.name",
          "in": "[parameters('listOfAllowedSKUs')]"
        }
      }
    ]
  },
  "then": {
    "effect": "Deny"
  }
}
```

Notice the `[parameters('listofAllowedSKUs')]` value; this is a replacement token that will be filled in when the policy definition is applied to a scope. When a parameter is defined, it's given a name and optionally given a value.

### Assign a definition to a scope of resources

Once you've defined one or more policy definitions, you'll need to assign them. A *policy assignment* is a policy definition that has been assigned to take place within a specific scope.

This scope could range from a full subscription down to a resource group. Policy assignments are inherited by all child resources. This means that if a policy is applied to a resource group, it is applied to all the resources within that resource group. However, you can exclude a subscope from the policy assignment. For example, we could enforce a policy for an entire subscription and then exclude a few select resource groups.

You can assign any of these policies through the Azure portal, PowerShell, or Azure CLI. When you assign a policy definition, you will need to supply any parameters which are defined.

![Screenshot showing parameters when assigning a policy to a scope in the Azure Portal](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/media/2-policy-parameters.png)

### Policy effects

Requests to create or update a resource through Azure Resource Manager are evaluated by Azure Policy first. Policy creates a list of all assignments that apply to the resource and then evaluates the resource against each definition. Policy processes several of the effects before handing the request to the appropriate Resource Provider to avoid any unnecessary processing if the resource violates policy.

Each policy definition in Azure Policy has a single effect. That effect determines what happens when the associated policy rule is matched. When that happens, Azure Policy will take a specific action based on the assigned effect.

| Policy Effect           | What happens?                                                |
| :---------------------- | :----------------------------------------------------------- |
| Deny                    | The resource creation/update fails due to policy.            |
| Disabled                | The policy rule is ignored (disabled). Often used for testing. |
| Append                  | Adds additional parameters/fields to the requested resource during creation or update. A common example is adding tags on resources such as Cost Center or specifying allowed IPs for a storage resource. |
| Audit, AuditIfNotExists | Creates a warning event in the activity log when evaluating a non-compliant resource, but it doesn't stop the request. |
| DeployIfNotExists       | Executes a template deployment when a specific condition is met. For example, if SQL encryption is enabled on a database, then it can run a template after the DB is created to set it up a specific way. |

### View policy evaluation results

Azure Policy can allow a resource to be created even if it doesn't pass validation. In these cases, you can have it trigger an audit event which can be viewed in the Azure Policy portal, or through command-line tools. The easiest approach is in the portal as it provides a nice graphical overview which you can explore. You can find the Azure Policy section through the search field or *All Services*.

![Azure portal showing the Azure Portal Overview screen](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/media/2-policy-portal.png)

From this screen, you can spot resources which are not compliant and take action to correct them.

 Tip

If you continue in the Azure Fundamentals learning path, you'll see Azure Policy in more detail in the [Control and organize Azure resources with Azure Resource Manager](https://docs.microsoft.com/learn/modules/control-and-organize-with-azure-resource-manager/) module.

------

## Next unit: Organize policy with initiatives

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/3-initiatives)









# Organize policy with initiatives

- 5 minutes

Managing a few policy definitions is easy, but once you have more than a few, you will want to organize them. That's where *initiatives* come in.

Initiatives work alongside policies in Azure Policy. An *initiative definition* is a set or group of policy definitions to help track your compliance state for a larger goal. Even if you have a single policy, we recommend using initiatives if you anticipate increasing the number of policies over time.

Like a policy assignment, an *initiative assignment* is an initiative definition assigned to a specific scope. Initiative assignments reduce the need to make several initiative definitions for each scope. This scope could also range from a management group to a resource group.

Once defined, initiatives can be assigned just as policies can - and they apply all the associated policy definitions.

### Defining initiatives

Initiative definitions simplify the process of managing and assigning policy definitions by grouping a set of policies into a single item. For example, you could create an initiative named *Enable Monitoring in Azure Security Center*, with a goal to monitor all the available security recommendations in your Azure Security Center.

Under this initiative, you would have the following policy definitions:

| Policy definition                                      | Purpose                                                      |
| :----------------------------------------------------- | :----------------------------------------------------------- |
| Monitor unencrypted SQL Database in Security Center    | For monitoring unencrypted SQL databases and servers.        |
| Monitor OS vulnerabilities in Security Center          | For monitoring servers that do not satisfy the configured baseline. |
| Monitor missing Endpoint Protection in Security Center | For monitoring servers without an installed endpoint protection agent. |

You can define initiatives using the Azure portal, or command-line tools. In the portal, you use the "Authoring" section.

![Screenshot showing Azure portal defining initiatives and definitions](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/media/3-define-initiatives.png)

### Assigning initiatives

Like a policy assignment, an *initiative assignment* is an initiative definition assigned to a specific scope. Initiative assignments reduce the need to make several initiative definitions for each scope. This scope could also range from a management group to a resource group.

------

## Next unit: Enterprise governance management

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/4-management-groups)







# Enterprise governance management

- 5 minutes

Access management occurs at the Azure subscription level. This allows an organization to configure each division of the company in a specific fashion based on their responsibilities and requirements. Planning and keeping rules consistent across subscriptions can be challenging without a little help.

Azure Management Groups are containers for managing access, policies, and compliance across *multiple* Azure subscriptions. Management groups allow you to order your Azure resources hierarchically into collections, which provide a further level of classification that is above the level of subscriptions. All subscriptions within a management group automatically inherit the conditions applied to the management group. Management groups give you enterprise-grade management at a large scale no matter what type of subscriptions you might have.

The following diagram shows an example of creating a hierarchy for governance using management groups.

![Image showing Azure Management Groups as a tree graph of relationships](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/media/4-management-groups-tree.png)

Create a hierarchy so you can apply a policy, for example, limit VM locations to US West Region on the group "Infrastructure Team management group". This policy will inherit onto both EA subscriptions under that management group and will apply to all VMs under those subscriptions. This security policy cannot be altered by the resource or subscription owner allowing for improved governance.

Another scenario where you would use management groups is to provide user access to multi subscriptions. By moving many subscriptions under that management group, you can create one role-based access control (RBAC) assignment on the management group, which will inherit that access to all the subscriptions. One assignment on the management group can enable users to have access to everything they need instead of scripting RBAC rules over different subscriptions.

You can manage your Azure subscriptions more effectively by using Azure Policy and Azure role-based access controls (RBACs). These provide distinct governance conditions that you can apply to each management group. The resources and subscriptions you assign to a management group automatically inherit the conditions that you apply to that management group.

 Tip

If you continue in the Azure Fundamentals learning path, you'll learn more about RBAC in the [Control and organize Azure resources with Azure Resource Manager](https://docs.microsoft.com/learn/modules/control-and-organize-with-azure-resource-manager/) module.

------

## Next unit: Define standard resources with Azure Blueprints

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/5-azure-blueprints)









# Define standard resources with Azure Blueprints

- 5 minutes

Adhering to security or compliance requirements, whether government or industry requirements, can be difficult and time-consuming. To help you with auditing, traceability, and compliance with your deployments, use **Azure Blueprint**artifacts and tools.

![Icon representing Azure Blueprint](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/media/5-azureblueprint.png)

**Azure Blueprint** allows you to define a repeatable set of Azure resources that implement and adhere to your organization's standards, patterns, and requirements. Blueprint enables development teams to rapidly build and deploy new environments with the knowledge that they're building within organizational compliance with a set of built-in components that speed up development and delivery.

Azure Blueprint is a declarative way to orchestrate the deployment of various resource templates and other artifacts, such as:

- Role assignments
- Policy assignments
- Azure Resource Manager templates
- Resource groups

The process of implementing Azure Blueprint consists of the following high-level steps:

1. Create an Azure Blueprint
2. Assign the blueprint
3. Track the blueprint assignments

With Azure Blueprint, the relationship between the blueprint definition (what *should be* deployed) and the blueprint assignment (what *was* deployed) is preserved. This connection supports improved deployment tracking and auditing.

Azure Blueprints are different from Azure Resource Manager Templates. When Azure Resource Manager Templates deploy resources, they have no active relationship with the deployed resources (they exist in a local environment or source control). By contrast, with Azure Blueprint, each deployment is tied to an Azure Blueprint package. This means that the relationship with resources will be maintained, even after deployment. Managing relationships, in this way, improves auditing and tracking capabilities.

Azure Blueprints are also useful in Azure DevOps scenarios, where blueprints are associated with specific build artifacts and release pipelines and can be tracked more rigorously.

------

## Next unit: Explore your service compliance with Compliance Manager

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/6-azure-compliance)









# Explore your service compliance with Compliance Manager

- 8 minutes

Governing your own resources and how they are used is only part of the solution when using a cloud provider. You also have to understand how the *provider* manages the underlying resources you are building on.

Microsoft takes this management very seriously and provides full transparency with four sources:

1. Microsoft Privacy Statement
2. Microsoft Trust Center
3. Service Trust Portal
4. Compliance Manager

## Microsoft Privacy Statement

The Microsoft privacy statement explains what personal data Microsoft processes, how Microsoft processes it, and for what purposes.

The statement applies to the interactions Microsoft has with you and Microsoft products such as Microsoft services, websites, apps, software, servers, and devices. It is intended to provide openness and honesty about how Microsoft deals with personal data in its products and services.

There is a link to the privacy statement in the summary of this module.

## What is the Microsoft Trust Center?

**Trust Center** is a website resource containing information and details about how Microsoft implements and supports security, privacy, compliance, and transparency in all Microsoft cloud products and services. The Trust Center is an important part of the Microsoft Trusted Cloud Initiative, and provides support and resources for the legal and compliance community including:

- In-depth information about security, privacy, compliance offerings, policies, features, and practices across Microsoft cloud products.
- Recommended resources in the form of a curated list of the most applicable and widely-used resources for each topic.
- Information specific to key organizational roles, including business managers, tenant admins or data security teams, risk assessment and privacy officers, and legal compliance teams.
- Cross-company document search, which is coming soon and will enable existing cloud service customers to search the Service Trust Portal.
- Direct guidance and support for when you can't find what you're looking for.

![Screenshot of the Trust Center website](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/media/6-trustcenter.png)

## What is the Service Trust Portal?

The **Service Trust Portal** (STP) hosts the Compliance Manager service, and is the Microsoft public site for publishing audit reports and other compliance-related information relevant to Microsoft’s cloud services. STP users can download audit reports produced by external auditors and gain insight from Microsoft-authored reports that provide details on how Microsoft builds and operates its cloud services.

STP also includes information about how Microsoft online services can help your organization maintain and track compliance with standards, laws, and regulations, such as:

- ISO
- SOC
- NIST
- FedRAMP
- GDPR

![Screenshot of the Trust Center website](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/media/6-servicetrustportal.png)

Service Trust Portal is a companion feature to the Trust Center, and allows you to:

- Access audit reports across Microsoft cloud services on a single page.
- Access compliance guides to help you understand how can you use Microsoft cloud service features to manage compliance with various regulations.
- Access trust documents to help you understand how Microsoft cloud services help protect your data.

## Compliance Manager

**Compliance Manager** is a workflow-based risk assessment dashboard within the Trust Portal that enables you to track, assign, and verify your organization's regulatory compliance activities related to Microsoft professional services and Microsoft cloud services such as Office 365, Dynamics 365, and Azure.

Compliance Manager provides the following features:

- Combines the following three items:
  1. Detailed information provided by Microsoft to auditors and regulators, as part of various third-party audits of Microsoft 's cloud services against various standards (for example, ISO 27001, ISO 27018, and NIST).
  2. Information that Microsoft compiles internally for its compliance with regulations (such as HIPAA and the EU GDPR).
  3. An organization's self-assessment of their own compliance with these standards and regulations.
- Enables you to assign, track, and record compliance and assessment-related activities, which can help your organization cross team barriers to achieve your organization's compliance goals.
- Provides a Compliance Score to help you track your progress and prioritize auditing controls that will help reduce your organization's exposure to risk.
- Provides a secure repository in which to upload and manage evidence and other artifacts related to compliance activities.
- Produces richly detailed reports in Microsoft Excel that document the compliance activities performed by Microsoft and your organization, which can be provided to auditors, regulators, and other compliance stakeholders.

![Screenshot showing Compliance Manager website](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/media/6-compliancemanager.png)

Compliance Manager provides ongoing risk assessments with a risk-based scores reference displayed in a dashboard view for regulations and standards. Alternatively, you can create assessments for the regulations or standards that matter more to your organization.

As part of the risk assessment, Compliance Manager also provides recommended actions you can take to improve your regulatory compliance. You can view all action items, or select the action items that correspond with a specific certification.

 Important

Compliance Manager is a dashboard that provides a summary of your data protection and compliance stature and recommendations for improvement. The Customer Actions provided in Compliance Manager are recommendations only; it is up to each organization to evaluate the effectiveness of these recommendations in their respective regulatory environment prior to implementation. Recommendations found in Compliance Manager should not be interpreted as a guarantee of compliance.

------

## Next unit: Monitor your service health

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/7-monitoring)







# Monitor your service health

- 8 minutes

Defining policy and access provides fine-grained control over resources in your cloud IT infrastructure. Once those resources are deployed, you will want to know about any issues or performance problems they might encounter.

Azure provides two primary services to monitor the health of your apps and resources.

1. Azure Monitor
2. Azure Service Health

## Azure Monitor

![Icon representing Azure Monitor](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/media/7-azuremonitor.png)

**Azure Monitor** maximizes the availability and performance of your applications by delivering a comprehensive solution for collecting, analyzing, and acting on telemetry from your cloud and on-premises environments. It helps you understand how your applications are performing and proactively identifies issues affecting them and the resources they depend on.

### Data sources

Azure Monitor can collect data from a variety of sources. You can think of monitoring data for your applications in tiers ranging from your application, any operating system and services it relies on, down to the platform itself.

| Data tier                          | Description                                                  |
| :--------------------------------- | :----------------------------------------------------------- |
| Application monitoring data        | Data about the performance and functionality of the code you have written, regardless of its platform. |
| Guest OS monitoring data           | Data about the operating system on which your application is running. This could be running in Azure, another cloud, or on-premises. |
| Azure resource monitoring data     | Data about the operation of an Azure resource.               |
| Azure subscription monitoring data | Data about the operation and management of an Azure subscription, as well as data about the health and operation of Azure itself. |
| Azure tenant monitoring data       | Data about the operation of tenant-level Azure services, such as Azure Active Directory. |

### Diagnostic settings

As soon as you create an Azure subscription and start adding resources such as virtual machines and web apps, Azure Monitor starts collecting data. *Activity Logs* record when resources are created or modified and *Metrics* tell you how the resource is performing and the resources that it's consuming.

You can extend the data you're collecting into the actual operation of the resources by enabling **diagnostics** and adding an agent to compute resources. Under the resource settings you can enable Diagnostics

- *Enable guest-level monitoring*
- *Performance counters*: collect performance data
- *Event Logs*: enable various event logs
- *Crash Dumps*: enable or disable
- *Sinks*: send your diagnostic data to other services for more analysis
- *Agent*: configure agent settings

### Getting more data from your apps

Data monitoring is only useful if it improves your visibility of the operations in your computing environment. Azure Monitor includes several features and tools that provide valuable insights into your applications, and the other resources they may depend on.

**Application Insights** is a service that monitors the availability, performance, and usage of your web applications, whether they're hosted in the cloud or on-premises. It leverages the powerful data analysis platform in Log Analytics to provide you with deeper insights into your application's operations. Application Insights can diagnose errors, without waiting for a user to report them. Application Insights includes connection points to a variety of development tools, and integrates with Microsoft Visual Studio to support your DevOps processes.

**Azure Monitor for containers** is a service that is designed to monitor the performance of container workloads, which are deployed to managed Kubernetes clusters hosted on Azure Kubernetes Service (AKS). It gives you performance visibility by collecting memory and processor metrics from controllers, nodes, and containers, which are available in Kubernetes through the metrics API. Container logs are also collected.

**Azure Monitor for VMs** is a service that monitors your Azure VMs at scale, by analyzing the performance and health of your Windows and Linux VMs (including their different processes and interconnected dependencies on other resources, and external processes). Azure Monitor for VMs includes support for monitoring performance and application dependencies for VMs hosted on-premises, and for VMs hosted with other cloud providers.

Integrating any, or all, of these monitoring services with Azure Service Health has additional benefits. Staying informed of the health status of Azure services will help you understand if, and when, an issue affecting an Azure service is impacting your environment. What may seem like a localized problem could be the result of a more widespread issue, and Azure Service Health provides this kind of insight. Azure Service Health identifies any issues with Azure services that might affect your application. Azure Service Health also helps you to plan for scheduled maintenance.

### Responding to alert conditions

In addition to allowing you to analyze your monitoring data interactively, an effective monitoring solution must respond proactively to any critical conditions that are identified within the data it collects. This might involve, for example, sending a text or email to an administrator who is responsible for investigating an issue, or launching an automated process that attempts to correct an error condition.

**Alerts**. Azure Monitor proactively notifies you of critical conditions using alerts, and can potentially attempt to take corrective actions. Alert rules based on metrics can provide alerts in almost real-time, based on numeric values. Alert rules based on logs allow for complex logic across data, from multiple sources.

**Autoscale**. Azure Monitor uses Autoscale to ensure that you have the right amount of resources running to manage the load on your application effectively. Autoscale enables you to create rules that use metrics, collected by Azure Monitor, to determine when to automatically add resources to handle increases in load. Autoscale can also help reduce your Azure costs by removing resources that are not being used. You can specify a minimum and maximum number of instances, and provide the logic that determines when Autoscale should increase or decrease resources.

### Visualize monitoring data

Visualizations, such as charts and tables, are effective tools for summarizing monitoring data and for presenting data to different audiences. Azure Monitor has its own features for visualizing monitoring data, and it leverages other Azure services for publishing data for different audiences. Other tools you may use for visualizing data, for particular audiences and scenarios, include:

- Dashboards
- Views
- Power BI

### Integrate with other services

You'll often need to integrate Azure Monitor with other systems, and build customized solutions that use your monitoring data. Other Azure services can work with Azure Monitor to provide this integration.

## Azure Service Health

![Icon representing Azure Monitor](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/media/7-azureservicehealth.png)

**Azure Service Health** is a suite of experiences that provide personalized guidance and support when issues with Azure services affect you. It can notify you, help you understand the impact of issues, and keep you updated as the issue is resolved. Azure Service Health can also help you prepare for planned maintenance and changes that could affect the availability of your resources.

Azure Service Health is composed of the following views.

**Azure Status** provides a global view of the health state of Azure services. With Azure Status, you can get up-to-the-minute information on service availability. Everyone has access to Azure Status and can view all services that report their health state.

**Service Health** provides you with a customizable dashboard that tracks the state of your Azure services in the regions where you use them. In this dashboard, you can track active events such as ongoing service issues, upcoming planned maintenance, or relevant *Health advisories*. When events become inactive, they are placed in your *Health history* for up to 90 days. Finally, you can use the **Service Health** dashboard to create and manage service *Health alerts*, which notify you whenever there are service issues that affect you.

**Resource Health** helps you diagnose and obtain support when an Azure service issue affects your resources. It provides you details with about the current and past state of your resources. It also provides technical support to help you mitigate problems. In contrast to Azure Status, which informs you about service problems that affect a broad set of Azure customers, *Resource Health* gives you a personalized dashboard of your resources' health. *Resource Health* shows you times, in the past, when your resources were unavailable because of Azure service problems. It's then easier for you to understand if an SLA was violated.

Together, the Azure Service Health components provide you with a comprehensive view of the health status of Azure, at the level of granularity that is most relevant to you.

------

## Next unit: Summary

[Continue](https://docs.microsoft.com/en-us/learn/modules/intro-to-governance/8-summary)









# PART 11: Control and organize Azure resources with Azure Resource Manager

# Introduction

- 2 minutes

Imagine you've joined a company who has been moving to the cloud. This movement happened organically across different departments, and resulted in a lack of awareness of what's already been created and where everything is. There's no ability to easily determine who owns which resources. There's no enforcement of standards for things like resource names, resource sizes, and geographic locations. There's also been several instances where critical resources were inadvertently deleted, causing business-critical outages.

Your manager has asked you to head up an effort to put some order into the chaos, but you're new to Azure and aren't entirely sure what you can do to make this better.

Azure Resource Manager has a number of features that you can use to organize resources, enforce standards, and protect critical Azure resources from accidental deletion. We'll take a tour through these features, and show how you can use them to your advantage.

## Learning objectives

In this module, you will:

- Use resource groups to organize Azure resources
- Use tags to organize resources
- Apply policies to enforce standards in your Azure environments
- Use resource locks to protect critical Azure resources from accidental deletion

 Note

For this module, you will need use your own subscription to follow along. We'll be working with resources that will have no cost associated with them, so a trial subscription or a subscription you already have access to will work to follow along with these exercises.

------

## Next unit: Principles of resource groups

[Continue](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/2-principles-of-resource-groups)


  





# Principles of resource groups

- 10 minutes

In your first week on your new job, you've looked through the existing resources in your company's Azure subscription. There are a number of resource groups that contain many different resources, but they aren't organized into a coherent structure. You've worked on Azure before, but aren't entirely sure how resource groups work and what their role is. You've guessed (correctly) that they can play a role in how you organize your resources. Let's look at what they are, and how they can be used.

 Note

If you don't have an Azure subscription, create a [free account ](https://azure.microsoft.com/free/) before you begin.

## What are resource groups?

Resource groups are a fundamental element of the Azure platform. A resource group is a logical container for resources deployed on Azure. These resources are anything you create in an Azure subscription like virtual machines, Application Gateways, and CosmosDB instances. All resources must be in a resource group and a resource can only be a member of a single resource group. Resources can be moved between resource groups at any time. Resource groups can't be nested. Before any resource can be provisioned, you need a resource group for it to be placed in.

### Logical grouping

Resource groups exist to help manage and organize your Azure resources. By placing resources of similar usage, type, or location, you can provide some order and organization to resources you create in Azure. Logical grouping is the aspect that we're most interested in here, since there's a lot of disorder among our resources.

![Conceptual image showing a resource group box with a Function, VM, database, and app included](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/2-rg.png)

### Life cycle

If you delete a resource group, all resources contained within are also deleted. Organizing resources by life cycle can be useful in non-production environments, where you might try an experiment, but then dispose of it when done. Resource groups make it easy to remove a set of resources at once.

### Authorization

Resource groups are also a scope for applying role-based access control (RBAC) permissions. By applying RBAC permissions to a resource group, you can ease administration and limit access to allow only what is needed.

## Create a Resource Group

Resource groups can be created by using the following methods:

- Azure portal
- Azure PowerShell
- Azure CLI
- Templates
- Azure SDKs (like .NET, Java)

Let's walk through the steps you'd take to create a resource group in the Azure portal. If you'd like to follow along in your own subscription, you may.

1. Open a web browser and sign into the [Azure portal ](https://portal.azure.com/).

    Important

   Make sure to use your *own* subscription. When you are in the free sandbox environment, it will not allow you to create resource groups. You can tell which subscription you are using by looking at the tenant name under your profile picture. You can switch tenants by clicking on your profile picture and selecting **Switch Directory** from the options menu.

2. On the left pane, select **+ Create a resource**

3. Type **Resource Group** in the search box and hit Enter.

4. The first item in the list should be the resource group resource. Select it and then click the **Create** button.

   ![Search results searching the marketplace for a new resource group](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/2-create-search-resource-group.png)

5. Enter your resource group name, let's use **msftlearn-core-infrastructure-rg**. Select the subscription it should be in, and select the region for the resource group. Click **Review + Create** and then **Create** to create the resource group.

   ![Fill in the required fields to create the resource group](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/2-create-resource-group.png)

That's it, you've created a resource group that you can now use when you deploy Azure resources. Let's take a closer look at this resource group and some important things to consider.

## Explore a resource group and add a resource

In the portal, select **Resource groups** on the left menu, and select your newly created resource group. Note that you may also see a resource group called **NetworkWatcherRG**. You can ignore this resource group, it's created automatically to enable Network Watcher in Azure virtual networks.

![Overview panel of resource group](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/2-rg-overview.png)

On the Overview panel, there's the basic information about the resource group like the subscription it's in, the subscription ID, any tags that are applied, and a history of the deployments to this resource group. We'll cover tags in the next unit. The deployments link takes you to a new panel with the history of all deployments to this resource group. Anytime you create a resource, it's a deployment, and you see that history for the resource group here.

Across the top you can add more resources, change the columns in the list, move the resource group to another subscription, or delete it entirely.

On the left menu, there are a number of options

We don't have any resources in this resource group yet, so the list at the bottom is empty. Let's create a couple resources inside the resource group.

1. Click **+ Add** at the top or click the **Create resources**, either will work.

2. Search for **Virtual network**. The first result should be the virtual network resource. Click it, and on the next screen, make sure **Select a deployment model** is set to **Resource Manager**. Click **Create**.

3. Name the virtual network **msftlearn-vnet1**. For the **Resource group** drop-down, select the resource group that you created earlier. Enter **192.168.0.0/24** for both the **Address space** and subnet **Address range**. Leave the defaults for all other options, and click **Create**.

4. Repeat the steps again to create one more VNet, where both the **Address space** and subnet **Address range** are for a different network than your previous network, (e.g. **192.168.100.0/24**). Name it **msftlearn-vnet2**, and make sure to place it in the resource group that you created earlier.

5. Go back to your resource group, and on the **Overview** panel you should see the two VNets you created.

   ![Overview panel of resource group showing the VNet](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/2-rg-with-vnet.png)

Our resource group now contains two virtual network resources because we specified in our deployment (when we created the resources) which resource group we wanted the VNet to be placed in. We could create additional resources inside this resource group, or we could create additional resource groups in the subscription to deploy resources into.

When creating resources, you usually have the option to create a new resource group as an alternative to using an existing resource group. This simplifies the process a bit, but as you see in your new organization, can lead to resources spread across resource groups with little thought as to how to organize them.

## Use resource groups for organization

So how can you use resource groups to your advantage in your new organization? There are some guidelines and best practices that can help with the organization.

### Consistent naming convention

You can start with using an understandable naming convention. We named our resource group **msftlearn-core-infrastructure-rg**. We've given some indication of what it's used for (**msftlearn**), the types of resources contained within (**core-infrastructure**), and the type of resource it is itself (**rg**). This descriptive name gives us a better idea of what it is. If we had named it **my-resource-group** or **rg1**, we have no idea on a glance of what the usage may be. In this case, we can deduce that there are probably core pieces of infrastructure contained within. If we created additional VNets, storage accounts, or other resources the company may consider *core infrastructure*, we could place them here as well, to improve the organization of our resources. Naming conventions can vary widely between and even within companies, but some planning can help.

### Organizing principles

Resource groups can be organized in a number of ways, let's take a look at a few examples. We might put all resources that are *core infrastructure* into this resource group. But we could also organize them strictly by resource type. For example, put all VNets in one resource group, all virtual machines in another resource group, and all Azure Cosmos DB instances in yet another resource group.

![Image of resources organized by type](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/2-resource-type-rg.png)

We could organize them by environment (prod, qa, dev). In this case, all production resources are in one resource group, all test resources are in another resource group, and so on.

![Image of resources organized by environment](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/2-environment-rg.png)

We could organize them by department (marketing, finance, human resources). Marketing resources go in one resource group, finance in another resource group, and HR in a third resource group.

![Image of resources organized by department](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/2-department-rg.png)

We could even use a combination of these strategies and organize by environment and department. Put production finance resources in one resource group, dev finance resources in another, and the same for the marketing resources.

![Image of resources organized by environment and department](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/2-env-dept-rg.png)

There are a few factors that can play into the strategy you use to organize resources: authorization, resource life cycle, and billing.

#### Organizing for authorization

Since resource groups are a scope of RBAC, you can organize resources by *who* needs to administer them. If your database administration team is responsible for managing all of your Azure SQL Database instances, putting them in the same resource group would simplify administration. You could give them the proper permissions at the resource group level to administer the databases within the resource group. Similarly, the database administration team could be denied access to the resource group with virtual networks, so they don't inadvertently make changes to resources outside the scope of their responsibility.

#### Organizing for life cycle

We mentioned earlier that resource groups serve as the life cycle for the resources within it. If you delete a resource group, you delete all the resources in it. Use this to your advantage, especially in areas where resources are more disposable, like non-production environments. If you deploy 10 servers for a project that you know will only last a couple of months, you might put them all in a single resource group. One resource group is easier to clean up than 10 or more resource groups.

#### Organizing for billing

Lastly, placing resources in the same resource group is a way to group them for usage in billing reports. If you're trying to understand how your costs are distributed in your Azure environment, grouping them by resource group is one way to filter and sort the data to better understand where costs are allocated.

## Summary

The bottom line is that you have flexibility in how to organize resources in your resource groups. Put some thought into it so that you have a coherent approach to how you use resource groups in your Azure environment.

------

## Next unit: Use tagging to organize resources

[Continue](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/3-use-tagging-to-organize-resources)


  







# Use tagging to organize resources

- 8 minutes

You've gone through your resources and moved them into resource groups that are more organized than before. But what if resources have multiple uses? How do you better search, filter, and organize these resources? Tags can be helpful as you look to improve organization of your Azure resources.

## What are tags?

Tags are name/value pairs of text data that you can apply to resources and resource groups. Tags allow you to associate custom details about your resource, in addition to the standard Azure properties a resource has:

- department (like finance, marketing, and more)
- environment (prod, test, dev),
- cost center
- life cycle and automation (like shutdown and startup of virtual machines).

A resource can have up to 15 tags. The name is limited to 512 characters for all types of resources except storage accounts, which have a limit of 128 characters. The tag value is limited to 256 characters for all types of resources. Tags aren't inherited from parent resources. Not all resource types support tags, and tags can't be applied to classic resources.

Tags can be added and manipulated through the Azure portal, Azure CLI, Azure PowerShell, Resource Manager templates, and through the REST API. For example, to add a resource tag to a virtual network using the Azure CLI, you could use the following command:

Azure CLICopy

```azurecli
az resource tag --tags Department=Finance \
       --resource-group msftlearn-core-infrastructure-rg \
       --name msftlearn-vnet1 \
       --resource-type "Microsoft.Network/virtualNetworks"
```

You can use Azure Policy to automatically add or enforce tags for resources your organization creates based on policy conditions that you define. For example, you could require that a value for the Department tag is entered when someone in your organization creates a virtual network in a specific resource group.

## Apply tags to resources

Let's apply some tags to the resources you created. Recall that we created a resource group **msftlearn-core-infrastructure-rg** and two VNets inside that resource group, **msftlearn-vnet1** and **msftlearn-vnet2**. The names of the VNets are relatively generic, so we'd like to associate the VNets with services from different departments.

1. Go ahead and pull up the [Azure portal ](https://portal.azure.com/). Navigate to your **msftlearn-core-infrastructure-rg** resource group.

2. On the **Overview** tab of your resource group, you should see your two VNets listed. The default view doesn't display the tags column, so let's add that to the display. Select **Edit columns** at the top. In the **Available columns** list, select **Tags** and click **->** to add it to the **Selected columns** list. Click **Apply** to apply your changes.

   ![Image of portal showing how to add the tags column to the display](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/3-add-tag-column.png)

3. You should now see the tags column, but it will be empty since we haven't added any tags yet. We'll add the tags directly here. You can also add tags to any resource that supports it on the resource's **Tags** panel. In the list of resources, you should see a pencil in the **TAGS** column where you can directly edit the tags. Click the pencil for the **msftlearn-vnet1** resource.

4. This will display the dialog to edit the Tags. Let's add a couple tags to this VNet. In the **NAME** box type **Department**, and in the **VALUE** box type **Finance**. Click **Save** to save your changes, then click **Close** to close the dialog.

   ![Image of portal showing the dialog to add tags](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/3-add-tag-1.png)

5. Let's do the same steps for the **msftlearn-vnet2** VNet. For this VNet, add a **Department:Marketing** tag to the resource.

   You should now see your tags applied to each resource.

   ![Image of portal showing resources with tags](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/3-tags-displayed.png)

6. Let's add tags to both of these resources in bulk. Select the checkbox on the left for each of the VNets and click **Assign tags** in the top menu. By selecting multiple resources, we can add a tag to them in bulk, making it easy if we have multiple resources we want to apply the same tag to.

   Add the **Environment:Training** tag to the resources. You should see in the dialog that the tag will be applied to each of the VNets.

   ![Image of portal showing the dialog to add tags in bulk](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/3-add-bulk-tag.png)

   Back in the resource list you'll now see a **2** displayed as we now have two tags applied to each resource.

7. Let's take a look at how we can use tags to filter your resources. On the main Azure menu on the left, select **All resources**.

8. In the **All tags** drop down, under **Environment** select **Training**. You should see only your two VNets displayed, since we tagged those resources with the **Environment:Training** tag.

   ![Image of all resources filtered on the Training tag](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/3-all-resources-tag-filter.png)

9. We can further filter these resources by additionally filtering on the **Department:Finance** or **Department:Marketing**tags.

## Use tags for organization

The above example is just one example of where you can use tags to organize your resources. With their flexibility, there are several ways you can use tags to your advantage.

You can use tags to group your billing data. For example, if you're running multiple VMs for different organizations, use the tags to group usage by cost center. You can also use tags to categorize costs by runtime environment, such as the billing usage for VMs running in the production environment. When exporting billing data or accessing it through billing APIs, tags are included in that data and can be used to further slice your data from a cost perspective.

You can retrieve all the resources in your subscription with a specific tag name or value. Tags enable you to retrieve related resources from different resource groups. This approach is helpful when you need to organize resources for billing or management.

Tagging resources can also help in monitoring to track down impacted resources. Monitoring systems could include tag data with alerts, giving you the ability to know exactly who is impacted. In our example above, we applied the **Department:Finance** tag to the **msftlearn-vnet1** resource. If an alarm was thrown on **msftlearn-vnet1** and the alarm included the tag, we'd know that the finance department may be impacted by the condition that triggered the alarm. This contextual information can be valuable if an issue occurs.

It's also common for tags to be used in automation. If you want to automate the shutdown and startup of virtual machines in development environments during off-hours to save costs, you can use tags to assist in this. Add a **shutdown:6PM** and **startup:7AM** tag to the virtual machines, then create an automation job that looks for these tags, and shuts them down or starts them up based on the tag value. There are several solutions in the Azure Automation Runbooks Gallery that use tags in a similar manner to accomplish this.

------

## Next unit: Use policies to enforce standards

[Continue](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/4-use-policies-to-enforce-standards)


  









# Use policies to enforce standards

- 7 minutes

You're organizing your resources better in resource groups, and you've applied tags to your resources to use them in billing reports and in your monitoring solution. Resource grouping and tagging have made a difference in the existing resources, but how do you ensure that new resources follow the rules? Let's take a look at how policies can help you enforce standards in your Azure environment.

## What is Azure Policy?

Azure Policy is a service you can use to create, assign, and manage policies. These policies apply and enforce rules that your resources need to follow. These policies can enforce these rules when resources are created, and can be evaluated against existing resources to give visibility into compliance.

Policies can enforce things such as only allowing specific types of resources to be created, or only allowing resources in specific Azure regions. You can enforce naming conventions across your Azure environment. You can also enforce that specific tags are applied to resources. Let's take a look at how policies work.

## Create a policy

We'd like to ensure that all resources have the **Department** tag associated with them and block creation if it doesn't exist. We'll need to create a new policy definition and then assign it to a scope; in this case the scope will be our **mslearn-core-infrastructure-rg** resource group. Policies can be created and assigned through the Azure portal, Azure PowerShell, or Azure CLI. Let's walk through how to do create a policy in the portal.

### Create the policy definition

1. Go ahead and pull up the [Azure portal ](https://portal.azure.com/) in a web browser if you haven't already. In the search box in the top navigation bar, search for **Policy** and select the **Policy** service.

2. In **Authoring** section in the left menu, select **Definitions**.

3. You should see a list of built-in policies that you can use. In this case, we're going to create our own custom policy. Click **+ Policy definition** in the top menu.

4. This brings up the **New policy definition** dialog. To set the **Definition location**, click the blue **...**. Select the subscription for the policy to be stored in, which should be the same subscription as our resource group. Click **Select**.

5. Back on the **New policy definition** dialog, for **Name** give your policy a name of **Enforce tag on resource**.

6. For the **Description**, enter **This policy enforces the existence of a tag on a resource.**

7. For **Category** select **Use existing** and then select the **General** category.

8. For the **Policy rule**, delete all text in the box and paste in the following JSON.

   JSONCopy

   ```json
   {
     "mode": "indexed",
     "policyRule": {
       "if": {
         "field": "[concat('tags[', parameters('tagName'), ']')]",
         "exists": "false"
       },
       "then": {
         "effect": "deny"
       }
     },
     "parameters": {
       "tagName": {
         "type": "String",
         "metadata": {
           "displayName": "Tag Name",
           "description": "Name of the tag, such as 'environment'"
         }
       }
     }
   }
   ```

   Your policy definition should look like below. Click **Save** to save your policy definition.

   ![Image of the portal showing the new policy definition dialog](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/4-policy-definition.png)

### Create a policy assignment

We've created the policy, but we haven't actually put it into effect yet. To enable the policy, we need to create an assignment. In this case, we'll assign it to the scope of our **msftlearn-core-infrastructure-rg** resource group, so that it applies to anything inside the resource group.

1. In the policy pane, in the **Authoring** section on the left, select **Assignments**.
2. Select **Assign policy** at the top.
3. In the **Assign policy** pane, we'll assign our policy to our resource group. For **Scope**, click the blue **...**. Select your subscription and the **msftlearn-core-infrastructure-rg** resource group, then click **Select**.
4. For **Policy definition**, click the blue **...**. In the **Type** drop-down, select **Custom**, select the **Enforce tag on resource**policy you created, then click **Select**.
5. In the **Parameters** section, for **Tag name** enter **Department**. Click **Assign** to assign the policy.

### Test out the policy

Now that we have assigned the policy to our resource group, any attempts to create a resource without the **Department**tag should fail. Let's try this out.

1. Click **+ Create a resource** in the top left of the portal.

2. Search for **Storage Account** and select **Storage account** in the results. Click **Create**.

3. Select your subscription, and the **msftlearn-core-infrastructure-rg** resource group.

4. For **Storage account name**, give it any name of your choice, but note that it does have to be a globally unique name.

5. Leave the rest of the options at their default, click **Review + create**.

   Validation of your resource creation will fail because we don't have a **Department** tag applied to the resource.

    Important

   Please note that the assignment may take up to 30 minutes to take effect. Because of this delay, you may see it pass the validation, but fail the deployment. If this happens, allow for additional time and retry your deployment.

   ![Image of the portal showing a violation of policy](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/4-policy-violation.png)

   Let's fix the violation so we can successfully deploy the storage account.

6. Select **Tags** at the top of the **Create storage account** pane.

7. Add a **Department:Finance** tag to the list.

   ![Image of the portal showing a new Department tag](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/4-add-department-tag.png)

8. Now click **Review + create**. Validation should now pass, and if you click **Create** your storage account will be created.

## Use policies to enforce standards

We've seen how we could use policies to ensure that our resources have the tags that organize our resources. There are other ways policies can be used to our benefit.

We could use policy to restrict which Azure regions we can deploy resources to. For organizations that are heavily regulated or have legal or regulatory restrictions on where data can reside, policies help to ensure that resources aren't provisioned in geographic areas that would go against these requirements.

We could use policy to restrict which types of virtual machine sizes can be deployed. You may want to allow large VM sizes in your production subscriptions, but maybe you'd like to ensure that you keep costs minimized in your dev subscriptions. By denying the large VM sizes through policy in your dev subscriptions, you can ensure they don't get deployed in these environments.

We could also use policy to enforce naming conventions. If our organization has standardized on specific naming conventions, using policy to enforce the conventions helps us to keep a consistent naming standard across our Azure resources.

------

## Next unit: Secure resources with role-based access control

[Continue](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/5-role-based-access)









# Secure resources with role-based access control

- 5 minutes

Implementing Azure Policy ensured that all our employees with Azure access are following our internal standards for creating resources, but we have a second issue we need to solve: how do we protect those resources once they are deployed? We have IT personnel that need to manage settings, developers that need to have read-only access, and administrators that need to be able to control them completely. Enter Role-Based Access Control (RBAC).

RBAC provides fine-grained access management for Azure resources, enabling you to grant users the specific rights they need to perform their jobs. RBAC is considered a core service and is included with all subscription levels at no cost.

Using RBAC, you can:

- Allow one user to manage VMs in a subscription, and another user to manage virtual networks.
- Allow a database administrator (DBA) group to manage SQL databases in a subscription.
- Allow a user to manage all resources in a resource group, such as VMs, websites, and virtual subnets.
- Allow an application to access all resources in a resource group.

To view access permissions, use the **Access Control** (IAM) blade in the Azure portal. On this blade, you can see who has access to an area and their role. Using this same blade, you can also grant or remove access.

![Screenshot of the Access control - Role assignment blade. In the Access control (IAM) pane, settings, and permissions for a user display](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/5-resource-group-access-control.png)

In the above screenshot, **Alain Charon** has been assigned the **Backup Operator** role for this resource group.

### How RBAC defines access

RBAC uses an **allow model** for access. When you are assigned to a role, RBAC *allows* you to perform specific actions, such as read, write, or delete. Therefore, if one role assignment grants you read permissions to a resource group, and a different role assignment grants you write permissions to the same resource group, you will have write permissions on that resource group.

## Best Practices for RBAC

Here are some best practices you should use when setting up resources.

- Segregate duties within your team and grant only the amount of access to users that they need to perform their jobs. Instead of giving everybody unrestricted permissions in your Azure subscription or resources, allow only specific actions at a particular scope.
- When planning your access control strategy, grant users the lowest privilege level that they need to do their work.
- Use **Resource Locks** to ensure critical resources aren't modified or deleted (more on that next!)

------

## Next unit: Use resource locks to protect resources

[Continue](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/6-use-resource-locks-to-protect-resources)









# Use resource locks to protect resources

- 7 minutes

In a recent conversation, your manager mentioned that there had been instances where critical Azure resources had been mistakenly deleted. Since there was disorganization across their Azure environment, some good intentions of cleaning up unnecessary resources resulted in accidental deletion. You've heard of resource locks on Azure. You mention to your manager that you think you can help prevent this type of incident from happening in the future. Let's take a look at how you could use resource locks to solve this problem.

## What are resource locks?

Resource locks are a setting that can be applied to any resource to block modification or deletion. Resource locks can set to either **Delete** or **Read-only**. Delete will allow all operations against the resource but block the ability to delete it. **Read-only** will only allow read activities to be performed against it, blocking any modification or deletion of the resource. Resource locks can be applied to subscriptions, resource groups, and to individual resources, and are inherited when applied at higher levels.

 Note

Applying **Read-only** can lead to unexpected results because some operations that seem like read operations actually require additional actions. For example, placing a Read-only lock on a storage account prevents all users from listing the keys. The list keys operation is handled through a POST request because the returned keys are available for write operations.

When a resource lock is applied, you must first remove the lock in order to perform that activity. By putting an additional step in place before allowing the action to be taken on the resource, it helps protect resources from inadvertent actions, and helps protect your administrators from doing something they may not have intended to do. Resource locks apply regardless of RBAC permissions. Even if you are an owner of the resource, you must still remove the lock before you'll actually be able to perform the blocked activity.

Let's take a look at how a resource lock works in action.

## Create a resource lock

Recall our **msftlearn-core-infrastructure-rg** resource group. We've now got two VNets and a storage account in them. We consider these resources to be critical pieces of our Azure environment, and want to ensure that they aren't mistakenly deleted. Let's apply a resource lock to the resource group to prevent the resource group and its contained resources from being deleted.

1. Go ahead and pull up the [Azure portal ](https://portal.azure.com/) in a web browser if you haven't already. In the search box in the top navigation bar, search for **msftlearn-core-infrastructure-rg** and click on the resource group.

2. In the **Settings** section in the left menu, select **Locks**. You should see that the resource currently has no locks. Let's add one.

3. Click **+ Add**. Name the lock **BlockDeletion** and select a **Lock type** of **Delete**. Click **OK**.

   ![Image of the portal showing a new resource lock being configured](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/6-add-lock.png)

   You now have a lock applied to the resource group that will prevent deletion of the resource group, and is inherited by all resources within the resource group. Let's try to delete one of the VNets to see what happens.

4. Go back to **Overview**, and click on **msftlearn-vnet1** to view the resource.

5. In the **Overview** pane for **msftlearn-vnet1**, click **Delete** at the top, then **Yes** to confirm. You should receive an error, stating that there is a lock on the resource preventing its deletion.

   ![Image of error showing resource is blocked from deletion](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/media/6-delete-error.png)

6. In the **Settings** section in the left menu, select **Locks**. You should see here that our **msftlearn-vnet1** has a lock that is inherited by from the resource group.

7. Navigate back to the **msftlearn-core-infrastructure-rg** resource group, and bring up the **Locks** pane. Let's remove our lock so we can clean up. Click the **...** on the **BlockDeletion** lock and select **Delete**.

## Using resource locks in practice

We've seen how resource locks can protect from accidental deletion. In order to delete the virtual network, we needed to remove the lock. This concerted action helps ensure that you really intend to delete or modify the resource in question.

Use resource locks to protect those key pieces of Azure that could have a large impact if they were removed or modified. Some examples are ExpressRoute circuits, and virtual networks, critical databases, and domain controllers. Evaluate your resources, and apply locks where you'd like to have an extra layer of protection from accidental actions.

------

## Next unit: Check your Knowledge

[Continue](https://docs.microsoft.com/en-us/learn/modules/control-and-organize-with-azure-resource-manager/7-quiz)


  





# Summary

- 2 minutes

We've taken a look at several features you can use to put organization and control around your Azure resources.

We talked about how resource groups worked, and some ways you can use them to organize your resources.

We looked at how tags allow you to add custom contextual information to your resources, for use in areas such as billing and filtering.

We saw how we could use policies to enforce standards across our Azure resources.

We used resource locks to prevent accidental deletion of critical resources.

By using these tools throughout your Azure environment, you'll have greater organization across your Azure resources.

## Clean up

Let's clean up the resources that we created. Since we deployed everything in a single resource group, cleaning up is easy.

1. Go ahead and pull up the [Azure portal ](https://portal.azure.com/) in a web browser if you haven't already. In the search box in the top navigation bar, search for **msftlearn-core-infrastructure-rg** and click on the resource group.
2. In the **Overview** pane, click **Delete resource group**. Enter the **msftlearn-core-infrastructure-rg** resource group name to confirm, and click **Delete**.

------

## Module complete:









# PART 12: Predict costs and optimize spending for Azure

# Introduction

- 2 minutes

When planning a solution in the cloud, there's always the challenge of balancing cost against performance. It can feel like a guessing game whether your selected options will stay within budget or if you'll have a surprise on your next bill.

You need to be able to confidently answer several questions:

- What will this solution cost this fiscal year?
- Is there an alternate configuration you could use to save money?
- Can you estimate how a change would impact your cost and performance *without* putting it into a production system?

In this module, we'll explore the tools you can use to answer these questions and more.

## Learning objectives

In this module, you will:

- Learn the different options you have to purchase Azure services
- Estimate costs with the Azure pricing calculator
- Predict and optimize costs with Azure Cost Management and Azure Advisor
- Apply best practices for saving on infrastructure costs
- Apply best practices for saving on licensing costs

------

## Next unit: Purchasing Azure products and services

[Continue](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/1a-purchasing-products)









# Purchasing Azure products and services

- 5 minutes

Let's start by examining the purchasing options you have with Azure. There are three main customer types on which the available purchasing options for Azure products and services are contingent, including:

- **Enterprise** - Enterprise customers sign an Enterprise Agreement with Azure that commits them to spend a negotiated amount on Azure services, which they typically pay annually. Enterprise customers also have access to customized Azure pricing.
- **Web direct** - Direct Web customers pay general public prices for Azure resources, and their monthly billing and payments occur through the Azure website.
- **Cloud Solution Provider** - Cloud Solution Provider (CSP) typically are Microsoft partner companies that a customer hires to build solutions on top of Azure. Payment and billing for Azure usage occur through the customer's CSP.

Products and services in Azure are arranged by category, which has various resources that you can provision. You select the Azure products and services that fit your requirements, and your account is billed according to Azure's pay-for-what-you-use model.

![Depiction of the various Azure products with the Featured products selection highlighted, displaying names and short descriptions of those products](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/media/1a-azure-products-overview.png)

### Usage meters

When you provision an Azure resource, Azure creates one or more meter instances for that resource. The meters track the resources' usage, and generate a usage record that is used to calculate your bill.

For example, a single virtual machine that you provision in Azure might have the following meters tracking its usage:

- Compute Hours
- IP Address Hours
- Data Transfer In
- Data Transfer Out
- Standard Managed Disk

- Standard Managed Disk Operations
- Standard IO-Disk
- Standard IO-Block Blob Read
- Standard IO-Block Blob Write
- Standard IO-Block Blob Delete

The meters and pricing vary per product and often have different pricing tiers based on the size or capacity of the resource. Check the documentation for specific details on what each service area costs.

At the end of each monthly billing cycle, the usage values will be charged to your payment method and the meters are reset. You can check the billing page in the Azure portal at any time to get a quick summary of your current usage and see any invoices from past billing cycles.

The key takeaway is that resources are always charged *based on usage*. For example, if you de-allocate a VM then you will not be billed for compute hours, I/O reads or writes or the private IP address since the VM is not running and has no allocated compute resources. However you will incur storage costs for the disks.

 Note

De-allocating a VM is not the same as *deleting* a VM. De-allocation means the VM is not assigned to a CPU or network in a datacenter. However, your persistent disks remain, and the resource is present in your subscription. It's similar to turning off your physical computer.

------

## Next unit: Factors affecting costs

[Continue](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/1b-factors-affecting-cost)









# Factors affecting costs

- 5 minutes

Just like your on-premises equipment costs, there are several elements that will affect your monthly costs when using Azure services. Let's look at a few of the primary factors including resource type, services, the user's location, and the billing zone.

### Resource type

Costs are resource-specific, so the usage that a meter tracks and the number of meters associated with a resource depend on the resource type.

 Note

Each meter tracks a *particular kind of usage*. For example, a meter might track bandwidth usage (ingress or egress network traffic in bits-per-second), the number of operations, size (storage capacity in bytes), or similar items.

The usage that a meter tracks correlates to a number of billable units. Those are charged to your account for each billing period, and the rate per billable unit depends on the resource type you are using.

### Services

Azure usage rates and billing periods can differ between Enterprise, Web Direct, and Cloud Solution Provider (CSP) customers. Some subscription types also include usage allowances, which affect costs.

The Azure team develops and offers first-party products and services, while products and services from third-party vendors are available in the [Azure Marketplace ](https://azuremarketplace.microsoft.com/). Different billing structures apply to each of these categories.

![Image depicting a billing period, with a calendar, computer, and meter linked to illustrate the correlation between the three](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/media/2b-billing-period-graphic.png)

### Location

Azure has datacenters all over the world. Usage costs vary between locations that offer particular Azure products, services, and resources based on popularity, demand, and local infrastructure costs.

For example, you might want to build your Azure solution by provisioning resources in locations that offer the lowest prices, but this would require transferring data between locations if dependent resources and their users are located in different parts of the world. If there are meters tracking the volume of data that moves between the resources you provision, any potential savings you make from choosing the cheapest location could be offset by the additional cost of transferring data between those resources.

### Azure billing zones

Bandwidth refers to data moving in and out of Azure datacenters. Most of the time inbound data transfers (data going *into* Azure datacenters) are free. For outbound data transfers (data going *out* of Azure datacenters), the data transfer pricing is based on **Billing Zones**.

![Image that shows internet traffic traveling between two datacenters around a globe](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/media/1b-azure-regions-globe.png)

A **Zone** is a geographical grouping of Azure Regions for billing purposes. The following zones exist and include the listed countries (regions) listed.

| Zone      | Areas                                        |
| :-------- | :------------------------------------------- |
| Zone 1    | United States, Europe, Canada, UK, France    |
| Zone 2    | Asia Pacific, Japan, Australia, India, Korea |
| Zone 3    | Brazil                                       |
| DE Zone 1 | Germany                                      |

In most zones, the first outbound 5 GB per month is free. After that, you are billed a fixed price per GB.

 Note

Billing zones aren't the same as an *Availability Zone*. In Azure, the term *zone* is for billing purposes only, and the full term *Availability Zone* refers to the failure protection that Azure provides for datacenters.

------

## Next unit: Estimate costs with the Azure pricing calculator

[Continue](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/2-estimate-costs-with-the-azure-pricing-calculator)


  





# Estimate costs with the Azure pricing calculator

- 15 minutes

Imagine that you've been asked to build a system on Azure, and you've been asked for an estimate of what it might cost to run over the next 12 months. You already know that Azure pricing is fully transparent and that you're billed monthly for only the services that you use. How would you get that estimate without deploying and running those services or without manually pricing out each service from the Azure service pricing pages?

## Introducing the Azure pricing calculator

To make estimates easy for customers to create, Microsoft developed the **Azure pricing calculator**. The Azure pricing calculator is a free web-based tool that allows you to input Azure services and modify properties and options of the services. It outputs the costs per service and total cost for the full estimate.

The options that you can configure in the pricing calculator vary between products, but basic configuration options include:

| Option                 | Description                                                  |
| :--------------------- | :----------------------------------------------------------- |
| Region                 | Lists the regions from which you can provision a product. Southeast Asia, central Canada, the western United States, and Northern Europe are among the possible regions available for some resources. |
| Tier                   | Sets the type of tier you wish to allocate to a selected resource, such as Free Tier, Basic Tier, etc. |
| Billing Options        | Highlights the billing options available to different types of customer and subscriptions for a chosen product. |
| Support Options        | Allows you to pick from included or paid support pricing options for a selected product. |
| Programs and Offers    | Allows you to choose from available price offerings according to your customer or subscription type. |
| Azure Dev/Test Pricing | Lists the available development and test prices for a product. Dev/Test pricing applies only when you run resources within an Azure subscription that is based on a Dev/Test offer. |

### Try out the Azure pricing calculator

In another browser window or tab, open the [Azure pricing calculator](https://azure.microsoft.com/pricing/calculator/). On the pricing calculator page, you'll see three tabs:

1. **Products.** This tab is where you'll do most of your activity. This tab has all the Azure services listed and is where you'll add or remove services to put together your estimate.
2. **Estimates.** This tab has all of your previously saved estimates. We'll go through this process in a moment.
3. **FAQ.** Just as it says, this tab has answers to some frequently asked questions.

Let's start with the **Products** tab. You'll see the full listing of service categories down the left-hand side. Clicking on any of the categories will display the services in that category. There's also a search box where you can search through all services for the service you're looking for. Clicking on the service will add that service to your estimate. You can add just one service, or you can add as many as you need, including multiples of the same service (for example, multiple virtual machines).

After you've added the services, you'll want to price them. Scrolling down on the page will show you customizable details for that service that apply to pricing. For example, on virtual machines, you can select details such as the region, operating system, and instance size, all of which will impact the pricing for the VM. You'll see a subtotal for the service. And scrolling further down, you'll see a full total for all services included in the estimate. Along with the total, you'll see buttons where you can export, save, and share the estimate.

## Estimate a solution

From our original scenario, let's imagine that this system will run on two Azure VMs and will connect to an Azure SQL Database instance. We also want to have a layer 7 firewall in place to ensure we have enhanced load-balancing capabilities. The following illustration shows an application gateway connected to two virtual machines that are connected to a single Azure SQL Database instance.

![An illustration of a sample architecture that will be used as an example to demonstrate estimating costs.](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/media/2-estimate-costs-architecture.png)

We can use the Azure pricing calculator to figure out what the solution will cost and export our estimate to share with the team.

 Tip

Make sure you have a clean calculator with nothing listed in the estimate. If you have anything present in your estimate, click the trash can icon on each item to reset the estimate.

In the Azure pricing calculator, on the **Products** tab, add the following services to the estimate by clicking on them:

- Virtual Machines in the Compute category
- Azure SQL Database in the Databases category
- Application Gateway in the Networking category

We can configure the details of each, on the **Estimates** tab, to get a solid estimate of our costs. Use the **West US** region for all resources.

- **Virtual Machines.** This is an ASP.NET application, so we'll need to use a **Windows OS** VM. This application doesn't require a massive amount of computing power, so select the **D2 v3** instance size. We'll need two virtual machines, and they will run all the time (730 hours/month). We're going to use standard SSD storage for these VMs and will require just one disk per VM of size **E10**, for a total of two disks.
- **SQL Database.** For the database, we're going to provision a **single database type** using the **vCore model**. We want a General Purpose, Gen 5 database with 8 vCores. We'll need 32 GB of storage.
- **Application Gateway.** For Application Gateway, we're going to use the Web Application Firewall tier, so we have some protection for our environment. And we're going to go with just two instances and medium size, as our load isn't going to be high. We expect to process 1 TB of data per month. We don't expect to process any data in Europe (Zone 1).

Looking through your estimate, you should see a summary cost for each service you've added and a full total for the entire estimate. In this case, your estimate should be around **$2,100.00 per month**. You can try playing with some of the options - particularly the *location* you place these resources in to see the estimate go up and down.

 Tip

If you have resources that are not location-sensitive, you can save a lot of money by locating them in less expensive regions. Checking the pricing calculator can help you determine the most cost-effective place to put these services.

## Share and save your estimate

We now have an estimate for our solution. We can save this estimate, so we can come back to it later and adjust it if necessary. We can also export it to Excel for further analysis or share the estimate via a URL.

To export the estimate, click `Export` at the bottom of the estimate. This will download your estimate in Excel (**.xlsx**) format and will include all the services you added to your estimate.

We can either share the Excel spreadsheet, or we can click on the `Share` button in the calculator. This gives you a URL that you can use to share this estimate. Anyone with this link will be able to access it, making it easy to share with your team.

If you are logged in with your Azure account, you can save the estimate, so you can come back to it later. Go ahead and click the **Save** button. If you are signed in, you should see a notification that your estimate was saved. If you aren't signed in, you'll see a message to sign in to save your estimate. After you've saved the estimate, scroll back up to the top of the page and select the **Estimates** tab. You will see your estimate there. You can then select it to pull it back up or delete it if you no longer need it.

We have arrived at a cost estimate for a set of Azure services without spending any money. We didn't create anything, and we have a fully sharable estimate that we can do further analysis or modifications on in the future. You can use this not only to create estimates for systems where you know the specific services you plan to use but also to compare how different services might impact your overall costs. An example is Microsoft SQL Server on a VM vs. Azure SQL Database.

## Check your knowledge

\1. 

Which tab of the Azure pricing calculator will you use to put together your estimate?



Estimate



Products

\2. 

True or false: You can share your estimate through an Excel spreadsheet or through a URL.



True



False











# Predict and optimize with Cost Management and Azure Advisor

- 15 minutes

We learned how to estimate your costs before you deploy services on Azure, but what if you already have resources deployed? How do you get visibility into the costs you're already accruing? If we had deployed our previous solution to Azure and now want to make sure that we've sized the virtual machines properly and predict how much our bill will be, how can we do this? Let's look at a few tools on Azure that you can use to help you solve this problem.

## What is Azure Advisor?

**Azure Advisor** is a free service built into Azure that provides recommendations on high availability, security, performance, and cost. Advisor analyzes your deployed services and looks for ways to improve your environment across those four areas. We'll focus on the cost recommendations, but you'll want to take some time to review the other recommendations as well.

Advisor makes cost recommendations in the following areas:

1. **Reduce costs by eliminating unprovisioned Azure ExpressRoute circuits.** This identifies ExpressRoute circuits that have been in the provider status of *Not Provisioned* for more than one month and recommends deleting the circuit if you aren't planning to provision the circuit with your connectivity provider.
2. **Buy reserved instances to save money over pay-as-you-go.** This will review your virtual machine usage over the last 30 days and determine if you could save money in the future by purchasing reserved instances. Advisor will show you the regions and sizes where you potentially have the most savings and will show you the estimated savings you might achieve from purchasing reserved instances.
3. **Right-size or shutdown underutilized virtual machines.** This monitors your virtual machine usage for 14 days and then identifies underutilized virtual machines. Virtual machines whose average CPU utilization is 5 percent or less and network usage is 7 MB or less for four or more days are considered underutilized virtual machines. The average CPU utilization threshold is adjustable up to 20 percent. By identifying these virtual machines, you can decide to resize them to a smaller instance type, reducing your costs.

 Note

If you don't have an Azure subscription, create a [free account ](https://azure.microsoft.com/free/) before you begin.

Let's take a look at where you can find Azure Advisor in the portal.

1. Sign into the [Azure portal ](https://portal.azure.com/) using your Microsoft account.
2. Click on **All Services**, and in the **Management Tools** category, you will see **Advisor**. You can also type `Advisor` in the filter box to filter on just that service.
3. Click on Advisor, and you'll be taken to the Advisor recommendations dashboard where you can see all the recommendations for your subscription. You'll see a box for each category of recommendations.

 Note

You might not have any recommendations on cost in Advisor. This could be because assessments have not yet completed or simply because Advisor has no recommendations.

![Screenshot of the Azure portal showing the Advisor blade with four category boxes for Advisor recommendations: high availability, security, performance, and cost.](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/media/3-advisor-recommendations.png)

Clicking on the **Cost** box will take you to detailed recommendations where you can see the recommendations that Advisor has.

![Screenshot of the Azure portal showing the cost recommendations portion of the Advisor blade.](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/media/3-advisor-cost-recommendations.png)

Clicking on any recommendation will take you to the details for that specific recommendation. Then you'll be able to take a specific action, such as resizing virtual machines to reduce spending.

![Screenshot of the Azure portal showing recommendation details on the Shut down or resize your virtual machine recommendation.](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/media/3-advisor-resize-vm.png)

These recommendations are all places where you might be inefficiently spending money. They're a great place to start and continue to revisit when looking for places to reduce costs. In our example, there's an opportunity for us to save around $700 per month if we take these recommendations. This savings adds up, so be sure to review this periodically for recommendations across all four areas.

## Azure Cost Management

Azure Cost Management is another free, built-in Azure tool that can be used to gain greater insights into where your cloud money is going. You can see historical breakdowns of what services you are spending your money on and how it is tracking against budgets that you have set. You can set budgets, schedule reports, and analyze your cost areas.

![Screenshot of the Azure portal showing the Cost analysis section of the Cost Management + Billing blade.](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/media/3-cost-management.png)

## Cloudyn

Cloudyn, a Microsoft subsidiary, allows you to track cloud usage and expenditures for your Azure resources and other cloud providers including Amazon Web Services and Google. Easy-to-understand dashboard reports help with cost allocation and chargebacks. Cost Management helps optimize your cloud spending by identifying underutilized resources that you can then manage and adjust. Usage for Azure is free, and there are paid options for premium support and to view data from other clouds.

![Screenshot of the Azure portal showing the Cloudyn management dashboard.](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/media/3-cloudyn-mgt-dash.png)

As you can see, there are several tools available for no cost on Azure that you can use to track and predict your cloud spend and identify where your environment may be inefficient from a cost perspective. You'll want to make sure you make it a regular practice to review the reports and recommendations that these tools make available, so you can unlock savings across your cloud footprint.

## Check your knowledge

\1. 

True or false: Azure Advisor provides recommendations on cost only.



True



False

\2. 

Azure Cost Management allows you to _________.



See historical breakdowns of what services you are spending your money on.



See estimates of what your services might cost if you make a change.









# Estimate the Total Cost of Ownership with the Azure TCO calculator

- 8 minutes

The pricing calculator and cost management advisor can help you predict and analyze your spend for new or existing services.

If you are starting to migrate to the cloud, a useful tool you can use to predict your cost savings is the **Total Cost of Ownership** (TCO) calculator. To use the TCO calculator, you need to complete four steps.

### Step 1: Open the TCO calculator

Start by opening the [Total Cost of Ownership calculator ](https://azure.microsoft.com/pricing/tco/) website.

### Step 2: Define your workloads

Start by entering details about your on-premises infrastructure into the TCO calculator according to four groups:

| Group      | Description                                                  |
| :--------- | :----------------------------------------------------------- |
| Servers    | Enter details of your current on-premises server infrastructure. |
| Databases  | Enter details of your on-premises database infrastructure in the *Source* section. In the *Destination* section, select the corresponding Azure service you would like to use. |
| Storage    | Enter the details of your on-premises storage infrastructure. |
| Networking | Enter the amount of network bandwidth you currently consume in your on-premises environment. |

### Step 3: Adjust assumptions

Adjust the values of assumptions that the TCO calculator makes, which might vary between customers. To improve the accuracy of the TCO calculator, you should adjust the values, so they match the costs of your current on-premises infrastructure. The assumptions you can customize include:

- Storage costs
- IT labor costs
- Hardware costs
- Software costs
- Electricity costs
- Virtualization costs
- Datacenter costs
- Networking costs
- Database costs

### Step 4: View the report

The TCO calculator generates a detailed report based on the details you enter and the adjustments you make. The report allows you to compare the costs of your on-premises infrastructure with the costs of using Azure products and services to host your infrastructure in the cloud.

![Depicts two TCO pie charts. One for total on-premises cost of $30,702,495 and one for Azure cost of $595,618](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/media/3a-tco-calculator-report.png)

------

## Next unit: Save on infrastructure costs

[Continue](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/4-save-on-infrastructure-costs)









# Save on infrastructure costs

- 10 minutes

We have seen how to create cost estimates for environments you'd like to build, walked through some tools to get details on where we're spending money, and projected future expenses. Our next challenge is to look at how to reduce those infrastructure costs.

## Use Azure credits

Visual Studio subscribers can activate a monthly credit benefit which allows you to experiment with, develop, and test new solutions on Azure. Use Azure credits to try out new services such as App Service, Windows 10 VMs, Azure SQL Server databases, Containers, Cognitive Services, Functions, Data Lake, and more without incurring any monetary costs.

When you activate this benefit, you will own a separate Azure subscription under your account with a monthly credit balance that renews each month while you remain an active Visual Studio subscriber.

The credit amount varies based on the program level - $50/month for VS Professional and $150/month for Enterprise. Check the documentation for more details on how much credit you receive for your specific subscription level.

 Important

The monthly Azure credit for Visual Studio subscribers is for **development and testing only** and does not carry a financially-backed SLA. Azure will suspend any instance (VM or cloud service) that runs continuously for more than 120 hours or if it's determined that the instance is being used for production. This benefit is made available to Visual Studio subscribers on a best efforts basis; there is no guarantee of capacity availability.

## Use spending limits

By default, Azure subscriptions which have associated monthly credits (which includes trial accounts) have a *spending limit*to ensure you aren't charged once you have used up your credits. This feature is useful for development teams exploring new solution architectures as it ensures you won't have an unexpectedly large bill at the end of the month.

 Note

Azure spending limits are not the same as Subscription, Service, or Resource Group limits and quotas.

Azure provides the Spending Limits feature to help prevent you from exhausting the credit on your account within each billing period. When your Azure usage results in charges that use all the included monthly credit, the services that you deployed are disabled and turned off for the rest of that billing period. Once a new billing period starts, assuming there are credits available, the resources are re-activated and deployed.

You are notified by email when you hit the spending limit for your subscription. In addition, the Azure portal includes notifications about your credit spend. You can adjust the spending limit as desired or even turn it off.

 Important

The spending limit feature is specific to subscriptions that include a monthly Azure credit allotment. It is not available on pay-only subscriptions.

## Use reserved instances

If you have VM workloads that are static and predictable, particularly ones that run 24x7x365, using reserved instances is a fantastic way to potentially save up to 70-80%, depending on the VM size. The following illustration shows that using Azure reserved instances saves you up to 72% and using reserved instance plus Azure Hybrid Benefit saves up to 80% in costs.

![An illustration showing cost benefits of using Azure reserved instances and Azure Hybrid Benefits compared to pay-as-you-go.](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/media/4-savings-coins.png)

Reserved instances are purchased in one-year or three-year terms, with payment required for the full term up front. After it's purchased, Microsoft matches up the reservation to running instances and decrements the hours from your reservation. Reservations can be purchased through the Azure portal. And because reserved instances are a compute discount, they are available for both Windows and Linux VMs.

## Choose low-cost locations and regions

The cost of Azure products, services, and resources can vary across locations and regions, and if possible, you should use them in those locations and regions where they cost less.

 Note

Some resources are metered and billed according to how much outgoing network bandwidth they consume (egress). You should provision connected resources that are bandwidth metered *in the same region* to reduce egress traffic between them.

## Research available cost-saving offers

Keep up-to-date with the latest Azure customer and subscription offers, and switch to offers that provide the most significant cost-saving benefit.

You can check the [Azure Updates page](https://azure.microsoft.com/updates/) for information about the latest updates to Azure products, services, and features, as well as product roadmaps and announcements.

## Right-size underutilized virtual machines

Recall from our previous discussion that Azure Cost Management and Azure Advisor might recommend right-sizing or shutting down VMs. Right-sizing a virtual machine is the process of resizing it to a proper size. Let's imagine you have a server running as a domain controller that is sized as a **Standard_D4sv3**, but your VM is sitting at 90% idle the vast majority of the time. By resizing this VM to a **Standard_D2sv3**, you reduce your compute cost by 50%. Costs are linear and double for each size larger in the same series. In this case, you might even benefit from changing the instance series to go to a less expensive VM series. The following illustration shows a 50% savings achieved by moving one size down within the same series.

![An illustration to demonstrate savings achieved by downsizing an under-utilized virtual machine.](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/media/4-vm-resize.png)

Over-sized virtual machines are a common unnecessary expense on Azure and one that can be easily fixed. You can change the size of a VM through the Azure portal, Azure PowerShell, or the Azure CLI.

 Tip

Resizing a VM requires it to be stopped, resized, and then restarted. This may take a few minutes depending on how significant the size change is. Plan for an outage, or shift your traffic to another instance while you perform this task.

## Deallocate virtual machines in off hours

If you have virtual machine workloads that are only used during certain periods, but you're running them every hour of every day, you're wasting money. These VMs are great candidates to shut down when not in use and start back up on a schedule, saving you compute costs while the VM is deallocated.

This approach is an excellent strategy for development environments. It's often the case that development may happen only during business hours, giving you the flexibility to deallocate these systems in the off hours and stopping your compute costs from accruing. Azure now has an [automation solution](https://docs.microsoft.com/azure/automation/automation-solution-vm-management) fully available for you to leverage in your environment.

You can also use the auto-shutdown feature on a virtual machine to schedule automated shutdowns.

![Screenshot of the Azure portal showing the Auto-shutdown section of a virtual machine blade with a shutdown time enabled.](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/media/4-vm-auto-shutdown.png)

## Delete unused virtual machines

This advice may sound obvious, but if you aren't using a service, you should shut it down. It's not uncommon to find non-production or proof-of-concept systems left around following a project that is no longer needed. Regularly review your environment and work to identify these systems. Shutting down these systems can have a multifaceted benefit by saving you not only on infrastructure costs but also potential savings on licensing and operations.

## Migrate to PaaS or SaaS services

Lastly, as you move workloads to the cloud, a natural evolution is to start with infrastructure-as-a-service (IaaS) services and then move them to platform-as-a-service (PaaS) as appropriate, in an iterative process.

PaaS services typically provide substantial savings in both resource and operational costs. The challenge is that depending on the type of service, varying levels of effort will be required to move to these services from both a time and resource perspective. You might be able to move a SQL Server database to Azure SQL Database easily, but it might take substantially more effort to transfer your multi-tier application to a container or serverless-based architecture. It's a good practice to continuously evaluate the architecture of your applications to determine if there are efficiencies to be gained through PaaS services.

Azure makes it easy to test these services with little risk, giving you the ability to try out new architecture patterns relatively easily. That said, it's typically a longer journey and might not be of immediate help if you're looking for quick wins from a cost-savings perspective. The Azure Architecture Center is a great place to get ideas for transforming your application, as well as best practices across a wide array of architectures and Azure services.

## Check your knowledge

\1. 

Which one of these is *not* a cost-saving solution?



Deallocate virtual machines during off hours.



Use Azure Reserved Virtual Machine Instances.



Load balance your virtual machines for incoming messages.



Right-size underutilized virtual machines.

\2. 

True or false: PaaS is generally less expensive than IaaS.



True



False




  







# Save on licensing costs

- 10 minutes

Licensing is another area that can dramatically impact your cloud spending. Let's look at some ways you can reduce your licensing costs.

## Linux vs. Windows

Many of the Azure services you deploy have the choice of running on Windows or Linux. In some cases, the cost of the product can be different based on the OS you choose. Where you have a choice, and your application doesn't depend on the underlying OS, it's useful to compare pricing to determine whether you can save money.

## Azure Hybrid Benefit for Windows Server

Many customers have invested in Windows Server licenses and would like to repurpose this investment on Azure. The Azure Hybrid Benefit gives customers the right to use these licenses for virtual machines on Azure. That means you won't be charged for the Windows Server license and will instead be billed at the Linux rate.

To be eligible for this benefit, your Windows licenses must be covered by Software Assurance. The following guidelines will also apply:

- Each two-processor license or each set of 16-core licenses is entitled to two instances of up to 8 cores or one instance of up to 16 cores.
- Standard Edition licenses can only be used once either on-premises or in Azure. That means you can't use the same license for an Azure VM and a local computer.
- Datacenter Edition benefits allow for simultaneous usage both on-premises and in Azure so that the license will cover two running Windows machines.

 Note

Most customers are typically licensed by core, so you'll use that model for your calculation. If you have questions about what licenses you have, reach out to your license reseller or your Microsoft account team.

Applying the benefit is easy. It can be turned on and off at any time with existing VMs or applied at deployment time for new VMs. The Hybrid Benefit (especially when combined with reserved instances) can provide substantial license savings.

## Azure Hybrid Benefit for SQL Server

The Azure Hybrid Benefit for SQL Server helps you maximize the value from your current licensing investments and accelerate your migration to the cloud. Azure Hybrid Benefit for SQL Server is an Azure-based benefit that enables you to use your SQL Server licenses with active Software Assurance to pay a reduced rate.

You can use this benefit even if the Azure resource is active, but the reduced rate will only be applied from the time you select it in the portal. No credit will be issued retroactively.

### Azure SQL Database vCore-based options

For Azure SQL Database, the Azure Hybrid Benefit works as follows:

- If you have Standard Edition per core licenses with active Software Assurance, you can get one vCore in the General Purpose service tier for every one license core you own on-premises.
- If you have Enterprise Edition per core licenses with active Software Assurance, you can get one vCore in the Business Critical service tier for every one license core you own on-premises. Note that the Azure Hybrid Benefit for SQL Server for the Business Critical service tier is available only to customers who have Enterprise Edition licenses.
- If you have highly virtualized Enterprise Edition per core licenses with active Software Assurance, you can get four vCores in the General Purpose service tier for every one license core you own on-premises. This is a unique virtualization benefit available only on Azure SQL Database.

The following illustration shows the vCore-based options available in each service tier with Azure Hybrid Benefit for SQL Server licenses.

![An illustration showing an example of how to maximize your existing SQL server license value using the Azure Hybrid Benefit.](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/media/5-sql-tradein-value.png)

For SQL Server in Azure Virtual Machines, the Azure Hybrid Benefit works as follows:

- If you have Enterprise Edition per core licenses with active Software Assurance, you can get one core of SQL Server Enterprise Edition in Azure Virtual Machines for every one license core you own on-premises.
- If you have Standard Edition per core licenses with active Software Assurance, you can get one core of SQL Server Standard Edition in Azure Virtual Machines for every one license core you own on-premises.

This can make a dramatic impact on your Azure spending with SQL Server workloads.

## Use Dev/Test subscription offers

The [Enterprise Dev/Test](https://azure.microsoft.com/offers/ms-azr-0148p/) and [Pay-As-You-Go Dev/Test](https://azure.microsoft.com/offers/ms-azr-0023p/) offers are a benefit you can take advantage of to save costs on your non-production environments. This benefit gives you several discounts, most notably for Windows workloads, eliminating license charges and only billing you at the Linux rate for virtual machines. This also applies to SQL Server and any other Microsoft software that is covered under a Visual Studio subscription (formerly known as MSDN).

There are a few requirements for this benefit, one being that it's only for non-production workloads, and another being that any users of these environments (excluding testers) must be covered under a Visual Studio subscription. In short, for non-production workloads, this allows you to save money on your Windows, SQL Server, and other Microsoft virtual machine workloads.

Below are the full details of each offer. If you are a customer on an Enterprise Agreement, you'd want to leverage the Enterprise Dev/Test offer, and if you are a customer without an Enterprise Agreement and are instead using PAYG accounts, you'd leverage the Pay-As-You-Go Dev/Test offer.

## Bring your own SQL Server license

If you are a customer on an Enterprise Agreement and already have an investment in SQL Server licenses, and they have freed up as part of moving resources to Azure, you can provision **bring your own license** (BYOL) images off the Azure Marketplace, giving you the ability to take advantage of these unused licenses and reduce your Azure VM cost. You've always been able to do this by provisioning a Windows VM and manually installing SQL Server, but this simplifies the creation process by leveraging Microsoft certified images. Search for **BYOL** in the Marketplace to find these images.

![Screenshot of the Azure portal showing BYOL options for SQL Server.](https://docs.microsoft.com/en-us/learn/modules/predict-costs-and-optimize-spending/media/5-byol-sql-server.png)

 Important

An Enterprise Agreement subscription is required to use these certified BYOL images.

## Use SQL Server Developer Edition

A lot of people are unaware that SQL Server Developer Edition is a free product for **nonproduction use**. Developer Edition has all the same features that Enterprise Edition has, but for nonproduction workloads, you can save dramatically on your licensing costs.

Look for SQL Server images for Developer Edition on the Azure Marketplace and use them for development or testing purposes to eliminate the additional cost for SQL Server in these cases.

 Tip

For full licensing information, take a look at the [documented pricing guidance](https://docs.microsoft.com/azure/virtual-machines/windows/sql/virtual-machines-windows-sql-server-pricing-guidance).

## Use constrained instance sizes for database workloads

Many customers have high requirements for memory, storage, or I/O bandwidth but low CPU core counts. Based on this popular request, Microsoft has made available the most popular VM sizes (DS, ES, GS, and MS) in new sizes that constrain the vCPU count to one half or one-quarter of the original VM size, while maintaining the same memory, storage, and I/O bandwidth.

| VM Size           | vCPUs | Memory | Max disks | Max I/O throughput      | SQL Server Enterprise licensing cost per year | Total cost per year (compute + licensing) |
| :---------------- | :---- | :----- | :-------- | :---------------------- | :-------------------------------------------- | :---------------------------------------- |
| Standard_DS14v2   | 16    | 112 GB | 32        | 51,200 IOPS or 768 MB/s |                                               |                                           |
| Standard_DS14-4v2 | **4** | 112 GB | 32        | 51,200 IOPS or 768 MB/s | 75% lower                                     | 57% lower                                 |
| Standard_GS5      | 32    | 448    | 64        | 80,000 IOPS or 2 GB/s   |                                               |                                           |
| Standard_GS5-8    | **8** | 448    | 64        | 80,000 IOPS or 2 GB/s   | 75% lower                                     | 42% lower                                 |

Because database products like SQL Server and Oracle are licensed per CPU, this allows customers to reduce licensing cost by up to 75 percent but still maintain the high performance their database requires.

## Check your knowledge

\1. 

True or false: If you already have Windows Server licenses, you have to pay for them again on Azure.



True



False

\2. 

True or false: Azure has money-saving options for test and development servers.



True



False









# Summary

- 4 minutes

We've talked through the Azure pricing calculator and how you can use it to estimate your costs on Azure and compare pricing between different service offerings. We looked at savings options, how to export pricing estimates, and at various tools that Azure has available to help you keep your cloud spend in check.

- Azure Advisor provides recommendations in many areas, including cost.
- Azure Cost Management gives you reporting and billing information, so you can gain insights into where you're spending your money.
- Cloudyn takes this even further and gives you detailed information that you can use for chargebacks and to identify areas of inefficiency.

We then explored best practices to help you save money on both infrastructure and licensing.

## Learn more

Here are some places to go to learn more about what we've covered today:

- [Setting up spending limits in Azure](https://docs.microsoft.com/azure/billing/billing-spending-limit)
- [Azure budgets](https://docs.microsoft.com/azure/billing/billing-cost-management-budget-scenario)
- [Explore flexible purchasing options for Azure](https://azure.microsoft.com/pricing/purchase-options/)
- [Understand terms on your Microsoft Azure invoice](https://docs.microsoft.com/azure/billing/billing-understand-your-invoice)
- [Bandwidth Pricing Details](https://azure.microsoft.com/pricing/details/bandwidth/)

## Check your knowledge

\1. 

Which of the following are used to determine Azure costs for each billing period?



The Azure website



Number of created virtual machines



The Azure pricing calculator



Usage meters

\2. 

Which of the following is a factor affecting costs?



Global infrastructure



Location



Availability zone

\3. 

Complete the following sentence. As an Azure customer, Azure Reservations offer discounted prices if you _________



Pay in advance



Provision many resources



Have a free account



Set Spending Limits





