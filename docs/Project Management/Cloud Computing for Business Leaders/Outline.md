---
sidebar_position: 1
---

# 1. INTRO
## How was the course designed?

Every business is either going through a digital transformation or planning to and the cloud is almost always an integral part of it. Cloud computing, has already crossed the chasm and is now mainstream across all industries.

`Cloud is not just a technology, it's a way of doing business.`

### Course organization and flow

When I looked at companies who have gone through digital transformation successfully and those who haven't, I realized I needed to organize this course along 4 vectors:

1. Understanding the business case for cloud and what cloud can do for your business. Once you understand it, then transitioning your existing workloads and creating new workloads requires a strategic approach to maximize your ROI and minimize risks.
2. Transitioning your people, processes, and culture to the new world of the cloud isn't as straightforward as you think. Most leaders, even though they understand the business value of the cloud, underestimate the significance of this transition and instead emphasize cloud technology and strategic roadmap. Taking the existing IT mindset to the cloud just doesn't work.
3. Once you have built the business case, started preparing your organization for the cloud world, and have figured out the workload transition path, you need to think about the governance aspects of the cloud. Everything is code and API-driven in the cloud. The power of code and API is a double-edged sword. While it gives you the speed to move fast with a lot of automation, it can lead to undesirable outcomes if you don't put a governance model before you start building on the cloud or moving your workloads to the cloud.
4. Once you are in the cloud, you can innovate much faster as the cost of experimentation is very low and the payoff could be very high. What Services are provided by the cloud that companies in every industry are using to innovate and in some cases reinvent themselves?

To bring everything home, I then discuss the case of a US company that has successfully transformed itself into the cloud using the approach mentioned above.

---

*" I don't know where you are in your cloud journey, Perhaps you have solved some of the challenges already, perhaps you are still struggling and don't know why or how to address them? I hope you get something out of this course to apply to your specific situation." --*Sanjay Agrawal

## Course Lesson Review

![Cloud transformation through the lessons of the course](https://video.udacity-data.com/topher/2021/March/605e13bb_ccblpicture/ccblpicture.png)

Cloud transformation through the lessons of the course

_The image above, based on the 4 vectors mentioned above, is also the foundation for the design of the course. We have expanded on each element below._

### Introduction and Business Case for Cloud Computing

- The basics of cloud and its different deployment models and service types.
- How to build a business case for the cloud.
- The fact that true ROI of cloud comes from business agility and other benefits, so one shouldn't be building a business case purely on the TCO model.
- How to align workload migration strategies with your business objectives.

### Organizational Capability Building

- The softer aspects of cloud adoption involving people, processes, and cultural changes needed to operate well in the cloud.
- How a target operating model could help you assess skill gaps
- How a virtual structure like CCOE can be a powerful instrument of change
- Cultural and mindset changes needed across your organization, and in that context, covering
    - DevOps
    - DevSecOps
    - FinOps

### Cloud Governance

- How governance plays a part in your cloud operations
- Cost management
- Security
- Compliance
- How to establish governance at enterprise scale using
    - Hierarchies
    - Guardrails
    - Policies.

## Innovations in the Cloud

- How to harness the power of innovation as part of your cloud strategy.
- How several leading-edge innovative services offered by CSPs can help you innovate

## Case Study

Finally, to bring it all together, We take a deep look at a real case study with a major US financial services company, and how they made a transformation to the cloud. We'll see that the journey they took referred to many of the same concepts we learned in this course. This will be great preparation for your final project!

## Final Project

You will apply the learnings and skills from this course to drive the transformation of a hypothetical company. This is the Capstone project where you'll be given a detailed scenario about the company and you'll use your judgment to answer questions and design a path forwards towards a cloud transformation.

After the course is over, we encourage you to use these same skills to evaluate your own organization.


## Lesson Overview

In this introductory lesson, we will focus on

- Prerequisites
- What Cloud Computing actually is, from the executive lens
- Why Cloud Computing matters to businesses
- Stakeholders who are affected by moving to the cloud
- Over the last several decades, what are the major events, breakthroughs, and time periods that brought us to where are today
- The final project you will build to demonstrate your new learning!

# What is Cloud Computing

## Once every 20-30 years change

Cloud Computing is one of the tectonic shifts in the computing models that happens once in a few decades. It has far-reaching implications on:

- **Finance** and **budgets**
- **Security** and **risk posture** as the cloud is multi-tenant and connected to the Internet
- E**ngineering,** and **operations** as everything including infrastructure provisioning happen through code and APIs.

### On-demand, pay as you go

At a high level, cloud computing is an on-demand, pay-as-you-go service model delivered over the internet. Unlike on-prem, you don't need to plan and buy capacity ...you know it will be there when you need it and you can instantly provision it. You don't pay upfront.. you pay for what you use on a monthly basis. And you get those services delivered over the internet by your provider.

## Why should you care?

`It's already a $266,000,000,000 market growing at a CAGR( Compound Annual Growth Rate) of 20% and targeted to exceed half a trillion dollars by 2025.`

### Cloud as a disruptor

If you have been in business for a long time - Imagine when the Internet happened in the 80s and if you had decided to ignore it .. would you still be in business?

What if your competitors embrace cloud and change their business model to out-innovate you? This is simply because cloud gives you business agility that, in most cases, not possible with on-prem infrastructure.

_Every business is becoming a technology business_. Multiple Industries have been disrupted with software innovation. Spotify and Itunes disrupted the music industry, Netflix disrupted the media industry, Amazon disrupted commerce, Lyft and Uber are disrupting transportation, Airbnb is disrupting Hospitality. The list will go on as the technology innovation cycle continues.

# History of Cloud Computing

## History of Cloud Computing

There have been several landmark moments in the history of computing that got us to cloud computing as we know it today. Let's look at the brief timeline of events:

- 1950s : John McCarthy introduced the notion of **time sharing a mainframe**. Mainframes were super-expensive and the notion of timesharing was introduced to drive higher utilization of the computing capacity. This invention made computing affordable to smaller companies who couldn't afford to buy their own mainframes.
- 1960s: J.C.R. Licklider came up with the idea of connecting computers to each other. This led to the creation of **ARPANET**, the predecessor to the internet.
- 1970s: IBM introduced the concept of virtualization by introducing a Virtual Machine operating system. The notion of a hypervisor abstracting hardware to enable virtual machines is a landmark in cloud computing history.
- 1980s and 1990s: There were several advances in computing such as the launch of the **internet** and the **world-wide-web** with the Netscape browser. The Internet revolutionized all industries as companies started to address new business models enabled by the Internet. **Datacenter** spending increased. However, the average utilization rate of infrastructure in IT datacenters continued to be than 20%.
- 1999
    - **Vmware** : Some smart engineers in silicon valley finally cracked this problem of low utilization. They founded a company and introduced Intel x86 hypervisor and virtual machines to the IT world in 1999. Although the concept of virtualization wasn't new, VMWARE solved the hard problem of virtualizing the Intel x86 architecture, the silicon that powered most data center computers. It was an instant hit. Vmware rocked the IT world as virtualization led to server consolidation driving the utilization of data centers significantly up.
    - **SalesForce** launched the concept of Software as a service by delivering sales management software through its own cloud. This led to a big disruption to the traditional shrink-wrapped or packaged software industry.
- 2005 : Sun Microsystems launched the **pay-as-you-go computing model** with $1 cpu/hr pricing for its utility computing offering. Unfortunately, It wasn't commercially successful and was withdrawn soon.
- 2006 : Modern **cloud computing** was seeded by AWS in 2006 with the launch of storage service S3 and soon after its compute service EC2. As a retailer Amazon had lots of scaling challenges and went through a lot of internal changes to grow the business by building a new model that allowed scaling of its infrastructure services. The idea of offering the **IaaS** infrastructure services to others so they can build their own apps was born, and the rest is history.

## I.T. infrastructure investments declining

Investments in traditional IT infrastructure have been declining year over year while public cloud spend is picking. Per IDC, Q2 2020 was the first time when public cloud IT spend surpassed traditional I.T. (infra)structure spend.

# Pre-requisites

## What skills do you need to be successful in this course?

- Students should be able to identify workloads (business processes, applications, etc) within their organization that can be automated or made more efficient.
- Students should be able to identify roles, skills, organizational silos, and procedural constraints within the organization.
- Students should have a basic understanding of information security.
- Students should have a familiarity with current budgeting practices.
- Students should have a familiarity with word processors, spreadsheets, and similar numerical analysis tools, presentation tools.
# Business Stakeholders

`Cloud computing is not just a technology but a way of doing business.`

Therefore, every role is impacted in one way or the other. However, some organizations are going to be more impacted by the adoption of cloud than the others.

## High impact

These people will be highly impacted and will be taking an active part in the transition to the cloud

- In many companies, **CIO** leads the (I)information (T)echnology division and has been responsible for running companies' data centers and applications. _This organization is most impacted_
- **CTO** or **Head of Engineering** who runs engineering for all of the companies IT products and services where these products and services are software enabled. These engineering teams are dependent on infrastructure provisioning by the CIO staff.
- **Head of Information Security** for the company. As we will see, the security model in the public cloud changes significantly.
- **Head of Finance**, as the cloud spend model is Opex driven while the traditional model has been CAPEX heavy.
- **Head of Products** is impacted as the product development lifecycle changes significantly when built on the cloud. Products have to evolve to fit into the cloud's "as a service model" to stay relevant. Many shrink-wrapped software companies die as they couldn't reinvent themselves for the cloud world.

## Medium to low impact

These people are still impacted, but just not as directly as the roles we just talked about

- **CRO** or **Head of Sales**
- **CMO** or **Head of Marketing**
- **HR**
- **Legal**

# Project Overview

## Bintoso's Cloud Transformation

### Scenario

- You will be working with an international clothing company called Bintoso. The organization is facing stiff competition from other department stores as well as online retailers. The revenues and margins have been trending down.
- The previous executive team did not have a forward-thinking strategy, so the new CEO has asked you to lead the digital transformation of the company.

### Background business documents

You will be provided with a wealth of information to help you understand the current culture of Bintoso, including business documents such as

- A detailed company backgrounder
- Recent income statement
- Current financial information on current and upcoming data center costs
- Current hierarchical organizational charts
- Email exchanges between executive team members and staff highlighting business challenges and opportunities

Don't be intimated by those artifacts, once you start with the company backgrounder provided by us, they will all fall into place, and in fact, will give you a really solid picture of the organization

### What will you do?

This is where your project starts. Ultimately, your task is to analyze and propose a cloud strategy for Bintoso. Through your analysis, you will:

- Identify business problems best addressed with cloud
- Prioritize workloads to maximize ROI
- Re-define the organizational model so that it reflects needed changes in skill levels, culture, and processes
- Define a governance model that would mitigate risks and optimize spend, as well as bring automation into the organization
- Propose a new innovative solution on the cloud that would deliver new business benefits
# Lesson Review

## Lesson Review

Let's take a brief look back at what we went over in this lesson:

- We discussed what skills you will need to already have to be successful in this course
- We talked about what Cloud Computing actually is, from the lens of the executive..and looked at a scenario to demonstrate that
- We saw the value of Cloud Computing and addressed why should you care
- We looked at the various people in the organization who are affected by moving to the cloud
- We took a step back in time and noticed the major events, breakthroughs, and time periods that brought us to where are today
- We talked about the final business project you will build to demonstrate your new learning!
# Glossary

| KeyTerm       | Definition                                                    |
| ------------- | ------------------------------------------------------------- |
| on-demand     | Made available when you demand it/or customer needs service   |
| on-prem       | On premises or in customer-owned data centers or co-locations |
| pay-as-you-go | No upfront payment, you pay as you consume                    |
# Further Learning and Reading

- [A brief history of Cloud Computing(opens in a new tab)](https://www.ecpi.edu/blog/a-brief-history-of-cloud-computing): This article discusses the technology, culture, and business transition from the 1960s to the present.
- [How Amazon’s S3 jumpstarted the cloud revolution(opens in a new tab)](https://www.protocol.com/enterprise/amazon-aws-s3-15-years): Looking back over 15 years since Amazon's first real web service brought us everything from Pinterest to coronavirus vaccines.
- [AWS Executive Insights(opens in a new tab)](https://aws.amazon.com/executive-insights/): Perspectives on enabling cloud innovation and transformation through culture, talent, and leadership
- [Book: Reaching Cloud Velocity(opens in a new tab)](https://www.amazon.com/gp/product/B086VDRTC2/): AWS has transformed the ability of businesses of every size and in every industry to reduce costs while being more secure, more resilient, and innovating much faster than ever before. Leaders looking to emulate this business impact with the cloud will learn powerful lessons from those who have gone before to accelerate their own journeys.