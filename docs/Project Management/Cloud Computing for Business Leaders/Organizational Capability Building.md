---
sidebar_position: 3
---

# 3. Organizational Capability Building


# Lesson Outline

## Lesson outline

In this lesson, we will focus on Organizational Capability Building that is so important for the successful adoption of the cloud. _Many cloud endeavors fail or stall due to executives not paying enough attention to this topic._

## In this lesson:

- We will start by building an understanding of different components of Organizational capabilities.
- We will consider why Organizational Capability Building is important in the bigger picture
- What's the ideal target state you should be striving for and how can you get there.
- How do you evaluate your people and skills needed in the organization and bridge the skill gaps?
- There are many changes your organization will need to adapt to reach the target state. Process and Culture are two of the most important. As part of that, implementing a new virtual structure called a CCOE is extremely important
- How do DevOps and DevSecOps intersect to play a critical part in Organizational Capability Building
- What is FinOps and How does FinOps play a part in Organizational Capability Building.
- Finally, we will look at some best practices and other expert perspectives on this topic

# What is Organizational Capability Building

## Building organization capabilities

Organization capabilities are built to transform environmental inputs such as customer feedback, market trends, technology trends into outputs such as products or services for your customers.

![Organizational capability building benefits](https://video.udacity-data.com/topher/2021/March/603e38f2_organ-capab/organ-capab.png)

Organizational capability building benefits

If we look deeper, organizational capabilities are built around three key pillars -

1. **People**
2. **Process**
3. **Technology**

In simple terms, it's a combination of professional skills, processes defining how things get done, and technology that allows inputs to convert to outputs. What binds them together is the culture that's unique to an organization and in many cases a differentiator

## The Impact

When you are done with changes in **People**, **Process**, **Technology**, and **Culture** you should see the pervasive impact throughout your organization. You can see the effectiveness of the changes in terms of

- The increased **speed** that's measured by how quickly you can respond to changing inputs to produce outputs
- And a higher rate of **innovation** measured by the number of innovative products and services you introduce to delight your customers.

# Why do you need to build new organizational capability ?

## Re-evaluating your organizational capabilities

A big technology change such as the cloud requires you to re-evaluate your **organizational capabilities**. You need to bring this big of a change in harmony with the other pillars of your organization:

- **People**
- **Processes**
- **Culture**

Many cloud projects stall or fail due to leadership f_ailure to recognize_ the need for this balance. Most people think of the cloud as a destination. Few realize that the cloud is not a destination but an entirely different way of running a business.

## The Impact

![Organizational impact](https://video.udacity-data.com/topher/2021/March/603e3a7c_org-impact/org-impact.png)

Organizational impact

- Moving to _pay as you go_ means a change in your **financial model** from CAPEX to OPEX
- **Procurement** isn't negotiating commercial license agreements anymore with software and hardware vendors. They now work with cloud vendors and negotiate discounts based on consumption commitments.
- **Engineering teams** who were used to raising tickets for servers, storage and networking infrastructure provisioning now have the power to provision infrastructure as code in the API-driven provisioning model in the cloud.
- **InfoSec teams** who had to end the responsibility of securing physical and logical access to apps and infrastructure, now share this responsibility with the CSP. So they need to evolve their practices in line with this new shared responsibility model.
- **Legal and Compliance** complexities come from the fact that the cloud provider has a global presence, offers many services, and is constantly rolling out new services. This poses new challenges as developers adopt new services and provision infrastructure around the globe. Earlier the IT assets were limited to maybe a few data centers in a known location.
- **IT operations** earlier favored stability over feature changes. To support business agility in the cloud, the focus of IT operations is now shifting towards supporting frequent changes while still ensuring stability. This requires a different approach to build and deploy features.
# Target State Model

## What is Target State

Your target state is never an end state. In the cloud world, the only constant is _**CHANGE**_. But you know the organizational capabilities you are building are effective when you begin to see results in these 4 key buckets.

- **Speed**
    - You should be seeing an order of magnitude more changes getting rolled out to customers. For reference, companies such as Amazon and Netflix do 1000s of deployments per day. While it took them many years to get to this level of maturity, it should give you an idea of what to aim for that's best for your business.
- **Innovation**
    - The cost of experimentation is very low in the cloud. The Organizational capabilities you enable should result in a culture of risk-taking and innovation.
- **Collaboration**
    - No more silos. Application teams not just build apps but are responsible for running them too. Security is everyone's responsibility and needs are baked in the process. No more security check gates. Everyone is watching for costs and optimal spending. It's no longer purely a finance dept. check.
- **Efficiency**
    - Measure the new efficiency you gained by reducing your spending on undifferentiated activities. Long ago, I was interviewing with a startup that was building intelligent network processing cards that go into servers and offload certain operating system network processing in hardware. The founder of the company told me - 60% of his funds go into building a basic network card before he can add intelligence to it. Cloud allows you to just build what your core differentiators are leaving the heavy-lifting of infrastructure and operations to CSP.

## How do we get there?

- **People and Skills**
    - People and Skills - No change is possible without people's support and appropriate skill set for the new world. Often it is people who become the blockers, so you need to handle this part carefully.
- **Culture**
    - Process and Culture feed off of each other. A forced process change without the accompanying culture would face resistance. As a leader, you need to build the mindset for change before introducing the change. We will look at some of the cultural philosophies and practices commonly in play at companies that have successfully adopted the cloud.
- **Process**
    - Cloud requires things to be done differently. Treating the cloud as just another hosted data center and carrying on-prem practices to the cloud is a common mistake. We will discuss a mechanism called cloud center of excellence also known as CCOE that can be instrumental in the adoption of new processes and practices.

Process and Culture feed off of each other. A forced process change _without_ the accompanying culture would face resistance.

`As a leader, you need to build the mindset for change before introducing the change.`

# People & Skills

## People and Skills

The passion and skills of the people in your organization are where you need to start. Many cloud projects stall or fail because of resistance from within the organization or lack of understanding of why this change is good for the people and for the business. In addition, the rapid pace of digital transformation is driving a shortage of skills in the industry.

_The answer lies in motivating your own employees to upskill themselves._

As we said before, the people, processes, and culture changes are all interlinked and need to be driven together, leading you to your desired target state.

### People in your organization

![](https://video.udacity-data.com/topher/2021/March/60638d32_spheres/spheres.png)

The Spheres of Responsibility

### Spheres of responsibilities in the cloud

As you see in the image above, there are essentially 4 spheres of responsibilities in the cloud where you need to map your existing people.

- **Cloud Business Management** sphere is about managing your business needs to cloud. Things such as budgets, application portfolios, migration strategies, and plans are all managed by roles that map to this sphere. For instance program management, financial analysts, or controllers would map to this sphere.
- **The Cloud Infrastructure** sphere is about planning and managing types of instances, networks, storage services, or disaster recovery. The infrastructure architect and the infrastructure Ops engineer is responsible for creating reusable templates and assets for infra provisioning and operations.
- **The Cloud Security** sphere is about ensuring organization security and compliance policies are architected into the applications and infrastructure. Cloud providers have a "_Shared responsibility_" model where the security of the cloud itself is CSP's responsibility but anything that's built on top becomes the customer's responsibility.
- **Cloud Application Infrastructure** sphere is about building and provisioning application assets in the cloud using cloud services such as databases, queues, etc. The DevOps model which will be covered later allows the DevOps engineering and application developers to collaborate to ensure the application meets the required functional as well as non-functional needs of the business. These non-functional needs may include performance, scalability, uptime, etc.

### Cloud Enterprise Architect

The Cloud Enterprise Architect that may map to the Enterprise Architect role in your organization goes across all spheres, aligned with the businesses to make sure the business needs can be met with the cloud platform.

#### Example

Application architects along with DevOps may package the infrastructure provisioning in the code itself for dynamic provisioning of infra and apps. We will discuss this deeper when we talk about DevOps and DevSecOps.

### Bridging Skills Gaps

We did a rough mapping of roles in the cloud world. If those roles are to be played by your existing staff, they need to upskill themselves. This is the hard part. Why?

- **Realize**
    - _People generally have a resistance to change_. They like to be in their comfort zone where they hold a position of power. It is not natural for people to unlearn and then learn new skills.
- **Motivate**
    - _Start with yourse_lf. Take a course or two or perhaps a certification. Assure people that learning together is fun and that there is no risk to their current job. Reward appropriate behaviors. Also, make sure they do something with new skills so training isn't just an academic exercise. Providing sandboxes is one of the ways.
- **Scale and Attract**
    - As pockets of learnings happen throughout the organization, make sure the cloud-savvy community is growing by _sharing their learnings_. Once the word goes out, this would attract external talent too.
# Process : CCoE

## CCoE

### (C)loud (C)enter (o)f (E)xcellence

Addressing skill gaps is important, but you also need to think about the process and cultural changes needed to embrace the cloud.

`Process and Culture feed off of each other.`

There is a powerful mechanism called **Cloud Center of Excellence** that has proven to be successful in driving the process as well as cultural change at scale in large organizations. Once you understand the concept and motivation behind CCOE, you can adapt it to fit your specific needs. Some organizations may refer to it as _Cloud Program Office_ or _Cloud Business Office._ While CCOE will get you started on this big change, you need to be aware of a couple of other things as well that will need to be part of this effort

- Cultural changes such as **DevOps** and **DevSecOps** to help drive agility in your business
- Changes in your financial model from _Capex to Opex._ You need to be aware of a growing concept called **FinOps**. FinOps practices would allow you to manage the change in the financial model introduced by the cloud. _At its core, FinOps is also a cultural practice._

These structures, processes, and cultural changes will enable your organization to get the best out of your cloud investments.

### CCoE

- **What is CCoE?** CCOE is not a permanent structure, but instead _a virtual_ team consisting of people from different functions such as Engineering, Operations, Finance, Business, and Security. CCOE gets its sponsorship from a C-level leader typically CIO or CTO
- **Why do I need it?** You don't have to have a CCOE but it has been proven to be very successful in removing the blockers and accelerating cloud adoption, especially in large organizations with multiple business units.
- **What does it deliver?**
    - **Governance** - We will cover Governance in the next lesson but just know that CCOE will ensure adherence to all of your organizational policies through tooling and automation. These policies scan across security and compliance, cost management, and other areas.
    - **Brokerage** - CCOE can assist users in selecting cloud providers, architect the cloud solution(s) and collaborate with the sourcing team for contract negotiation and vendor management.
    - **Community** - Raise the level of cloud knowledge in the organization and capture and disseminate best practices through a knowledge base, source code repository, training events, outreach throughout the organization, and more.

### CCoE structure

![](https://video.udacity-data.com/topher/2021/March/603e3e3b_ccoe/ccoe.png)

Business Units image

As you see in the image above, the CCOE typically sits outside the **(B**)usiness **(U**)nits and provides its services to multiple BUs. For example, a consumer durable manufacturing company such as LG or Samsung may have separate BUs for refrigerators, washing machines, televisions, etc. In addition to an enterprise-wide central IT organization, each BU may have its own specific IT organization.

### CCOE functions

- **Business**
    - On the business side, CCOE works with all BU stakeholders to identify business priorities, creates onboarding plans for identified workloads, consolidates BU needs to negotiate contracts with cloud vendors, and puts control around organizational policies. It manages risks and compliance with a proper governance model as well. It also implements policies and controls to ensure cloud spend is optimized.
- **Technical**
    - CCOE acts as an enabler for all application teams supporting different BUs, provides a set of shared services, provides reusable assets such as templates, code, etc. In addition, as a champion of cloud, CCOE also runs training and education events for cloud skills enablement of the entire organization.

In practice, the business and technical functions are sometimes difficult to separate as they are very much intertwined.

### For example

Cost management spans across vendor contracts as well as engineering practices which if not managed well, can lead to wasted cloud spend.

---

_CCOE exists as a change agent to drive cloud adoption across the enterprise. As different teams become proficient in utilizing cloud over time, the need for CCOE should diminish_.

# Culture

## Typical Current State

There is tremendous value in figuring out your current state. Be willing to ask hard questions and really dig to determine the truth.

Below are several of the most common states in a typical large legacy enterprise. _If your organization can relate to any of these, it might be an indication that changes are needed._

- **Big Releases**
    - To avoid risks, they plan for big releases only with a typical frequency of once or twice a year. This also helps amortize overhead costs.
    - **Changes needed:** Instead of big releases, you need to plan and release small changes. Many organizations such as Netflix and Amazon do thousands of changes per day.
- **Functional Silos**
    - Organizations have functional silos that excel in what they do but this structure is not designed for high-frequency releases. This structure was optimized for maximizing quality and stability over speed which made sense for those times when the market demands didn't change at the pace they change today. These can include
        - Business groups such as marketing, sales, finance
        - Appdev
        - Operations
        - Infrastructure
        - InfoSec
        - Enterprise Architecture
    - **Change needed:**
        - This would require a _collaborative_ approach that cuts through all functional silos. So for instance, if there is an outage, everyone takes ownership to resolve it. It's not just an operations job.
        - risk-taking is an important part of the culture. if things break, they can be rolled back. If you are on the Agile transformation path, you are partly there!
        - the rest would come from DevOps and DevSecOps practices. (We will cover DevOps and DevSecOps in the next lesson. )
- **Low Deployment Rate**
    - The rate of deployments is relatively low. Again, This is by design as the organization and processes were designed to meet the then prevailing business needs. real Example?
    - **Change needed**: You shouldn't be afraid of increasing the frequency of deployments. If things break in production, you can always rollback.
- **Technical Deb**t
    - As businesses feel the need to respond fast, they ask for more. In the current operating structure, IT responds by taking shortcuts causing technical debt to start mounting. real Example?
    - **Change needed**: While making all these changes won't reduce your existing technical debt, it would certainly not make it worse. This is because the changes allow you to operate at the speed of the business now.
# Exercise: People in the Organization

## HR Perspective: Your people

### Exercise 1

Assume you are the head of HR for your company. Your CEO values the Cloud as imperative and has asked you to come up with a plan to assist other engineering and business leaders with cloud transformation. Identify 3 key problem areas from an HR perspective and justify key steps you would take to enable this transformation. Consider elements of culture, skills, and people.

Please continue to use the template `Exercise Template.docx` or `Exercise Template.txt` to record your responses. This is located under the Resources section of the course, in the top left of this page.

# Solution Exercise 1

## Solution

3 key problem areas:

- Motivating employees to re-invent themselves:
    - Sign up with 3rd party training companies (such as Acloud.guru, Udacity etc.) to make cloud training available to employees at enterprise discounts.
    - Work with BU heads to launch new initiatives to encourage employees to learn new skills. BU heads can lead by example by taking courses such as “CCBL” from Udacity and discuss the significance of a growth mindset in town halls.
    - Launch quarterly “Hackfests” and hackdays in partnership with cloud providers.
- Creating a culture of risk-taking and experimentation
    - Work with finance and BU heads to create new programs such as letting employees work on their favorite cloud projects for 10% of their time.
    - Rewards and recognition for top innovators in quarterly town halls.
    - Ensuring there is low friction for employees to get access to cloud sandboxes
    - Build executive education programs to help executives remove silos, understand the significance of collaboration across business units, IT, Operations, etc, and redefining metrics of success for collaborative teams and not just individual functions.
    - Re-examining team structures and ensuring teams are small in size (10-12 people at most)
- Attracting new talent to help with cloud transformation
    - Market the cultural transformation initiatives (e.g. employees get 10% of their time to work on their favorite cloud projects) at the company
    - Publish case studies of cloud led innovation at the company
    - Run targeted campaigns with the help of your key employees who can speak to the work environment at your company and the ground floor opportunity to drive a key transformation.
# DevOps and DevSecOps

### DevOps

How do we evolve the culture to adopt the changes we just talked about?

- **Culture**: DevOps is a culture where business analysts or product managers, application developers, testers, and operations all work together as one team with a singular focus _- deliver features to customers with quality and at a high velocity,_
- **Process automation and tooling**: They accomplish these goals by developing automation frameworks and tools that remove manual processes and error-prone delivery. In a perfect DevOps world, the moment code is checked in by a developer, a series of automation tasks are spun up to build, test, and verify things. When all checks pass, the code is automatically deployed to production. Monitoring and observability tools and frameworks give real-time visibility to developers so they can take corrective action if needed through code modifications.
- **Continuous Integration and Continuous deployment**: We have talked about Continuous Integration and Continuous deployment in an earlier lesson. They are an integral part of DevOps culture.

### DevSecOps

DevSecOps is a modification of the DevOps culture where security as a practice is also included.

- **Shift-left security**: 'The core idea here is to "shift-left" security earlier in the development cycle and make it an integral part of the DevOps practice.
- **Part of the DevOps teams**: In the DevSecOps world, Infosec architects become part of the DevOps teams helping deploy secure code to production.
- **Security as a "gate"**: This eliminates security as a "Gate" in the pre DevOps days where things would slow down due to back and forth between Dev, Ops, and Infosec teams.

### DevOps Cycle

The traditional DevOps environment has evolved into a typical cycle as shown in the image below.

- The team starts with planning a change that developers code.
- The changes go through the Continuous Integration/continuous deployment process
    - Build
    - Test and
    - Release
- The Production team
    - Operates the environment
    - Monitors the environment
    - Observes the running environment

Then the team returns to the top of the cycle planning of the next change to either improve the existing environment for scale and efficiency or introduce a new feature.

By planning small changes and rolling them back as needed, the team is able to deploy many changes in a day.

![Phases of the DevOps Cycle](https://video.udacity-data.com/topher/2021/March/603e41d8_devops-cycle/devops-cycle.png)

DevOps Cycle

### DevSecOps Cycle infused into DevOps Cycle

DevSecOps overlays security functions on the DevOps processes and makes security an integral part of the cycle. You can see this DevSecOps cycle overlayed onto the DevOps cycle we looked at earlier on the page.

The team implements different security features throughout the entire process:

- Defining security policies and threat modeling at the planning stage. The team may refine the threat model based on observed security incidents from the prod environment.
- Static analysis of the code for security flaws is done in the **code** and **build** stages. Manual **code reviews** combined with **automated static code analysis** are typical at this stage and are integrated with the CI/CD pipeline.
- Several **security tests** are run in the Test stage including Pen testing. When all tests pass the pipeline moves to the deploy stage.
- Ensuring tamper-proof logs are archived for audit purposes and forensic analysis as part of security incident response is an important step during the deploy stage.
- When the system is in operation, **threat intelligence tools** and platforms collect information from diverse sources to mitigate threats such as Advanced Persistent threats, Zero-day attacks.
- Security is continuously **monitored**, **intrusions detected** and **responded to** using tools and automation from a combination of CSP services and third-party tools.
- Security incidents if any are **recorded for analysis** and continuous improvements, with a focus on quick recovery to avoid downtime.
- Similarly, security **compliance validation** is done on a continuous basis and violations reported immediately for automated or manual remediation. A combination of CSP services and third-party tools allows you to stay compliant to security standards such as CIS or NIST benchmarks and even controls provided by industry-specific compliance standards such as PCI DSS, HIPAA, and Hi-trust.

The DevOps processes lead to a model where security is everyone's responsibility and the team is able to move fast by eliminating security gates in the pre-DevOps world. The security posture is significantly improved as security is now _baked in_ and not _bolted on_.

![Phases of the DevSecOps Cycle](https://video.udacity-data.com/topher/2021/March/603e41ed_devops-secops/devops-secops.png)

DevSecOps Cycle

#### What do DevOps and DevSecOps practices deliver?

- High-velocity deployments to production
- Rapid feedback and iteration based on the feedback
- Agility and responsiveness to customer needs

### DevOps in Waterfall and Agile Methodologies

In the image below, you can see the time differences of deployment for all of the methodologies.

- **Waterfall** model of deployment: each function hands over its output to the next function. When the build is fully tested, it gets handed over to Operations for deployment. This process was designed for big releases and can take _**months**_.
- **Agile** model of deployment: This movement in the developer community came into existence to break big releases down into smaller chunks. It helped _accelerate_ the processes as many in-efficiencies of waterfall got eliminated in this model and reduces time to _**weeks**_. However, there was still a _separation_ that existed between DevTest and Operations organizations as DevTest would handover the build to operations for deployment. The separation caused issues such as "_It works in Dev/Test environment but breaks in production_". Also, there was limited observability of the production environment so Developers couldn't improve things fast enough.

![Waterfall & Agile & DevOps & DevSecOps](https://video.udacity-data.com/topher/2021/March/603e41fb_waterfall-agile/waterfall-agile.png)

Waterfall & Agile & DevOps & DevSecOps

### Quiz Question

Refresher: Technical debt is when ___ .

the rate of change of business requirements exceeds the rate of change sustainable by IT.

the rate of change sustainable by IT exceeds the rate of change of business requirements

Submit

### Does this DevSDecOps model address technical debt?

While Agile helps, it is not sufficient to drive the velocity required. It can still take weeks.

### Impact of DevOps and DevSecOps culture

DevOps and DevSecOps culture bring all functions together in one team to plan and iteratively deliver features at a higher velocity without compromising security and quality. There are no silos and no handoffs. The release velocity can now be in _**days**_ and even _**hours**_ with a fully automated CI/CD pipeline. _Think of how innovative you can be with this type of flexibility._

### Characteristics of a DevOps culture

_What is it that sets DevOps culture apart?_

- DevOps teams **plan and release small change**s. They are easier to manage and rollback is a lot easier. Companies such as Netflix and Amazon do thousands of deployments per day.
- **Close-knit collaborative teams**: DevOps is a culture and the core of the culture is close-knit collaborative teams that have a singular focus. No more Developers saying "_Ops resists changes_", and Ops saying "D_evs deliver crappy builds that break production_".
- The singular focus of DevOps teams is to deliver **secure cod**e at **high velocity** while **minimizing potential risk**s.
- Often teams can't scale due to people resources as bottlenecks. DevOps teams **build automation** where appropriate to **eliminate human intervention** and chances of human errors.
- In the DevOps world, there is **no business vs IT**. It's all business. Teams work towards the **common goal** of planning and delivering business features.
- Since business and IT are working together to plan and deliver features, there are **no more shortcuts by IT** and as a result no or much less technical debt.

## Ease of implementing DevOps in the Cloud

- **API driven**: Cloud infrastructure and services are driven by Application Programming Interfaces (API). This allows the DevOps team to build an automation framework easily provisioning infrastructure and application resources programmatically.
- **CI/CD services**: Continuous Integration and Continuous Deployment services are natively provided by cloud providers. For instance, Azure provides Azure DevOps. AWS provides services such as AWS Codepipeline, AWS Codebuild, or AWS CodeDeploy.
- **Cloud elasticity benefits**: Cloud's elastic properties allow you to do multiple types of deployment models cost-effectively such as the Blue/Green deployment we discussed earlier. Cloud also makes it easy to programmatically clone a production environment for staging or testing.
- **Governance**: Cloud provides lots of controls and observability features that make Governance easier. CSPs provide fine-grain usage and cost reporting allowing you to track and manage your project's development and deployment costs.

# Exercise: Customer Service Response Time

## Addressing customer service response time

### Exercise 2

Assume you head a newly created CCoE for your organization. Your organization wants to improve the response time to customer needs. Your existing organization methodology is waterfall-driven. What specific steps would you take to transform your organization to improve the response time to customers? Name at least 3 steps and rationalize the expected outcome.

Please continue to use the template `Exercise Template.docx` or `Exercise Template.txt` to record your responses. This is located under the Resources section of the course, in the top left of this page.


# Solution Exercise 2

## Sample Solution

I’d take the following steps:

1. Recruit a cross-functional team to join CCOE by handpicking candidates who could be change agents, have a growth mindset, and are not afraid to fail. The team would be small ~6 people
2. Pick a small project (e.g. building a new app) and deliver it quickly on the cloud using DevOps model and tooling from the cloud provider (e.g. Infrastructure as code, CI/CD automation)
3. From this project, create a reference architecture, tooling, and other re-usable assets for the cloud that can be shared with other teams
4. Evangelize the outcome and benefits. Get leadership support to spread the message.
5. Organize DevOps education brown bags, share experiences and act as mentors for other teams. As more teams onboard to cloud and DevOps, keep adding to the re-usable assets
# FinOps

## What is FinOps?

- Also known as **Cloud Financial Managemen**t, it is a new cultural practice where finance, procurement, engineering collaborate to manage cloud spend.
- It's a new process - unlike the on-prem model where finance and procurement would negotiate with vendors and procure assets for use by engineering, in the cloud world engineering is procuring assets and spending the company's money when they spin up resources in the cloud.

## Why is FinOps needed?

- If you want to **get the best value** from your cloud spend, you need to adopt new practices and make changes to your operating models. Otherwise, You run the risk of cost overruns and wasted spend if the FinOps practices and controls are not put in place.
- When costs get out of control, it is hard to **drive accountability** across teams. FinOps practices help you with this.
- Every business makes a **tradeoff between speed, cost, and quality** with the limited money it has. FinOps helps you achieve the right balance.

## Phases of FinOps

There are 3 main phases of FinOps:

- **Inform**
    - FinOps teams start with data and look at the spend by department, BU, project, whether it is Dev, Test or Prod, etc. They also look for anomalies in the data to identify opportunities for savings. For instance, if a particular cloud SKU is showing lower utilization, perhaps it can be substituted with a lower SKU, a process called rightsizing.
- **Optimize**
    - Based on the data from Inform phase, the team would identify opportunities such as the one we mentioned with rightsizing. Financial goals are set and the team looks at ways to optimize spend to reach the goals.
- **Operate**
    - While some of the financial goals can be easily accomplished, others may require slightly longer processes. For instance, if the application requires architecture changes to minimize spend, it may take some time. The team would identity and execute processes to reach the financial goals.

## Team structure and relationship with FinOps

![FinOps Team Structures](https://video.udacity-data.com/topher/2021/March/603e451f_finsops-structure-teams/finsops-structure-teams.png)

FinOps Team Structures

As you can see in the above image, the FinOps team is cross-functional and mainly consists of 4 main teams

- **Engineering teams** are generally not trained to factor in cost along with other design goals such as performance, scalability, reliability, etc, that they have practiced for years. However, they are the ones who are making spend decisions as they deploy infrastructure and provision services in the cloud.
- **Business or Product owners** care about product costs and margins and can help the team make the right tradeoff calls between speed, cost, and quality.
- **Executive** sponsorship is essential to drive a cost-conscious culture in the organization as well as ensuring resourcing of the FinOps team.
- **Finance** can help by looking at the designs from a cost angle and work with engineering to make appropriate tradeoffs. Finance can also look at the cloud services usage data and identify opportunities for optimization. Procurement can consolidate the needs of engineering teams and negotiate cloud contracts with CSPs.
# Exercise: KPIs for Teams

## Team KPIs

Assume you are the CFO of your company and the executive sponsor for CCoE. Briefly describe that business to provide context for your responses. _Reminder: KPIs are measurable strategies that help businesses evaluate how effectively they’re meeting operational and strategic goals._ What business (K)ey (P)performance (I)ndicators would you create for each of your teams building on the cloud? Also in your response (**for each team)** how would you drive accountabilities and awareness so teams can take appropriate actions to improve the business KPIs?

Please continue to use the template `Exercise Template.docx` or `Exercise Template.txt` to record your responses. This is located under the Resources section of the course, in the top left of this page.

# Solution Exercise 3

## Sample Solution

I am the CFO of a ride-sharing company called RideWithUs. We provide 7 ride-sharing services for different classes of transportation ranging from scooters to black cars. There are 2 teams that build the common foundational services powering all of our service offerings while each service team is responsible for their own service built on top of common foundational services.

Business KPIs (Cost implies Cloud cost) for one such service X:

1. Cost per thousand rides of Service X
2. Foundational Service A cost per thousand rides of Service X
3. Foundational Service B cost per thousand rides of Service X

To drive accountabilities and awareness with specific goals, I’ll ensure that cloud-spend data is broken down to a fine grain level (utilizing resource tagging by departments, BUs, project teams, etc.) and custom reporting is available to each team to track/manage their individual costs. Further, I’ll create cost optimization KPIs for teams:

1. Reserved Instance utilization - target 90% (currently at 75%)
2. Right Sizing recommendations compliance - target 80% (currently 60%)

# Best Practice and Expert Intuition

![Best Practice and expert tips](https://video.udacity-data.com/topher/2021/July/60dde46d_tips/tips.png)

Best Practice and expert tips

## Executive Sponsorship

Experience has shown that organizations adopt cloud faster when there is a strong executive champion.

- The C-level sponsor needs to have a great understanding of the cloud and its benefits. It's a big change so the person needs to be empathetic as a top-down command and control approach won't work. The person's needs are involved, address any or all questions that may come up, and be able to get commitments behind the decisions made by him or her. Informal surveys of rank and file have reported a lack of executive understanding and appreciation of work involved to move to the cloud.
- The person needs to set a bold direction or goals and support people to realize the goal. As an example, a few years ago CIO of General Electric or GE set a goal for moving 50 apps to the cloud in 30 days. It seemed aggressive and unachievable. Eventually, the team moved 42 apps in 30 days but used the learnings to move 2000+ apps over the next 3 years.

## CCoE

- **Leader selection**
    - If you recall, CCOE is the center of the universe for all things cloud. Pick a CCOE leader who has strong EQ and people skills. The leader should be aware of the people, process, and cultural aspects of the change he/she is going to drive. If you recall, the CCOE leader interfaces with all BU heads and multiple functional organizations. Getting buy-in and commitment from all these organizations is a hard job given conflicting priorities. Typical roles leading CCOE could be CIO, one of CIO directs, Enterprise Architect, Leader of Program Management.
- **Member selection**
    - Pick members carefully - the most senior or qualified people aren’t necessarily the best choices. You need people who are hungry for new things, are go-getters, can try out different things and are not afraid to fail. They are change agents and command respect in their respective organizations for these skills. As you saw earlier, CCOE covers a variety of business and technical functions. Typically I have seen members join from infrastructure, operations, applications, finance, procurement, infosec, and program management organizations.

## DevOps culture

- **Start small and scale**
    - Changing your operating model and embracing DevOps culture is not a switch flip. You need to carefully plan it and slowly drive this from the ground up. I have seen this work in organizations where they pick a new workload and handpick a cross-functional team to work on it. The team will build practices and tools to optimize the delivery velocity and can deliver reusable automation and tooling for use by other teams.
- **Emphasize teamwork and collaboration**
    - You may also want to consider infusing other teams with members of this team to jumpstart DevOps philosophies. Remember to emphasize more teamwork and collaboration than on practices and tooling. DevOps at its core is a culture and mindset change.

## FinOps

- **Find an engineering savvy finance analyst**
    - A finance person with an engineering background or inclination could be an excellent fit on this team. He or she can gel well with the engineering team and significantly reduce the cost management burden from engineering teams who have to focus on delivering features.
- **Drive a cost-conscious culture**
    - Cost consciousness needs to be driven as a cultural practice across the organization. One way to do that is to - _Have the teams build and publish KPIs and score their own performance against them_. For instance, ride-sharing company Lyft started with a simple metric - cloud cost per ride as a start to bring cost awareness. Over time, they translated this simple metric to metrics for individual teams so each team can benchmark their own performance against other teams. This helped drive cost-consciousness in engineering ranks.
    - Another important point to remember - FinOps is not about cost reduction. it's about utilizing your cloud spend effectively to maximize business outcomes. If your spending is increasing commensurate with your business growth, it's a good thing.

## Tips and Advice for Success

- **Don't work incrementally. Make big bets**
    - Doing incremental work on the cloud isn't effective, you need to make big bets on the cloud to move fast. Recall the GE CIO example where she set an aggressive goal of moving 50 apps to the cloud in 30 days. Just dipping the toe in the water doesn't lead to any meaningful results for the business.
- **Be aware of 'frozen middle'**
    - The 'frozen middle' refers to middle management who become risk-averse over time and tend to slow down things. Handling the situation through rewards, recognition, and other motivational ways would line them up to support you.
- **Face inertia and resistance with reasoning and sincerity**
    - Changes are not easy to drive especially when the magnitude of the change is big impacting culture, processes, people, and technology. Don't resort to command and control leadership. Face the inertia and resistance on its face with reasoning and sincerity. This would require you to learn about the cloud as much as you can and to dive deep.
- **Trust your intuition**
    - Trust your intuition when faced with convincing data people will produce in support of their arguments. In one of my past experiences, I was shown data to show it is more cost-effective to run on-premises, and also there is a higher level of security risk when developers make a mistake in the cloud. I addressed the situation by diving deep and coming up with solutions to address the issues. We will discuss in the next chapter how a cloud governance model can mitigate the security risks in the cloud without compromising agility.
# Lesson Review

In this lesson:

- We spent time building an understanding of different components of Organizational capabilities
- We considered why Organizational Capability Building is important in the bigger picture
- We discussed what is the ideal target state you should be striving for and how can you get there.
- We learned how to evaluate your people and skills needed in the organization and bridge the skill gaps
- We identified the many changes your organization will need to adapt to reach the target state.
- We saw how DevOps and DevSecOps intersect to play a critical part in Organizational Capability Building
- We explored the role of FinOps and how it plays a part in Organizational Capability Building.
- Finally, we looked at some best practices and other expert perspectives on this topic

# Glossary

|KeyTerm|Definition|
|---|---|
|CCoE|A virtual team consisting of people from different functions such as Engineering, Operations, Finance, Business, and Security. CCOE gets its sponsorship from a C-level leader typically CIO or CTO.|
|Cloud Financial Management|A new cultural practice where finance, procurement, engineering collaborate to manage cloud spend.|
|Continuous Integration and Continuous deployment|An engineering practice where the code to deployment pipeline is fully automated.|
|DevOps|A culture where Development and Operations team collaborate to roll out new features quickly while keeping uptime and security.|
|DevSecOps|A culture where Development and Security and Operations team collaborate to roll out new features quickly while keeping uptime and security.|
|FinOps|A new cultural practice where finance, procurement, and engineering collaborate to manage cloud spend.|
|Functional Silos|Isolated teams that interact with each other formally.|
|Procurement|A team responsible for procuring hardware or software.|
|Shift-left security|When security principles are applied earlier in the development cycle.|
|Sphere of Responsibility|Areas or domain of responsibilities.|
|Target State model|A desired state of your organization when they have moved to cloud.|
|Technical Debt|The overhead price engineering teams pay for making any change due to past shortcuts or workarounds.|
# Further Learning and Reading

- [Using CCOE to transform the entire enterprise(opens in a new tab)](https://aws.amazon.com/blogs/enterprise-strategy/using-a-cloud-center-of-excellence-ccoe-to-transform-the-entire-enterprise/)
    - Milin Patel, the Principal Architect and Co-Founder of Rearc and formerly the Head of DevOps of Dow Jones, talk about Dow Jones’s move to the cloud and DevOps, and the organizational changes this shift inspired
- [FinOps: Collaborative, Real-Time Cloud Financial Management(opens in a new tab)](https://www.finops.org/)
    - Real-world stories, expertise, and inspiration for and by FinOps practitioners on cloud financial management best practices.
- [What is Target Operating Model?(opens in a new tab)](https://thinkinsights.net/strategy/tom-what-is-a-target-operating-model/)
    - Learn more about the Target operating model (TOM). It is a blueprint of a firm’s business vision that aligns operating capacities & strategic objectives. It provides an overview of the core business capabilities, internal factors, & external drivers, strategic & operational levers, organizational & functional structure, technology, & information resources of a company.
- [Taking target state modeling to the next level(opens in a new tab)](https://www.capstera.com/target-operating-model/)
    - Clarifying misconceptions and misunderstanding of the Target Operating Model.
- [What is DevSecOps?(opens in a new tab)](https://www.redhat.com/en/topics/devops/what-is-devsecops)
    - Now, in the collaborative framework of DevOps, security is a shared responsibility integrated from end to end. It’s a mindset that is so important, it led some to coin the term "DevSecOps" to emphasize the need to build a security foundation into DevOps initiatives.
- [How Zendesk started CCOE to manage overall cloud program and cloud spend governance(opens in a new tab)](https://www.youtube.com/watch?v=ha7MIKaYkR0)
    - When implemented well, the CCoE acts as a bridge, connecting all departments that use, measure, or fund your cloud operation. This video discussed the journey.

# 4. Cloud Governance Model
# Cost Governance

**On-Prem**

- Capex, capital expenditures on a yearly basis
- Yearly budget and procuring hardware and software licenses (fixed)
- Finance and Procurement have full spend control

**Cloud**

- Opex, operational expenditures as needed to run business
- Dynamic spend as cloud resources are spun (variable)
- Engineering gets control

## Governance gives you a handle on cloud costs

Engineering traditionally has not been trained for this model; it is common to leave resources running even when not in use, which will incur charges.

If you don’t put governance, you’ll likely end up with runaway cloud costs. Finance and procurement still have a role but _now need to collaborate with engineering to ensure the optimal usage of company spend._

This is a new mindset for many organizations.

---

## Cost factors

![Cost Factors](https://video.udacity-data.com/topher/2021/March/6042b913_cost-facotrs/cost-facotrs.png)

Cost Factors

Here are some major cost factors that impact your spending.

- **Idle Resources**
    - We talked about engineering getting control of procuring resources. Unfortunately, On-prem SDLC habits carried to the cloud would incur wastage. E.g. developers leaving the dev/test resources running in the evenings and weekends cost $ on the cloud. You can implement a tool or automation in your cloud environment to shut down idle resources
- **On-demand instances**
    - On-demand instances are the most expensive. Cloud providers allow you to pre-buy capacity at a significant discount. For instance, AWS offers Reserved Instances and Savings Plan. Once you pre-buy capacity, you use it or lose it. So the challenge is how do you estimate how much to buy? One of the ways you can estimate it is by looking at historical usage and collecting forecasted usage from your teams. Once you pre-buy, your cost governance model should aim to drive high utilization of this capacity.
- **Rightsizing**
    - There is also a tendency among developers to use the largest resource size (more expensive) when a smaller resource size (less expensive) can do the job. Not that they want to waste the company's money but lack of data may lead them to make wrong choices. You can implement a tool or automation to collect data from cloud resource usage and utilize this data to make sizing decisions. The process is called Rightsizing.
- **Spot Instance**
    - Spot instances are the excess capacity cloud providers have that they offer in the spot market at a steep discount. However, spot instances can be taken away programmatically with a 2 min warning. This requires architecture changes to accommodate this interruption and may not work for all types of workloads. Another cloud innovation is Serverless services where you don't need to spin up instances and pay for, only the time when your code runs. Serverless also requires architectural changes to your apps. You need to educate your teams and see if there are opportunities to utilize spot instances or Serverless.

### Quiz Question

Think about the various factors related to cost and how those can be addressed. Match cost factors with the right solutions

These are the correct matches.

#### Cost Factors

#### Solutions

Idle compute instances

Automation to shut down resources when not in use

On-demand vs Reserved Capacity

Collect data to plan for reserved capacity

Inappropriately sized resources

Rightsize instances based on usage data

On-demand vs spot instances

Explore if your applications can be rearchitected to take advantage of this cost saving instance type

## Where to Start

![Teams and the Cloud](https://video.udacity-data.com/topher/2021/March/6042bb76_teams/teams.png)

Teams and the Cloud

This is an important point that business leaders typically ignore. And that is the need to train all your teams with targeted cloud education. In the image above, you can see this represented.

- **Engineering** - _Cloud Economics_
    - Engineering teams are used to optimize for performance, reliability, scalability, etc but are not used to think about the cost since the cost was never a consideration in the on-prem world.
- **Finance** - _Cloud Technology_
    - Finance teams need to understand cloud technology terms and cost factors so they can team up with engineering to optimize spend.
- **Procurement** - _Cloud Agreements_
    - Cloud agreements are very different in nature than hardware and software licensing agreements so unless the procurement team is also aware of cloud basics, they won't be able to structure the agreements in the best interest of your organization.

`Assess the skill gaps and address them first, before you start addressing tech and process gaps with a cloud spend governance model.`

## Framework for cloud spend governance

Once you have addressed the skills gap, you are now ready to put a governance model for your organization.

![Framework for cloud spend governance](https://video.udacity-data.com/topher/2021/March/6042bbee_framework-for-cloud-governa/framework-for-cloud-governa.png)

Framework for cloud spend governance

Think back to the **FinOps** team structure from an earlier lesson. That would be a perfect place to start defining the governance model. Alternatively, a subteam within **CCOE** consisting of finance, procurement, and engineering can also be chartered to do the same. in the image above, you can see both represented in the center of the diagram, with several elements of the framework connected to them

- **Monitor spend, usage, and forecast**
    - The first step is to ensure you have a good cloud spend measurement system in place. This can be accomplished by implementing a tool or buying a third-party tool that would help you with spend usage, allocation, forecasts, and showback/chargeback across departments.
- **Negotiate enterprise discounts**
    - Once you have the usage data and 3-year spend forecast, use it to negotiate an enterprise discount with your cloud vendors. Set up your CCoE (Cloud Center of Excellence) and forecast cloud spend for 3 years. Stakeholders: Finance, Procurement, Eng
- **Allocate spend budgets by Department/BU**
    - Next, allocate the spending budgets across departments. The tool you implemented should help you with allocation, reporting as well as monitoring of spend against the budgets and can alert you when spends are trending to go over budget.
- **Implement spend policies and controls**
    - Ensure your organization policies and controls are implemented in your cloud environments through automation so you can manage spends on a continuous basis throughout the year, and get alerts/notifications, etc when actuals are trending to exceed budgets. For instance, You may want to implement controls in CI/CD to prevent developers from spinning up expensive SKUs in the developer environment.
- **Publish business KPIs and reward systems**
    - Build a cost-conscious culture, you can publish business KPIs and encourage teams to drive continuous improvements. You may also consider rewarding teams who take special measures to drive the KPIs.
    - **Example**: For instance, Lyft, a well-known rideshare company started with cloud cost per ride as a simple KPI and later defined fine-grain KPIs to make them relevant to individual teams.
# Exercise: Cost Management

## Cost Management

Assume you are the CIO of a company that is on its journey to the cloud with a cloud service provider(CSP). You review monthly invoices from your CSP and notice the bill is rising 20% month over month. What steps would you take? Include at least 4 or 5 possible steps.

Please continue to use the template `Exercise Template.docx` or `Exercise Template.txt` to record your responses. This is located under the Resources section of the course, in the top left of this page.


# Solution Exercise 1

## Sample Solution

Proposed Steps:

- Setup CCOE (if not already there) and charter them to define policies and controls to optimize spend.
- Analyze the usage data by BU/Dept/projects and usage type (Dev/Test/Prod). If the usage data is not available, implement a cost management tool to get fine-grained spending reporting.
- Check for wasted resources by examining data. E.g. Resources tagged as Dev for Project A incurring charges over weekends. Ask Operations to implement tools/automation to shut them down when not in use.
- Ask the teams if they have gone through an exercise of right-sizing instances using data provided by the tool.
- Identify opportunities to pre-buy capacity based on usage data from the tool.
- Ask teams if they can make architectural changes to use spot capacity (e.g. spot instances(AWS), Spot VMs (Azure), Preemptible VMs (Google)), and serverless architectures.
- Publish business KPIs and align team rewards with business KPIs

# Security Governance

![Shared Responsibility Model](https://video.udacity-data.com/topher/2021/March/604a4fa1_shared-resp/shared-resp.png)

Shared Responsibility Model

## Security responsibilities in the cloud

In the first lesson, we discussed the differences between on-prem, IaaS, PaaS, and SaaS in terms of who manages what components of the technology stack. The same model applies for managing security where "_security of the cloud_" is cloud providers' responsibility but "_security in the cloud_" is yours.

- There are some clear areas of security ownership such as applications, data, devices, cloud accounts and identities belong to the **customer(you)**.
- However, there are some grey areas in the **middle** where you need to dive into details of the services you use from your cloud provider and make sure you are carrying out your part of the responsibility.
- All **cloud providers** take a lot of security headaches away from you. They also provide you security-related services that you can use to do your part and secure the entire application stack.

## Security governance is a 3 layer model

![3-Layered Security Model](https://video.udacity-data.com/topher/2021/March/604910a4_3layers/3layers.png)

3-Layered Security Model

The graphic at the topic of the page goes into granular detail about what exactly is and is not provided. In a more simplified model, the best way to think of security governance is a **3 layer model**

- **Infrastructure security** is owned by the **cloud provider**. This includes securing compute, storage, and network resources. However remember the configuration of these resources is still owned by you and if not configured properly, can lead to potential security exposures.
- **Application security** is entirely owned by **you**. This includes application-specific security controls and data classification. We earlier talked about DevSecOps as a culture that fundamentally resides in this layer. This layer is supported by
- **Platform Security** as the middle layer, if done right can make things much simpler for DevOps teams. This layer includes foundational controls such as identity and access management, logging, auditing, automated response, and remediation. If you recall CCOE functions, this is one of the areas where CCOE can help by providing code, templates, tooling, and other assets. The more we can abstract from application teams in terms of foundational controls as well as common patterns we see across applications, the faster the application teams move. This middle layer is typically owned by the central cloud engineering team.

## Security is everyone's responsibility

Security governance isn't just a set of technologies and frameworks. While frameworks such as CIS benchmarks, NIST CSF, etc. are great to implement these frameworks alone won't help you achieve your security objectives.

You should think of security governance through the lens of your

- People
- Process
- Technology

A culture of "Security is everyone's responsibility" goes a long way in establishing good security governance.

### Role of InfoSec professionals

This role needs to evolve from being a gatekeeper to an enabler of the business where they provide automated controls and policies, work with developers to implement automated response and remediation of security incidents. They have a key role to play in CCoE to accomplish these objectives. This is the only way for Infosec to scale and ensure robust security governance.

# Exercise: Security Checks and Guardrails

## Security Checks and Guardrails

If you have a CI/CD pipeline in place for your cloud projects, find out what type of security checks are done in the pipeline. Additionally, describe any security guardrails that are in place.

If you don’t have a pipeline in your organization, how would you design a CI/CD pipeline with proper security checks and guardrails? List and describe specific security checks and guardrails you’d consider _(e.g. for containerized environments you may want to scan all container images through a tool)_

Please continue to use the template `Exercise Template.docx` or `Exercise Template.txt` to record your responses. This is located under the Resources section of the course, in the top left of this page.

# Solution Exercise 2

## Sample Solution 2

I’d design the pipeline with the following automated checks:

1. Security configuration checks (all application component configurations e.g. app, web server, DB, etc against guidelines from CIS, OWASP, etc.
2. Static code analysis
3. Dynamic Code analysis
4. Security assurance to confirm all high priority security issues have been addressed in the current build before moving to deployment
5. Threat modeling done
6. Penetration Testing completed
7. Security compliance checks passed
8. Scan container images for malware

Guardrails:

- A comprehensive set of guardrails can be implemented with help from the security team, but here are a few common ones:
- Prevent storage bucket public access - by automatically making it private or warning user when he accidentally creates a bucket with public access
- Secret keys in code - warn users and ask them to put secrets in vaults provided by cloud provider
- Configuration changes - e.g. changed security group settings that may open up internet ingress
# Compliance Governance

As discussed in the video and also demonstrated in the image below, it useful for us to understand the big picture of how Governance, Risk Management, and compliance are related.

### What is required to meet your compliance requirements in the cloud?

- **Risk**
    - Every organization has risks such as financial, legal, reputation, or cybersecurity-related.
    - Risk management function provides the risk parameters to the governance function that needs to ensure that policies, controls, and processes are designed and implemented to operate within risk boundaries.
- **Compliance**
    - Compliance function ensures that external and internal standards are adhered to. These could be industry regulations such as PCI DSS, HIPAA, or Hitrust. These could also be your own organizational standards or policies that may have been designed to mitigate risks or align with your business objectives. These standards or policies typically come from risk management functions.
- **Governance**
    - The compliance function needs support from governance to continuously monitor compliance and report or act on compliance violations for both externally or internally defined standards and policies.

![Governance, Compliance, and Risk](https://video.udacity-data.com/topher/2021/March/6042af79_gover/gover.png)

Governance, Compliance, and Risk

---

## Guardrails

Guardrails are simply preconfigured rules for

- Security
- Compliance
- Cost management

### Preventive and Detective Guardrails

![Guardrails](https://video.udacity-data.com/topher/2021/March/6049120f_sec-comp-guard/sec-comp-guard.png)

Preventive and Detective Guardrails

They can be applied to any hierarchical level in the organization. You can see in the image above what this looks like:

- **Preventive guardrails**
    - Preventive guardrails are configured to enforce and prevent any violation. They disallow actions that could lead to a policy violation. For instance, if you don't want any storage bucket to be exposed to the public read access on Internet, you can disallow the creation of a storage bucket unless proper protection is on. Another example - to manage cost better, you may have a guardrail that may disallow the creation of certain types of compute instances, since they are expensive, in developer accounts.
- **Detective guardrails**
    - Detective guardrails are configured to detect the violations and report them in a dashboard or other mechanisms. You may have a detective guardrail that senses non-compliant behavior in resource configurations and report it. For instance, you may have a list of prohibited applications for which you may want to create a detective guardrail to detect if any application from that list gets installed. Upon detection, you may report it in the dashboard and also take an action to shut down the compute instance on which the application got installed.

CSPs provide mechanisms to create preventive and detective guardrails. There are many third-party and open source products that make it easier to manage compliance extending the native capabilities of the CSP.


# Governance at Enterprise Scale

## Enterprise-scale adoption

### Cost Management

Cost Management requires a different approach. In the OPEX-driven model, Your engineering teams are taking the role of procurement and finance when they spin up resources in the cloud.

- Because the cloud is code and API-driven, you need mechanisms to manage and optimize cost without putting barriers on developers' agility.
- Manual processes simply won't work with hundreds or thousands of developers in your company.

### Security and Compliance

- The shared responsibility model may cause confusion around grey areas leaving you exposed.
- Your developers far outnumber the Infosec staff you have.
- Manual security check processes would kill developer agility.
- Manual processes don't scale well and are error-prone.

Cloud Service Providers understand these challenges and provide technical solutions to design and customize a governance model.

## Scale Challenges

As more teams start building on the cloud, teams need to be responsible for managing their own resources.

### Challenges to scaling operations into the cloud

- **Resource isolation**: Businesses have to make sure different users, business units and project teams are not impacting each other. They need their own resource containers to keep them isolated from others. This can be done through separate cloud accounts or subscriptions. But managing the growing number of accounts or subscriptions becomes challenging unless there is a way to organize them.
- **Cost Management**: Each business unit or project team may have a budget that needs to map to cloud accounts or subscriptions they own. Managing cost allocation, reporting and ensuring teams don't exceed the budgets becomes a challenge very quickly in organizations that are growing on the cloud.
- **Security and Compliance**: Ensuring security and compliance of these accounts and subscriptions when you have limited security and compliance professionals but more developers become challenging. Manual methods don't scale.
- **Account provisioning**: As new account or subscription requests come in, how do you make sure they come equipped with proper security, compliance, and cost management guardrails? Manual methods would be error-prone and won't be able to scale.

---

## Landing Zones

### What is a Landing Zone?

- **Pre-configured cloud environment**: Landing Zone is a way to organize and manage your cloud accounts. You can organize all of your cloud accounts in a hierarchy and configure controls and policies at any level - organization-wide, by business unit, departments, or projects. This makes sure that the accounts under a particular hierarchical level have controls and policies prescribed for that hierarchical level. For instance, a department that deals with personally identifiable data may want to enforce PCI DSS controls for all accounts in that department.
    
- **AWS accounts, Azure subscriptions, GCP projects**: All cloud providers provide mechanisms to create a landing zone where you can pre-configure accounts with your organizational policies, guardrails, security and compliance reporting tools, etc. Each cloud provider uses different terms for accounts that are nothing but isolated resource containers. AWS calls them accounts, Azure calls them subscriptions, GCP calls them projects. In essence, they all act as isolated resource containers.
    

### What does a Landing Zone deliver?

- **Resource isolation**: By organizing accounts in a hierarchy you can accomplish isolation at any level such as project, department, BU, etc. This drives accountability to each of these organizational units.
- **Cost management**: By allocating budgets to any organizational unit, you can ensure all accounts under that organization unit stay within the budget limits. We will see how this works later.
- **Security and compliance**: Each account comes pre-provisioned with security, compliance, and other organizational policies so your developers can be productive from the instant the account is provisioned.
- **Account provisioning**: Account provisioning can be completed automated as well. Once an account creation request is approved, landing zone automation will pre-configure the account with appropriate guardrails and disburse it to the requester almost immediately.

![Landing Zone typical setup](https://video.udacity-data.com/topher/2021/March/6049130e_landing-zone/landing-zone.png)

Landing Zone typical setup

The image above represents a typical setup of a landing zone in large organizations. This setup is described below.

## Landing Zone typical setup

### Business unit IT

Business OUs and Sandbox OUs are typically managed by business unit IT owners. In some cases, I have to see Sandbox OU being assigned to a central cloud engineering organization.

### Foundational OU

Since the Landing zone allows you to organize accounts in a hierarchy, you may want to create a foundational OU or organizational unit that will serve all business units. You can see this in the center of the image above, in the foundational OU, you may have accounts with security-related functions such as logging, auditing, forensics, and another security tooling. This gives visibility and control to InfoSec professionals across all accounts in the organization.

- You may also run some shared infrastructure services such as network configurations for all accounts.
- Security accounts have controlled access to Infosec professionals
- Similarly Shared services accounts are typically managed by central cloud engineering organizations.

### Business Units OU

Business Units OUs get set up over the foundational OUs. Each BU may have differing security or compliance requirements. However, this mechanism allows BUs to be different yet inherit common foundational security and compliance controls.

### Sandbox OU

We earlier talked about Sandbox accounts. They also come pre-provisioned with the right cost and security controls.

## Governance in Action

As you can see in the image below, **Security** and **Compliance** guardrails flow down through the hierarchy, as do the **budgets**. For instance, you may assign _$500K_ to Operations and $_300K_ to engineering, leaving $_200K_ to HR. The guardrails system would warn if any cost bucket is running too hot and likely to exceed budge.

## Example

![Governance in Action](https://video.udacity-data.com/topher/2021/March/60491382_gov-in-act1/gov-in-act1.png)

Governance in Action Flow of guardrails and budgets

## Exceeding budget scenario

Imagine that **Project 3 by team B** exceeds the budget. The guardrails system would warn if any cost bucket is running too hot and likely to exceed budget, which has an impact on **Engineering** as well as **Operations** as a whole.

In the image below, you can see the effect on multiple organizational levels as the Project 3 cost overrun flows back up(red).

You may want to put a guardrail to restrict or throttle the creation of new resources in this situation. Just like security and compliance guardrails, the cost management guardrail can be put at any organizational level.

![](https://video.udacity-data.com/topher/2021/March/6049138a_goc-in-act2/goc-in-act2.png)

Governance in Action guardrails can control budget overuns

## Automate

The cloud is that it allows you to automate a big chunk of your governance model. So for example,

- **Spend Governance**: If the spend is likely to exceed the assigned budget in an account, automation can alert the account owner so he or she can take appropriate actions to stay within budget. You can even put preventive automation that restricts engineers from spinning up expensive resources in the CI/CD pipeline itself.
- **Security Governance**: You can put preventive automation for security too in the CI/CD pipeline, which will prevent insecure code to get deployed. Automation can also be used for not only detecting anomalous activities but also responding to them with a user-defined action or set of actions.
- **Compliance Governance**: Many compliance rules can be automated so any deviance from compliance guardrails can be flagged and appropriate actions are taken to bring the system back on track. For instance, HIPAA has many privacy and security rules that can be automated to keep your systems HIPAA compliant continuously.

Developers who are not financially savvy, or have the security of compliance expertise can _freely innovate_ knowing the system would always keep them within the guardrails. Finance, security, and compliance professionals aren't running around conducting reviews and audits because they can now trust the automation will take care of it.

## Mechanisms to help with Governance

There are many powerful mechanisms and tools provided by your CSP in the cloud to help you build automation for practically any use case.

### Tagging:

Tag is a metadata for a cloud resource. You can use tagging for multiple use cases. For instance, you can tag resources for a nightly backup. Tags can also be associated with projects or departments for proper cost allocation. Tags also allow you to create fine-grain access control policies for security and compliance.

### Identity and Access Management (IAM:

Cloud providers provide their own IAM system that can be used to define identities and control access to cloud resources. You can use tagging to build IAM policies to provide attribute-based access controls. For instance, you can build a policy that allows user A to administer only those organizations units that have a tag X.

### Configuration Management:

Services such as AWS Config or Azure policies allow you to detect changes to your configuration. They can be used for many purposes including auditing and compliance. For instance, you can specify a rule as a detective guardrail that the service can flag, such as ports being open on an instance, allowing you to take any action on the resource to bring your system back on track.

### Policies:

Mechanisms such as AWS Service Control Policies and Azure Policies allow you to apply organization-wide guardrails. For instance, you can define a policy to disallow resource creation in certain regions.

### Logging and Monitoring

Logging and Monitoring services such as AWS Cloudtrail, AWS Cloudwatch, Azure Monitor, Azure Application Insights allow you to record events for security incident management and forensics and monitor your environment for anomalous activities.

### Serverless Services

Serverless Services are services such as AWS Lambda or Azure Functions that allow you to write your own rules in response to events. You can use them to implement an organizational policy. For instance, if the event is related to a configuration change on a resource you can write a rule to either shut down the resource or quarantine it.

### CSP Native services

CSPs also provide many services for cost management, security, and compliance that you may want to use out of the box or build upon them. For instance, AWS Trusted Advisor or Azure Advisor provide a thorough analysis of your environment to help you improve security posture and find cost optimization opportunities.


# Exercise: Workflows, Costs, Accounts, & Security

## Workflows

Oftentimes, when a new user requests a new account(e.g. AWS or Azure, Google, or IBM), it can come with a budget envelope of $2000(or some amount). There may be warnings or throttles as you reach that limit. This is the equivalent to an enterprise providing a debit card to its employee with $2000 in it.

Does your organization have a self-service portal to request/open a new cloud account? If yes, investigate and list the workflow steps operating behind the scenes that put cost boundaries, provisions security guardrails, and ensure compliance of the account. List the specifics to the extent you can discover them (e.g. each account under $2000 is automatically provisioned else goes to manager approval).

If you don’t have one, how would you go about designing one? List specific workflow steps you’d consider putting in prior to provisioning new accounts.

Please continue to use the template `Exercise Template.docx` or `Exercise Template.txt` to record your responses. This is located under the Resources section of the course, in the top left of this page.

## Solution

- Provide a list of account types for users to pick from. If the account type picked is of type “Sandbox”, immediately provision it with required policies and guardrails and time/budget limits. Developer can start using it right away
- For non-sandbox accounts, review the requested budget and purpose. If it exceeds automatic approval limits set by the BU head, send it to the manager’s approval.
- Upon approval, do the following:
    - Create a baseline architecture in the account, configure Identity and Access Management policies, drop pre-defined service configurations such as VPC, code repositories, security tools, storage buckets, etc.
    - Associate the account with the GRC tool so the account can be monitored for compliance
- Enable cost monitoring so as to warn users when account limits are closed.
- Make the account available for use.
# Best Practice and Expert Intuition

- **Automate everything**
    
    - The beauty of the cloud is the power of API and 100+ services at your disposal to automate anything. Automation allows you to
        - scale
        - reduce human errors
        - drives agility.
    - Many organizations such as Netflix, Amazon, CapitalOne, GE Appliances have built the automation we discussed to run cost management, security, and compliance on auto-pilot allowing their teams to innovate fast while keeping them secure and compliant.
- **Don't forget people, process, and culture**
    
    - Good governance is not just technology and automation. Its also the people, process, and culture that plays a key role in defining and implementing a governance model. For instance, cost governance without a cost-conscious culture would lead to sub-optimal business outcomes.
    - **Example**: Lyft, the ride-sharing company, came up with creative ways to publish the cloud cost numbers individualized by teams to create awareness. This resulted in a desire to improve when team managers saw other teams doing better than them.
- **Get away from IT governance mindset**
    
    - IT governance in traditional IT organizations is gated by people, tickets, manual approvals, etc slowing things down. Cloud changes the model completely. You put your organizational policies and processes as code in the environment using cloud services and eliminating humans and manual actions from the mix. Net result - you move fast.
- **Focus on CCoE**
    
    - Constituting your CCoE with the right leader and members is very important as I discussed in the previous lesson. In addition to being the cloud champion for the organization, CCOE helps you build and implement the right governance model. From my own experience in working with a large enterprise, I saw little progress when the CCOE leader wasn't a good fit for the role. A leadership change was made after several months, and things began to improve significantly.
- **Governance is dynamic**
    
    - Governance is never one and done. Your organizational context keeps changing including the markets, customer needs, business priorities. Accordingly, your governance model should keep evolving to maximize alignment with the business objectives while minimizing risks. Remember governance exists to serve the business not restrict it. The best part is - it's all in software so can be changed easily. Your employees feel good that they don't have to worry about things that are beyond their competencies.

# Lesson Review

## Lesson Review

Let's quickly recap what we learned about

- The definition of Governance
- Why is governance important
- Problems such as cost overruns, security compromises, compliance violations, etc you may run into if you don't put a good governance model in place
- Cost management and the cloud spend governance model
- Shared responsibility model.
- Security governance through a layered approach.
- The relationship between Governance, Risk Management, and Compliance functions.
- Preventive and detective guardrails to monitor and manage compliance.
- Finally, we showed you how to build and operate your all-up governance model by pre-configuring your cloud environment using services provided by the cloud provider.
# Glossary

|KeyTerm|Definition|
|---|---|
|Application security|Entirely owned by the customer.|
|Cloud governance|A set of policies, controls, and processes defined to ensure the organization can accomplish those objectives within well-defined risk boundaries.|
|Compliance|When one has to comply with certain rules, standards, or regulations|
|Data sovereignty regulations|Regulations associated with keeping data in the country|
|Detective guardrails|configured to detect the violations and report them in a dashboard or other mechanisms|
|Idle Resources|Resources that are assigned to you and getting charged but not being used|
|Infrastructure security|Owned by the cloud provider|
|KPI|Key Performance Indicators|
|Landing Zone|A pre-configured account structure|
|Platform Security|The middle layer, if done right can make things much simpler for DevOps teams.|
|Preventive guardrails|configured to enforce and prevent any violation.|
|Rightsizing|Ensuring the compute size is properly selected to meet the needs of the workload|
|Shared responsibility|When responsibility is shared between the customer and the cloud provider|
|Spot Instance|A compute instance type offered by cloud provider at steep discounts but comes with certain conditions|
# Further Reading and Learning

[Establishing your cloud presence: Governance and Risk in the cloud (opens in a new tab)](https://aws.amazon.com/blogs/mt/governance-risk-and-compliance-when-establishing-your-cloud-presence/): Business and technology leaders express the need to bring new products and services to market quickly, but that is also secure. At the same time, they must maintain a resilient environment while adapting workloads to changing business needs over time. Read about best practices to help our customers plan their cloud environments to meet these security, scalability, and adaptability requirements.

[Standard business and complex business Governance guides(opens in a new tab)](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/govern/guides/): The actionable governance guides in this section illustrate the incremental approach of the Cloud Adoption Framework governance model, based on the Govern methodology previously described. Learn to establish an agile approach to cloud governance that will scale.

[Case Study: McDonald's digital transformation(opens in a new tab)](https://www.ciodive.com/news/mcdonalds-cloud-ETL-talend-digital-transformation/523132/): Abhi Bhatt, director of data and analytics at McDonald's tells the story of McDonald's, whose supply chain is one of the largest in the world and every day goes to work filling 71 million orders across 6,000 menu items, according to

[Cloud Financial Management(opens in a new tab)](https://troposcale.com/cloud-financial-management/): According to studies, 35% of cloud spend is wasted. Spot wasting yours by adopting proven cloud financial management practices.

[Managing cloud financials - Lyft case study(opens in a new tab)](https://www.youtube.com/watch?v=ChupgIbZr5Q): See a video of guest speakers from Lyft sharing how they’ve accelerated cost optimization and improved cost visibility while growing their business with cloud computing.

[How Zendesk started CCoE to manage overall cloud program and cloud spend governance(opens in a new tab)](https://www.youtube.com/watch?v=ha7MIKaYkR0): When implemented well, the CCoE acts as a bridge, connecting all departments that use, measure, or fund your cloud operation. This video discussed the journey.

[Governance Guides(opens in a new tab)](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/govern/guides/): These actionable governance guides illustrate the incremental approach of the Cloud Adoption Framework governance model, based on the Governance methodology.

