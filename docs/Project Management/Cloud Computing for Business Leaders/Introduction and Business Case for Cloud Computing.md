---
sidebar_position: 2
---

# 2. Introduction and Business Case for Cloud Computing

# Lesson Outline

## Lesson Topics

In this lesson, we will

- Define exactly what Cloud Computing is
- Consider why Cloud Computing is important in the bigger picture
- Look at scenarios where it does and does not apply
- Explore different cloud computing models
- Learn about the characteristics of cloud computing
- Learn about the benefits of cloud computing
- How we calculate ROI (_Return of Investment_)
- Learn some reasons why a company should be considering cloud adoption
- Talk about building a strategy for moving your business into the cloud
- Look at some best practices and other expert perspectives
# What is Cloud Computing

## Cloud Computing

Cloud Computing is made up of these main aspects

- **ON-DEMAND:** Available when you need it. No need to pre-provision or request in advance. For example, if you need storage for your videos or photos, you can open an account with Google Drive or OneDrive from Microsoft and start uploading your videos and photos right away.
- **DELIVERY OF IT RESOURCES**: Service is delivered over the Internet. No need to be physically collocated to use. In the same example, you access Google Drive and OneDrive as services over the internet.
- **PAY AS YOU GO:** You pay for Metered charges based on consumption. No upfront capital investment required. For example, if you need a server to run an application, instead of buying and making a capital investment, you can open a cloud account with companies such as Amazon, Microsoft, and Google - request a server when you need it and start paying for it by the hour.

![Cloud Computing Graphic](https://video.udacity-data.com/topher/2021/February/602d976b_cloud-big-picture/cloud-big-picture.png)

Cloud Computing

## Types of service

In the image above, you can see that cloud service providers provide 3 main types of service

- Software application services(**SaaS**)
    - Software as a Service
- _Platform_ services (**Paas**)
    - Platform as a Service
- _Infrastructure_ services (**Iaas**)
    - Infrastructure as a Service

We will dive into each of these in the coming lessons.


# Why Cloud Computing Matters

## Rise in Cloud Adoption

There has been a dramatic rise in cloud adoption across all industries and customer segments. the demand is driven by 4 key business values.

- **Cost savings** - There have been several companies such as Netflix and Capital One that have retired all of their data centers and have reported as much as 50% savings.
- **Productivity** - As companies embrace the cloud, they report significant improvement in productivity - this is due to the elimination of wastage due to over-provisioning. They also report staff productivity improvements due to automation tools and innovative services provided by the CSP (c_loud service provider_).
- **Operational Resilience** - Cloud provides resilient infrastructure and other capabilities that allow you to improve operational resilience and reduce outages due to power disruption, hardware failures, natural disasters, human errors, and security breaches.
- **Business Agility** - Cloud provides an on-demand and elastic set of services allowing your application teams to focus on business value and not deal with infrastructure issues. This frees up people to innovate in your business, use cloud services to scale into new geographies, and enter new markets rapidly. With traditional infrastructure, it could have taken weeks to procure and provision new hardware.

# When do we use /not use Cloud Computing

### Start with a cloud-first approach

Cloud computing makes sense for the vast majority of use cases. It is a fundamental shift in the computing model, so try to always start with a cloud-first approach to new projects.

### (S)ervice (L)evel (A)greements

(C)loud (S)ervice (P)roviders, or CSPs provide an SLA for each of the services they offer, such as:

- Availability, Performance, Security, and Privacy of data, Location of data,
- The process to identify problems and resolution expectations
- eDiscovery and legal hold and so on and so forth.

### Consider bare metal

Most cloud providers provide what's known as "bare metal" offerings that allow your workloads to run directly on physical machines with no virtualization or multi-tenancy.

- If your workload is highly specialized and requires physical access to machines, you may run into limitations.
- Many high-performance computing workloads such as Genomics, Chip-design, Life-sciences, etc are optimized to run on bare metal. Bare metal instance types might be limited so you need to make sure your business needs can be met.

### Does the SLA meet business needs?

If the SLAs can't meet your business needs, you may be better off with moving to another CSP, or consider alternative solutions.

#### Cast study:

From my experience, one of the CSPs had an SLA clause - if they find any objectionable material, they will ask the tenant to remove it within 24 hours failing which they will shut down the tenant. The customer I was working with hosted their own customer data and had a higher SLA with their customers - 72 hours, the CSP's SLA, therefore, did not meet their business requirements. These are the types of business strategy decisions you need to recognize.

# loud Computing Models

## Deployment

- **Private** cloud is not the same as virtualized workloads running in your datacenter. Unlike virtualized workloads running in your data center, private cloud is typically on-demand, elastic, and charged based on consumption. Typically hosted by IT infrastructure team for internal customer
- **Public** cloud is offered by third-party providers such as AWS, Azure, GCP, IBM, Oracle, etc. They house multiple customers on the same shared infrastructure. The systems are not exclusive and can be used by anyone. Third-party providers, Multi-tenant and available to everyone.
- In reality, many organizations end up having a **hybrid** solution that takes advantage of the benefits of each of the deployment types i.e, public cloud, private cloud, on-premises infrastructure. Any combination of public, private, on-premises infrastructure, or edge location
- Some organizations may want to make use of **multiple cloud** providers - they may decide to host certain types of workloads in one public cloud and another type of workload in another public cloud. When 2 or more public clouds are used, the deployment type is commonly referred to as multi-cloud.

![Cloud Services from CSP](https://video.udacity-data.com/topher/2021/March/603e2bec_cloud-services/cloud-services.png)

tech stack

## Service

Depending on your needs and capabilities, there are several service model options available as you can see in the image above. These models are based on the responsibility split between you and your Cloud Service Provider.

Note: The term **CSP** will be used from now on to refer to a **(C)loud (S)ervice (P)rovider** such as Microsoft, Amazon, Google, IBM, etc.

- **IaaS** - In the Infrastructure as a service model, CSP provides you the basic infrastructure services - Compute, Storage, and Network. You are responsible for your application and data, along with all dependencies such as operating systems, databases, queues, language runtimes, etc. This model gives you the most control but you end up managing more components.
- **PaaS** - In the Platform as a service model, the CSP provides platform services you use to quickly build your applications. You are responsible for keeping your application and its data up to date, and the rest is managed by the CSP.
- **SaaS** - In the software as a service model, the CSP delivers the entire application as a service to you. You consume the application as is, with nothing to manage except your own data. Your CSP keeps your application up to date.

#### Description

#### Deployment model

Takes advantage of the benefits of multiple deployment types

hybrid

Typically on-demand, elastic, and charged based on pay-as-you-go consumption

private

Typically multi-tenant with multiple customers on the same shared infrastructure.

public

Typically when more than one public cloud is used

mixed cloud


An e-commerce company has significant operations in Europe with 2 datacenters running a private cloud in Europe serving all its European customers. The company is planning an expansion into the US and for latency and site experience reasons has decided to extend its e-commerce site by hosting it in the US for US customers. It needs to find the fastest way to do it to meet demand. After evaluating all options, the company decided to build a Hybrid cloud. Did they make a good choice?

Yes

# Public Cloud Characteristics and Benefits

## Public Cloud

### Public cloud

You have seen a few of these before when we defined the basics of the cloud. Now Let's discuss what public cloud is and where they are similar or different from private clouds.

- **On-demand** - you can request capacity on demand. Private clouds offer the same model but the capacity might be more limited as compared to the public cloud.
- **Elastic** - You can scale your workloads up and down without planning capacity. Private clouds offer the same but the capacity might be more limited as compared to the public cloud. If you are an online retailer, you need to be able to immediately scale during certain times of the year, such as holidays.
- **Pay as you go** - No upfront payment needed. Your charges are metered based on consumption and you pay as you go. In a private cloud case, the model would be the same and the charges may appear as chargeback or showback to your department.
- **Global reach** - Public cloud covers most global regions and is constantly opening more. A private cloud may be limited in global scale and reach. For example, if you are located in India, you can use a CSP's region in India or close to India to host your application.
- **Multi-tenant** - Other customers may also be using the same cloud and running on the same physical infrastructure. But CSPs manage the isolation between tenants so you don't need to worry about security etc. In the private cloud case, this is true as well with the difference that private cloud is meant for use by departments within the company and will not allow external parties to use it.
- **Security** - Public clouds offer a shared responsibility model where the Security of the cloud is CSP's responsibility. Securing applications running on the cloud is the tenant's responsibility unless you are using the SaaS model where the CSP is responsible for the entire stack as we discussed earlier. The model doesn't apply in private cloud cases since IT applications and infrastructure are all hosted internally.

### Quiz Question

Match the cloud property to the statements below

These are the correct matches.

#### Statement

#### Cloud Property

I live in US but can deploy my application to a location in Australia

Global Reach

I run my finance application for 2 days every month. Thank god, I don't have to pay for all 365 days.

Pay as you go

I have to worry about my application security only, not infrastructure

Shared Responsibility Model

During holiday season, I get unpredictable bursts of traffic on my site but I never worry about capacity

Elastic

I can shut down my site anytime and owe nothing

On-demand


# R.O.I. of the Cloud

## ROI: Return on Investment

### Business Case for Cloud

### Typical ROI

Let's start with the basics. What is (R)eturn (O)n (I)investment? Here's a simple economic formula for calculating your ROI.

`(gain - investment) / investment`

To understand this formula, let's take a simple example.

Let's say you invest(ment) $100 in the stock market.

At the end of the year, you sell(gain) all your stocks for $140.

Your ROI, in this case, would be (140-100)/100 = 0.4

- Any number **< 1** indicates from a financial point of view, the investment will be far greater than the benefit, which could indicate the _minimal value._
- Any number **> 1** indicates from a financial point of view, the investment will be far less than the benefit, which might indicate _good value_.

The challenge in building ROI models is to accurately quantify **gains**. In some cases the **gains** are straightforward to quantify like the stock market example, in other cases, it may not be as straightforward to quantify **gains**.

### Calculating GAIN

How do you build an ROI model to justify cloud investments?

Remember from earlier that the traditional model for calculating ROI is

`(gain-investment) / investment`

Conventional thinking might be to use cost savings driven model based on **(T)otal (C)ost of (O)wnership** as a basis for building ROI but these models can fall short as they only factor in monetary cost savings but neglect the other business benefits that come with cloud. These additional benefits can add significant value to the monetary **GAIN**

What are these other business benefits?

- Productivity
- Speed
- Size
- Quality
- Operational Resilience

_We will be talking about each of these_!

### TCO: Cost Savings as a first component of Gains.

(Gain - Investment) / Investment

Recall where COST Savings (_**Gain - Investment**_) is in our formula for ROI

The (T)total (C)ost of (O)wnership or TCO is based on the fact that you not only pay to acquire your assets but also incur ongoing costs to maintain and manage them.

Cost Savings = TCO (on-prem) - Forecasted Cloud Spend

To calculate the cost savings, you need to understand the Total Cost of Ownership (TCO) of your on-premise assets

### Major TCO drivers

This is not a comprehensive list but gives you an idea of things to consider when calculating the TCO.

- Servers, storage, and networks require to be maintained and fixed over their lifetime.
- The same applies to other parts that go in your DC such as racks and assemblies.
- Software licenses need to be maintained and renewed.
- Many assets require 24/7/365 electricity to keep them running efficiently.
- Costs of datacenters buildings and land
- Cooling expenses are sizable and shouldn't be ignored.
- Support staff for maintaining your infra and securing physical access

### Understanding your TCO

Understanding your TCO is the first step in the process. You can then build a TCO model with help from your CSP or a trusted partner. Many CSPs provide on-line Cloud TCO calculators too. [Here is an example of this(opens in a new tab)](https://azure.microsoft.com/en-us/pricing/tco/calculator/).

In general, most companies have realized significant savings by retiring Datacenters and moving to the cloud. These savings could range from 20% to 50% per surveys done by research firms.

### Other Benefits to Consider in addition to money savings

As we discussed earlier on the page, the traditional ROI model is based on _cost savings_. But, there are _other business benefits_ that might far outweigh the benefits due to purely cost savings.

Your ROI model should include these business benefits to be complete. You need to quantify the value of each of them as applicable to your situation and build an ROI model factoring in these business benefits in addition to cost savings. However, these business benefits are not easy to quantify. Many leaders have made cloud investment decisions based on the qualitative assessments of these benefits.

**Example** - The CIO of GE made an executive decision to move 50 apps to the cloud in 30 days, subsequently retiring most of GE DCs, moving thousands of apps to the cloud over the next 2-3 years.

#### Benefits to consider

- **Productivity**: Eliminating waste and achieving higher productivity
- **Business Agility**
    - **Speed**: How quickly can you respond to your customer needs
        - Provision capacity On-Demand
        - Enable CI/CD
        - Enable new deployment models
    - **Size**: Scale-up and reach a global audience
- **Quality**: Focus on your core differentiators by eliminating undifferentiated heavy lifting
- **Operational Resilience**: Utilize resilient infrastructure, tooling, and security of cloud

### Productivity

![Opportunities in Productivity](https://video.udacity-data.com/topher/2021/March/603e2e7d_productivity2/productivity2.png)

Opportunities in Productivity

### Removing wastage and avoiding missed opportunities

Your infrastructure needs are never the same throughout the year or year over year.

In the image above, we can see a hypothetical demand curve for the infrastructure needs for a growth business over many years

- Dotted green line(_predicted demand_): Since you can't predict demand accurately for many years out, you typically forecast infrastructure demand for the next 1-2 years based on input from IT and business teams and procure additional infrastructure
- Solid black line(_traditional hardware_): In real life, your infrastructure demand and utilization fluctuates as seen here
- Solid pink: (_Actual demand_). This is what actually happens

### The problems with this model ?

First you are making a large upfront capital expenditure

1. **Large upfront capital expenditures**. Your money is already accounted for well in advance
2. **Opportunity cost:** Since you are incurring an opportunity cost due to idle infrastructure capacity. Wouldn't it be nice if you could use this money for other business priorities?
3. **Unexpected jumps in demand** for infrastructure: During this time, you lose customers while waiting for new capacity from procurement. This is represented by the shaded area.

Cloud eliminates all of these problems by allowing you to provision capacity on demand

**Automated cloud capacity:** This can be closely matched to your demand curve. The result:

- No more large **capital expenditure**
- No wastage of **resources**
- No need to **plan capacity** in advance
- Never **lose your customers** due to infrastructure issues.
- Significantly **improve the operational efficiency** of your business.

### Speed

Speed matters in business. Businesses that can quickly react to changes in market conditions and adapt to external changes thrive. Companies such as Netflix and Amazon do thousands of production deployments per day.

The way this speed is accomplished is through automated processes called Continuous Integration and Continuous Deployments also known as **CI/CD.**

- **Continuous integration** refers to the process when as soon as a developer checks in his code a set of processes automatically start that would build or compile the code and put the code through several tests.
- **Continuous deployment** refers to the subsequent stage when the tested code also called "build" from the previous stage is moved to a staging area that mimics the production environment for more testing. When the tests pass, the build is deployed to production.

Cloud is a great enabler for speed. Cloud provides services that facilitate this CI/CD pipeline along with necessary tooling and observability metrics needed.

![Continuous Integration / Continuous Deployment](https://video.udacity-data.com/topher/2021/March/603e2fda_ci-cd/ci-cd.png)

Continuous Integration / Continuous Deployment

### Blue-Green Deployment

Imagine your existing running app, known as **Blue Deployment**. Let's say you want to upgrade the app to a new release.

You can replicate the entire infrastructure along with the new application code and seamlessly direct all users to the new deployment also called **Green Deployment.** If something goes wrong in the **Green Deployment** you can seamlessly redirect all users back to the original deployment.

It's much easier done in the cloud. Imagine you have an app that runs on 50 servers. You'll need to keep another 50 servers idle to do **Blue-Green** on-prem. In the cloud, you can quickly spin up new capacity and de-provision old capacity when not needed.

![Blue Deployment](https://video.udacity-data.com/topher/2021/March/603e304a_blue/blue.png)

Blue Deployment

#### Blue deployment

Blue deployment allows you to keep the previous version running while making sure that your Green deployment (new version) rolls out and is tested. With a cloud solution, this can be easily done with minimal cost and infrastructure.

![Green Deployment](https://video.udacity-data.com/topher/2021/March/603e3062_green/green.png)

Green Deployment

#### Green deployment

As you roll out a new version of your application (**Green** deployment), the previous version can be maintained relatively easily with services in the cloud. If there are any issues with the new version roll out, you can easily revert back to the **Blue** deployment. Consider the amount and cost of resources that would be required for an organization that housed all it's own hardware and software; essentially an organization would have to maintain 2 independent sets of all necessary hardware and software.

#### Speed Takeaways

- **Provision capacity On-Demand** to eliminate planning and provisioning time
    
- **Enable CI/CD** to speed up deployment
    
- **Enable new deployment models** that allow for quick deployment and easy rollback if needed
    

### Size

Cloud reduces the risk of entering new markets

- Easy to provision and manage new capacity
- Lower cost to exit if the expansion doesn't succeed

Existing businesses can leverage the cloud for market expansions and new product introductions to reduce risk

### Quality

#### Working capital efficiency

Lower costs improve working capital efficiency.

As cloud services improve your cost model and free up capital locked in infrastructure, the freed up capital now drives better experiences for customers. For instance - Netflix made a decision to exit datacenters and move to the cloud as they wanted to focus on an awesome video delivery experience for customers and not worry about infrastructure issues.

#### Business Centric services

Mindset shift towards customers and business-centric services

As you free your organization up from infrastructure operations and management, you can start shifting the mindset of your technology teams from IT-centric services to business-centric services. This results in a significant improvement in quality. It is not an easy transition requiring cultural and process changes that we will discuss later in the course.

### Operational resilience

_Eliminating Unplanned Outages_

How does the cloud address this issue?

- Cloud provides a **resilient infrastructure** to protect against hardware failures, natural disasters, power outages, and network outages.
- Cloud provides tooling for **infrastructure automation** allowing you to reduce outages caused due to human errors.
- CSPs hire world-class **security** experts to protect the cloud itself and offer security services to improve your overall security posture. The net result, if done right you'll be more secure in the cloud as compared to on-prem
- Software deployment into production through **CI/CD** pipeline and related services reduce outages caused due to software issues.

# Motivations for Cloud Adoption

## Business motivations

Your business motivations should help you set the right goals and a strategy to adopt the cloud. Here are some typical business motivations.

- **Cost savings** is a common one as people look to exit datacenters and eliminate capital expenses and associated operational expenses.
- As companies succeed and grow across geographies and enter new markets, **scaling** becomes a challenge. Cloud gives them a vehicle to scale.
- CSPs bring in **innovative technologies and services** that significantly shorten the release cycles allowing companies to respond to market needs faster.
- **Creating a new product or service** with disruptive potential and scaling is best done on the cloud. The cloud **reduces the cost of entry.**
- Scaling your IT **elastically** to match customer expectations isn't easy. Cloud's elasticity and **geographic reach** allow you to improve customer experience.
- Outages are expensive and cost you a lot of money in lost revenue and damaged brand. Cloud's **resilient infrastructure** and other capabilities allow you to reduce outages.
# Exercise Finance Interview

## Financial Interview: Identifying costs

Throughout the course, you will be recording your responses to the **Exercise** questions. This information is an excellent artifact for students to keep for after the course is complete. We have created a template for you, called `Exercise Template.docx` or `Exercise Template.txt`) to use to record your responses. This is located under the Resources section of the course, in the top left of this page.

Please use this template for all exercises starting now.

![Location of Templates in the Resources Section](https://video.udacity-data.com/topher/2021/January/600884ad_resourcesccbl/resourcesccbl.png)

Location of Templates in the Resources Section

### Identifying IT costs

Schedule time with your finance controller. Ask for specific IT cost elements that contribute to your on-prem TCO. In your exercise template, identify each identified line items with estimated costs. Mark line items that can be eliminated or reduced by moving to the cloud.

You can create your own template, or use this one as a starting point.

#### Example Finance Interview Template

|Category|Type of Cost|Amount|Can be eliminated or reduced?|
|---|---|---|---|
|Server|Purchase Cost + annual maintenance|||
|Storage|Purchase Cost + annual maintenance|||
|Networking|Purchase Cost + annual maintenance|||
|Software|OS + Virtualization solution - licensing + support|||
|Infrastructure|Power and Cooling|||
|Infrastructure|Leasing|||
|Infrastructure|Land and Building depreciation|||
|Application|Application license + Support||


# Solution Exercise #1

## Solution

See below for an example of the Finance Interview results from a fictitious company.

|Category|Type of Cost|Amount|Can be eliminated or reduced?|
|---|---|---|---|
|Server|Purchase Cost + annual maintenance|$158MM|Yes|
|Storage|Purchase Cost + annual maintenance|$48MM|Yes|
|Networking|Purchase Cost + annual maintenance|$35MM|Yes|
|Software|OS + Virtualization solution - licensing + support|$7MM|Yes|
|Infrastructure|Power and Cooling|$2MM|Yes|
|Infrastructure|Leasing|$1.5MM|Yes|
|Infrastructure|Land and Building depreciation|$1MM|Yes|
|Application|Application license + Support|$3MM|No|

How did your conversation go? Did you find any other items that could be eliminated or reduced

# Migration Strategies

![Migration Strategies](https://video.udacity-data.com/topher/2021/January/60147f38_migrationst/migrationst.png)

Migration Strategies

## Migration Strategies

Consider the image above. Imagine you have built the business case and are now ready to adopt the cloud. Where do you start?

The first step is to _**discover all your apps**_. You can use commercially available tools to discover and inventory your apps if you don't have one already.

1. From the inventory of apps, identify the ones you want to **retain**. This could be due to regulatory compliance or other reasons.
2. Identify the ones that are no longer relevant or not in use - plan to **retire** or sunset them.
3. Of the remaining - classify them in three buckets:
    - "**Sustain**" - These are apps that do not core or strategic to your business success but you need them. They are doing their job just fine and don't need any performance or scalability boost. For example - legacy apps running on mainframes may fall into this bucket. Your strategy, called **rehost**, should be to lift and shift them to the cloud with no modifications.
    - "**Optimize**" - These are your custom apps that are important and enablers for your business. Finance, HR, Sales management applications are some examples. See if you can find an equivalent SaaS application that can replace it(**re-purchase)**. If there is no suitable SaaS equivalent, you may want to "Lift and Reshape" (**re-platform**) the application taking advantage of cloud features. For instance, you may want to replace your own database with a cloud-managed database. This should require very little change.
    - "**Grow**" - These apps are core to your business and often are revenue-generating apps. For instance, if you are in retail, this could be your online store app. You may want to put investment into re-architecting (**re-factor**) to make it cloud-native taking advantage of as many cloud features and capabilities as possible.

![Workload priorities](https://video.udacity-data.com/topher/2021/March/603e3943_workoad-prior/workoad-prior.png)

Workload priorities

## Workload Prioritization

Prioritizing workloads in the cloud:

- Make sure that you have a low friction way of giving developers sandbox accounts so they can learn, try out things. In addition to formal training and certification, this would be one of the fastest ways to get your organization ready for cloud adoption.
- Any new application should be built on the cloud. Again, this is a great way for your organization to learn the nuances of the cloud and apply the learning to other workloads.
- Applications classified as "Grow" in your migration planning phase should receive focus next, as they are critical to your business success.
- Prioritize all other workloads based on business priorities. For instance, If cost savings is a top business priority, and if you can avoid renewing a data center lease coming up for renewal, you should prioritize migrating applications hosted in that datacenter.
# Quiz: Migration Strategies

### Quiz Question

These are the correct matches.

What apps will you keep

Retain

What apps will you sunset

Retire

Is there a cloud service that can accomplish the same thing as the existing app

Repurchase

Can you rebuild the app using new cloud features

Refactor

"Lift and Shift" directly to the cloud

Rehost

"Lift and Reshape" Is there a better way to accomplish result using the cloud

Replatform

### Quiz Question

A company is in financial services industry. Match the application description with an appropriate 6R migration strategy

These are the correct matches.

#### Application

#### Migration Strategy

Application was built for a certain use case that's no longer relevant as the company has changed direction

Retire

This application has very sensitive financial data and CFO has mandated that this application should never leave the datacenter

Retain

Company had a homegrown application built 15 years ago managing customer's profile, sales, and service records

Repurchase

Company has a custom order management application that has specialized business logic and runs on Linux and MySQL

Replatform

Company's core application is consumer banking app that was developed several years ago. It takes a lot of time to respond to fast changing customer needs as application modules are tightly linked with several interdependencies making changes expensive and time consuming

Re-Architect

A legacy backend application is used to process transactional sales and generating special reports for audit purposes. The auditing standard and requirements haven't changed in years nor are likely to change in the coming years.

Lift and Shift


# Exercise IT Interview

## IT Interview: Application portfolio

### Exercise 2

Review your IT application portfolio by scheduling time with your IT program manager or requesting a list of applications from your IT contact.

#### Part 1

Identify several applications that exist that fall under **each** of the categories (**Sustain**, **Optimize**, **Grow**).

#### Part 2

Identify and justify at least one application in **each** of the categories - **Sustain**, **Optimize**, **Grow**. In your response, include

- Describe the application, including its value
- Justify why it should be sustained, optimized, or grown.

_Note: If you are unable to obtain the list of applications or the scenario above doesn’t apply to you you can use the attached “ Fictitious company - list of applications” to complete this exer_cise

Please continue to use the template `Exercise Template.docx` or `Exercise Template.txt` to record your responses. This is located under the Resources section of the course, in the top left of this page.

## Sample SolutionExercise 2

- Our IT application portfolio has 120 applications. After browsing through the list, a few standouts in each of the categories.
- Sustain:
    - Order Processing application: This is a backend application that has been running reliably, processing transactions. It is mission-critical but doesn’t need to change. Best to lift and shift this app.
- Optimize
    - Exchange Servers: The Microsoft email system can be moved to Office 365 SaaS application
- Grow
    - eCommerce site: This is a core business application exposed to customers on multiple devices - mobile, PC, Mac, and Web. Need to invest in this app to keep up with changing customer needs
## Applications and service models

### Exercise 3

Use the list of applications you obtained from your IT contact. Alternatively, you can use attached “Fictitious company - list of applications” to complete this exercise. Please continue to use the template `Exercise Template.docx` or `Exercise Template.txt` to record your responses. This is located under the Resources section of the course, in the top left of this page.

Identify and justify at least one business application or need applicable to your company in each of the following categories.

- **SaaS**: Name at least one SaaS application vendor that can broadly meet the need.
- **PaaS**: Describe the PaaS services you’d need from a cloud provider. Justify why SaaS isn’t a good fit.
- **IaaS**: Describe the IaaS service you’d need from a cloud provider and justify why SaaS and PaaS aren’t good fits.
## Solution

- **SaaS:** Microsoft Office 365 can retire our on-prem(ise) mail systems and mail applications.
- **PaaS:** eCommerce site is quite complex and can be re-architected using microservices/containers and serverless services from the cloud. It is a custom application and a big differentiator so it doesn't make sense to replace this with a SaaS app.
- **IaaS:** Order processing application. It is a custom application with logic that’s unique to our business. An equivalent SaaS application doesn’t exist. Moving it to PaaS would require re-architecting the application which doesn’t make economic sense. Best to lift and shift this app on IaaS.

# Expert Perspectives and Best Practices

## Expert Intuition and Perspective

### Things to be aware of and think about

#### Quick wins

This helps earn trust as well as bring attention to the effort

#### Be aware of naysayers

Your initial results may not demonstrate ROI .. look for inflection points to demonstrate the results. When you are moving workloads .. your costs are going to be higher. It's only when you have retired a DC that’s when a measurable success point happens.

#### Developers want to learn!

Have a process to allow new experimental workloads, it's the best place to try out new things at a very low cost. Have a process to allow anyone in your organization to get a sandbox. Your business teams would love the agility, your developers would love the empowerment and learning … and this is one of the best ways to use the cloud to get a business advantage

#### Focus less on cost and more on innovation

Cost savings help, but cost alone is not enough to justify moving to the cloud. Examples of business cases for innovation include:

- AirBnb provisions more rooms per day than established hotel chains without owning a single room.
- Uber is a large transportation company without owning a single cab.

#### Best practices are evolving!

CSPs are constantly adding new services and patterns and practices are changing everyday. Be ready for this evolution!


# Quiz: Best Practices

### Quiz Question

You are the CIO of a mid-size company in the Commercial Logistics and transportation sector and have convinced your CEO to move to the cloud. 30 out of 50 apps from your data center in Amsterdam have moved to the cloud. Your CFO is concerned that the costs have been going up and is not sure if the cloud decision was a good one. How would you convince your CFO and CEO to stay the course? (Select all good answers)

- [ ] We are at the risk of getting disrupted by new business models and the likes of Uber and Lyft unless we reinvent ourselves. Cloud is the best vehicle for us to innovate fast.

- [ ] It is expected that the costs will rise since we are still operating our datacenter and in addition have added cloud expenses. When all 50 apps have moved to allow us to retire our DC in 2022, that's when you'll see significant cost savings

- [ ] We have been at the risk of outages since we only operate out of a single datacenter. Cloud will protect our business from potential outages as the cloud is multi-datacenter and multiple regions giving our business operational resilience.


## Lesson review

In this lesson we

- Defined exactly what Cloud Computing is
- Considered why Cloud Computing is important in the bigger picture
- Looked at scenarios where it does and does not apply
- Explored some different cloud computing models
- Learned about the characteristics of cloud computing
- Learned about the benefits of cloud computing
- Learned traditional ROI, but also looked ad an expanded definition of ROI
- Talked about reasons why a company should be considering adoption?
- Talked about how to build a strategy for moving your business into the cloud
- Finally, we looked at some best practices and other expert perspectives

# Glossary

|KeyTerm|Definition|
|---|---|
|6 Rs|Retain, retire, rehost, replatform, repurchase, refactor|
|Bare metal|When the compute is run on the actual physical server and not on a virtual machine.|
|Blue-Green Deployment|A type of cloud deployment where one configuration called Blue is replicated to another configuration called Green with updated software running on Green.|
|CSP|Cloud Service Provider|
|Gain|Profit|
|Hybrid cloud|A model combining on premises computing with public cloud computing.|
|IaaS|Infrastructure provided as a service.|
|multiple cloud|When someone uses services from multiple cloud providers.|
|Operational Resilience|When your operations can withstand hardware or software failure and still provide service.|
|PaaS|Platform provided as a service.|
|ROI|Return on Investment. When dealing with the cloud, ROI should go beyond just financial returns.|
|SaaS|Software provided as a service.|
|SLA|Service Level Agreement, an agreement that defines the details such as service uptime/downtime, customer vs provider responsibilities|
|TCO|Total cost of ownership|

# Further Learning and Reading

- [Building a business case beyond financials(opens in a new tab)](https://www.isaca.org/resources/news-and-trends/isaca-now-blog/2017/calculating-cloud-roi)
    - The value proposition for the cloud is changing, as supported in recent research ISACA conducted on the topic of cloud ROI. The fact that it is changing points potentially to 2 things. First, it potentially changes how we as risk, security, and assurance professionals evaluate cloud deployments. Second, from a governance standpoint, it informs how we measure cloud deployments and ensure continuous improvement in our organization overall.
- [Calculating Cost of Cloud(opens in a new tab)](https://www.atlassian.com/it/cloud/roi-tco)
    - A thorough research tool for helping you identify elements of, as well as calculate, both ROI and TCO.
- [TCO Calculator from Microsoft(opens in a new tab)](https://azure.microsoft.com/en-us/pricing/tco/calculator/)
    - Estimate the cost savings you can realize by migrating your workloads to Azure
- [6R Application Migration Strategic framework(opens in a new tab)](https://aws.amazon.com/blogs/enterprise-strategy/6-strategies-for-migrating-applications-to-the-cloud/)
    - A deep dive into the 6 most common application migration strategies.

