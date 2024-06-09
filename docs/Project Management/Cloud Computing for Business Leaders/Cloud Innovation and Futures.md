---
sidebar_position: 4
---

# 4. Cloud Innovation and Futures

## Lesson Overview

The key reason people move to the cloud is for business agility and driving innovation in the cloud. In this lesson, we will look at some of the capabilities of the cloud that you can utilize to drive business innovation.

- We will start by looking at some business trends and see how the increased pace of innovation is driving disruption in all industries. Needless to say, you need to increase your own pace of innovation to avoid getting displaced or disrupted.
- We will discuss how some of the characteristics of cloud are well suited for innovation
- We will look at some of the major cloud services that are being utilized to drive innovation. We will also cover some typical use cases across all industry segments that are apt for these cloud services

Some of these innovations are shown below and will be the focus of this lesson

![Innovations in the cloud](https://video.udacity-data.com/topher/2021/March/605e2517_innovationscc/innovationscc.png)

Innovations in the cloud

## Case Study

After we complete the main elements of this lesson on innovation, we are going to do a deep dive into a real case study, where everything we have learned throughout the course comes together with a familiar organization that reinvented their businesses with the cloud.

# What is cloud innovation and why is it important

## What is cloud innovation and why is it important?

![S&P 500 Rolling 7-year average](https://video.udacity-data.com/topher/2021/March/605140a4_rolling/rolling.png)

S&P 500 Rolling 7-year average

### Changing landscape of S&P 500 companies

By 2027, the average company will last just 12 years on the S&P 500, according to Innosight’s biennial corporate longevity forecast. In the image above, notice the area highlighted in black; at the current and forecasted turnover rate, the Innosight study shows that nearly 50% of the current S&P 500 will be replaced over the next ten years.

### Compare the top 4 companies in 2020 vs 2000

![Rise of tech companies](https://video.udacity-data.com/topher/2021/March/6051f43a_rise/rise.png)

Rise of tech companies

What these top 4 firms all have in common are powerful digital platforms that provide the scale and scope to expand into new growth markets and geographies at speeds never before possible.

What does this tell us? The impact that technology platforms have on consumers as well as enterprise businesses.

`All companies are becoming technology companies!`

### Software is eating the world

Marc Andreesen(Wallstreet Journal) rightly said - Software is eating the world.

- The **music** industry is ruled by the likes of _Apple iTunes, Spotify, Pandora_.
- The **video** service industry is led by _Netflix_ and _Amazon_ prime video
- The largest **bookseller** Amazon is a software company that has even digitized books through Kindle.
- **Photography** is all digital and software-driven.
- **Movie** production company _Pixar_ was a software company bought by _Disney_ to stay relevant.
- **Transportation** companies _Uber_ and _Lyft_, both of them also really technology companies, complete more rides than all taxi companies in the US combined without owning a single taxi.
- **Vacation rental** company _Airbnb_ provisions more rooms per day than the 100-year-old Hilton chain.

Whatever business you are in ...whether it is Healthcare. Media and Entertainment, Retail, Industrial and Manufacturing, Mining, Agricultural or something else - you need to go digital and you need to innovate to stay on top or risk disruption.

Cloud gives you the digital platform to innovate.

### Why innovate in the cloud?

There are certain characteristics of the cloud that make it an appropriate platform for innovation

- **Global reach:** Innovation requires experimentation. Conducting experimentation in a certain geographic market won't be easy if you need to acquire resources in that region. With the cloud, you can pick a region or multiple regions and run your experiments programmatically.
- **Low cost of experimentation**: Your experiments are time-bound and may run for a few weeks or months. If they succeed great, but if they don't you can shut them down and owe nothing. This way you can fail fast, a key attribute of rapid innovation.
- **Speed of Provisioning**: If your experiment succeeds in the test market, you can quickly expand into other markets utilizing the global presence of cloud providers. Since everything is code and API-driven and you have access to a virtually unlimited pool of resources, the speed of provisioning gives you a significant advantage in the cloud.
- **Access to a variety of resources**: Cloud providers offer a variety of computing, storage, network, and higher-value services. The variety of resources you may need access to at the same time would have been difficult to acquire to conduct a timely experiment.

**Example**: If your experiment requires AI and Machine learning that's best done using the latest GPUs, a special type of processor, is readily available on the cloud along with other resources. The GPUs would have been difficult to acquire otherwise.

# Cloud Innovation Services

## Leading-edge innovation tools

There are numerous major service areas and domains where cloud providers continue to innovate to provide you the best services to help you innovate in your business faster.

For each of these topics, we will dive deeper and see what it is, how it can potentially deliver strategic value to you, and take a look at typical use cases across multiple industries.

- Serverless computing
- Containers
- Data Lake and Analytics
- Internet of Things(I.O.T.)
- AI and M.L.
- Blockchain as a service
- Edge computing
# Serverless

- No-server management. Provisioning, patching, and all I.T.-related activity of computing is handled by the CSP.
- Scaling is automatic
- Built-in fault tolerance

## Pay for Value vs. Pay for Use

One of the most valuable elements of serverless computing is something called Pay for Value

- **Pay-for-value**: No resource needs to be provisioned by you so there is no risk of wasted money due to idling or underutilization of resources. In the pay-for-value model, you upload your application to the cloud and only pay for the time when your application runs. You don't own compute instance so are not liable for paying for it.
- **Pay-for-use**: If you spin up a compute instance in the cloud for running your application. You are paying for computing instances by the minute regardless of whether your application is running or not. This is because the compute instance is yours until you shut it down.

## Real-World Examples

- **Function as a Service**
    - e.g _AWS Lambda or Azure Functions_
    - Compute services where you upload only your application code and pay for only the time when the code runs.
- **Datastores**
    - e.g _Amazon DynamoDB, or Azure SQL DB serverless_
    - Data Stores don't need any maintenance such as scaling, backup, recovery, etc, from you.
- **Application integration services**
    - e.g. _AWS API gateway or Azure API gateway_
    - App integration services allow you to focus on developing your app components and connect the components using app integration services. For instance, you can configure API Gateway to connect the client to the backend through APIs reducing a huge burden on developers

## Use Cases

Now that you understand the basic concept of Serverless, let's look at how different industries are using Serverless Computing.

- **Web applications** that can scale up and down with traffic are ideal for serverless. No need to fear crashing with sudden surges of traffic.
- Serverless computing is **event-driven a**nd can be triggered from a variety of triggers such as pub/subtopics, upload of a new object in storage, event logs, etc. These event streaming pipelines can be used in multiple ways without explicitly provisioning and de-provisioning infrastructure
- A simple example of **media processing** is the generation of a thumbnail using a serverless function when a new image is uploaded to a storage bucket in the cloud. An event is generated automatically with a new image upload that invokes the thumbnail generating logic provided by you.
- Serverless can be used to **automate the CI/CD pipeline** that gets triggered upon a code -check-in. The code check-in event can drive multiple function invocations in the pipeline such as - code security and other checks, build, test, and then deploy the code in production.

## Why should I use Serverless?

- Fast experimentation (Idea -> Market)
    - Serverless model as the highest level of abstraction allows you to quickly develop and deploy just your business logic for quick validation.
- Automatically scale from zero to peak demands
    - If successful you can scale up and down automatically driven by customer demand and not you.
- No idling of resources means you never overpay
    - Since you pay-by-value, you don't have to worry about overpaying.
# Containers

## What is a container?

- A way of packaging your application code and all its dependencies as a **single deployable unit.** It's called a container since you can ship it anywhere and run it either on-prem or cloud with just the underlying Operating system as a substrate.
- Containers are **lightweight abstractions** providing isolation from each other so multiple apps with their own set of dependencies on different libraries can run at the same time on the host hardware and operating system.

## Why should I use Containers?

- In the pre-container world, one of the struggles that the engineering and ops team had was making the development and production environment identical. Developers would build and test in the dev/test environment but things would fail in the production environment leading to a long cycle of troubleshooting. Containers eliminate that problem.
- Since containers can be deployed anywhere, with container orchestration technology such as Kubernetes, a container can be moved to any compute instance. This dynamic deployment flexibility helps maximize the utilization of compute instances.
- Containers by definition are portable so you can deploy them anywhere - on-prem or cloud. You can even move them across clouds making your investments more cloud-neutral.

## Use Cases

Container technology is rapidly getting adopted across multiple use cases.

- **Containerize current apps**: To drive agility, reduce deployment errors and maximize resource efficiency, companies are packaging their existing apps into containers and using an orchestrator like Kubernetes to deploy containers in on-prem as well as the cloud.
    
- **Microservices:** An application architecture concept where you have small pieces of functionality to provide a service that interacts with other services only through APIs. For instance, an e-commerce application can consist of several microservices such as
    
    - a shopping cart
    - search
    - order
    - payments
    - product recommendations Each microservice can be built using a different language or technology stack allowing the developers flexibility of what works the best for them. Containers provide an easy way to package and deploy microservices.
- Since containers are portable as we discussed, many companies use them for **Hybrid or Multi-cloud** scenarios. As your deployment choices evolve, you don't need to do much rework on your apps if they are already containerized.
    

### Combining serverless and containers

Some CSPs allow you to run your containers in a serverless environment, allowing you to take advantage of the potential capabilities of both at the same time

### Challenges

Managing thousands of containers for resource management, security and compliance, and cost allocation can be challenging.

Make sure you set up governance using CSP services or third party offerings

# Data Lake and Analytics

## What is a data lake?

If you are an on-prem enterprise, you probably have silos of data across your enterprise locked into different systems. A Data Lake is a unified repository of all of your structured and unstructured data.

As you can see in the image below, data pipelines "feed" the data lake from the bottom

- From all sources of data such as your **on-prem data** sources,
- **Real-time data** coming from devices, sensors, logs, etc to populate your data lake. CSPs provide a highly reliable and resilient storage infrastructure to build your data lake.

Services you can use based on that data

- You can build your **Machine Learning Models**
- Analytics can run on top of the data lake using services provided by the CSP.

![Data Lake](https://video.udacity-data.com/topher/2021/March/60512a91_datalake/datalake.png)

Data Lake

## Why should I build a Data Lake?

- Generate **new insights** for the business: Insights that were difficult to surface can now be surfaced with relative ease as you build analytics over your data lake that span across ALL of your data - structured as well as unstructured data.
- Build **machine learning models**: Having your data lake in the cloud streamlines your ML flows allowing you rapidly build, train and deploy ML models utilizing the data in the data lake.
- Build innovative **data-driven apps:** The creation of new innovative apps is a lot easier as your apps now have access to all the data with relative ease. Data Lake in a way democratizes the data empowering everyone in your organization to use data to make business decisions.

## Use Cases

- **Complex analytic queries**: If your data is spread across multiple silos it becomes super difficult to run queries against those multiple silos. Creating a data lake makes running complex business queries against structured and unstructured data easy and fast. As a result, _**your decision-making is faster and is data-driven.**_ Companies across all industries such as _Netflix, Equinix, Adobe, Pfizer, Moderna_ use cloud-based data lakes and analytics to discover business insights and deliver great customer experiences.
- **Real-time analytics**: Processing massive real-time data to gather insights and take action in near real-time isn't easy with conventional technologies. Cloud providers provide services that take away the heavy lifting associated with real-time data handling so you can focus on delivering great customer experiences. For instance, _Netflix_ analyzes data from all its viewers across the globe in real-time using cloud services, allowing it to discover issues and address them quickly delivering a great customer experience.
- **Operational analytics**: Whether you run an e-commerce site or other online operations, analyzing operational data through logs and clickstream is super important to discover operational issues and deliver a great customer experience. Companies such as _Intuit, Autodesk, CoinBase, Expedia_ all use cloud services for operational insights.

## On-prem vs. cloud solution

How much time, cost, and effort it is to expand your data lake with 4 nine availability, extremely high durability, security, compliance, and audit capabilities, and with multiple storage tiers to optimize cost?

Think about the services you need to build to ingest data, manipulate data, query data, and the operational cost and challenges? Does the heavy lifting add any value to your business? The cloud can help you build and secure your own data lake in days instead of months.

In the next section, we discuss Artificial Intelligence and Machine Learning services that nicely integrate with the data lake and related services to build, train and deploy your ML models to provide great customer experiences in a fraction of a time compared to doing it on-prem.

# A.I. & M.L.

There are two types of developers who will find value in using (A)rtificial (I)ntelligence and (M)achine (L)earning.

## Developer with A.I. and M.L. experience

- **If you are:** a developer with ML experience or you are a data scientist,
- **Who wants to**: build, train and deploy a model...
- **CSPs offer:** many ML services that are well integrated with ML infrastructure and frameworks such as Tensorflow, PyTorch, MxNet, etc. In addition, as we discussed earlier, data lake also becomes a big enabler within these cloud services providing seamless access to your data to build and train models.
- **Benefits**: Cloud not only removes complexity from your ML workflow but also allows you to speed up your model building, training, and deployment cycle. For instance, the availability of specialized processors called GPUs is important to accelerate the model training as well as inference time. CSPs are constantly adding the latest generation specialized processors allowing you to stay on the cutting edge.

---

## Developers with No A.I. and M.L. experience

- **If you are:** a developer an application developer with no machine learning background,
- **Who wants to:** infuse AI into your apps
- **CSPs offer**: ready-to-use AI services with pre-trained models offered through simple APIs you can use in your apps. The services span across areas such as Vision, Language, or Text. The services have been expanding to cover purpose-built AI solutions for industries. For instance, industrial companies who want to improve uptime for the plant, can deploy predictive maintenance solutions from the cloud provider in their plants and use the predictive maintenance AI services in their applications to predict failures.
- **Benefits**: You can significantly improve your operations or deliver new customer experiences avoiding the complexity of AI and ML workflows. The CSP takes care of the Machine Learning and data science behind the scenes to continuously improve the accuracy of AI services offered.

## Use Cases.

- **Predictive Analytics** is based on using historical data to predict the future. It's frequently used in customer lifecycle management to predict if a customer is likely to churn, or specific offerings that can drive growth via cross-selling. In the financial industry, it is used to assess the underwriting risk based on a prediction of bankruptcy or fraud, etc.
- **Predictive Maintainance**: Equipment failures can be catastrophic leading to production losses, unhappy customers, and other negative consequences for your business. Predictive maintenance allows you to predict if a piece of equipment is likely to fail so you can take appropriate action before it fails. It is used by many industrial and manufacturing companies.
- **Supply chain efficiency**: When inventories pile up lagging demand, companies suffer losses. Similarly, inventory shortages can lead to unhappy customers. Using AI in demand forecasting and dynamic network planning can lead to optimal supply chain and logistics for all companies.
- **Fraud Detection:** According to a recent survey from PwC, the fraud losses amounted to $42 billion in the US over the last 2 years. Companies can mitigate many fraud cases by deploying AI. Many financial companies use AI to detect credit card fraud, money laundering, and other financial crimes.
- **Customer Experiences**: Many customer experiences are being powered by AI across all industries. No need to tell who you are when you call customer care as AI can recognize your voice and bring up all your recent data. Product searches are no longer just typing a description of the product in a search bar, you can take a picture say on eBay and Amazon app, and the system will find similar things for you.

## A.I. and M.L. as electricity powering your organization

There is tremendous innovation happening in the AI/ML area across academia, industry, startups, government. Cloud providers are constantly adding new services bringing all the innovation in a form that's easy to consume by you. So, if YOU are not taking advantage of it, someone else in your industry is and they would likely leapfrog you. While you can do AI on-prem, moving your A.I. to the cloud is a smarter choice; it is easier to stay competitive given the cost and effort required to assemble the building blocks before you can deliver AI-driven experiences to your customers. CSPs take away a lot of heavy lifting behind AI and ML, allowing you to focus on your business innovation.

# IoT

## Internet of Things

#### What is IoT?

Internet of things refers to billions of devices and sensors connected over the internet, collecting and sharing data that's used to drive decisions or outcomes. If you have home automation with smart bulbs, smart switches, smart surveillance cameras, smart thermostats, and possibly something like Alexa or Google Home, you are getting the benefits of IoT already.

When you have billions of sensors and devices collecting data, you require very specialized infrastructure to not only control and manage these devices but also gather, store and analyze real-time data coming from these devices. Cloud provides you the services to do that efficiently.

### Why should we use IoT?

- **Deliver new customer experiences:** Many companies use IoT to deliver new customer experiences. For instance, iRobot, a robotics vacuum cleaner company uses IoT to deliver great customer experiences. Customers can use a mobile app or smart home device such as Alexa to manage the vacuum cleaner, find it if it gets stuck somewhere, schedule cleaning, etc.
- **Predictive Maintainance:** We discussed predictive maintenance earlier in the ML section. Otis, the leading elevator company, uses IoT on the cloud to do predictive maintenance of its 2 million elevators across the world. As a result, They are able to significantly reduce elevator downtime, delivering a better customer experience and reducing their own operational costs.
- **Operational Insights:** Many companies collect operational data from their equipment to see how customers use them so they can learn and make improvements in product designs. Data-driven decision-making in product design leads to optimal investments in product designs maximizing customer delights and reducing wasted spend on features sparingly used by customers.

### Use Cases

![I.O.T. Use Cases](https://video.udacity-data.com/topher/2021/March/60512af1_iot-use-cases/iot-use-cases.png)

I.O.T. Use Cases

- **Home Automation**
    - Home automation is one of the most common use cases for IoT. We earlier talked about iRobot, the robotic vacuum company. Rachio, a smart watering system company, provides a full IoT solution in the cloud that includes smart moisture sensors, controllers, weather forecasting system to design an automated and intelligent watering plan for your backyard.
- **Smart Factories**
    - We talked about Predictive Maintainance earlier. Predictive maintenance can reduce downtime leading to happier customers and reduced operating costs for you. The concept of Smart Factories goes much beyond predictive maintenance. It also means using IOT data to optimize factory functions for improving factory productivity. For instance, Volkswagen group, an automobile company, uses IoT on the cloud to improve the operations of all of its factories through data collected from sensors leading to a reduction of factory costs and a 30% increase in productivity.
- **Smart Cities**
    - Imagine a city where traffic signals are dynamically self-optimized depending on traffic conditions, authorities can respond to accidents and maintenance incidents faster. Many cities have active projects implementing these IoT-driven solutions on the cloud.
- **Health Monitoring**
    - Many healthcare device manufacturers are building IOT enabled devices for remote monitoring of patient health. This IoT solution delivers better patient care and timely response to health issues, connecting caregivers to patients in ways not possible before.
# Blockchain

## What is Blockchain

Blockchain conceptually is an **immutable distributed ledger** that allows multiple parties to engage in trusted transactions without having a central party acting as a trusted authority.

Cryptocurrencies such as Bitcoin use Blockchain as the underlying technology to conduct payment transactions without an intermediary such as a bank.

## Why should I use Blockchain?

- To build apps on blockchain, you need to build and secure a blockchain network requiring quite a bit of work. Maintaining and expanding the blockchain network as your blockchain ecosystem expands is also no-trivial.
- A Cloud provider helps eliminate the complexity associated with setting up and maintaining blockchain networks allowing you to build ledger applications.
- Think about what problems in your business you can potentially solve and experiment using blockchain on the cloud. For instance, if you have supply chain issues such as counterfeit goods, compliance violations, waste, or delays, you may want to think of solving them using blockchain. There are a variety of use cases in multiple industries where blockchain-based apps can shine.

## Use Cases

### Supply Chain

- **Transparency**: Every industry has a supply chain and therefore ensuring the authenticity of products and components as they move through the chain, avoiding wastes, and ensuring quality are all supply chain issues companies struggle with. Nestle, a European food company, well known for its coffee brands, was faced with similar supply chain issues. They also wanted to bring more transparency to the supply chain for its consumers to verify things such as the origin of coffee time of harvest, transaction certificate for the specific shipments, as well as the roasting period.
- **Trust**: Nestle turned to a Blockchain-based solution to provide the trust its buyers needed for the coffee and food items they consume. They used blockchain's transactional transparency and trust as an enabler for delivering an innovative experience for its buyers. By simply scanning a QR code, buyers can access the supply chain history of the food or coffee they just bought.

### Example : (D)igital (R)ights (M)management

![The Complexity of DRM](https://video.udacity-data.com/topher/2021/March/60512bc6_ccbl-c1-drm-problem/ccbl-c1-drm-problem.png)

The Complexity of DRM

Sony Music uses a digital rights management system. DRM and copyright verification are critical to ensuring artists are compensated for their work.

## The problem

You can this demonstrated in the image above -- the old method of contracts across multiple parties involved in the production and distribution of music to ensure digital rights is ripe with problems and leads to high costs for the creator of the music.

Follow along in the image above: Here is what this system looks like

- Copyright ownership begins with the creator at the genesis of the content.
- From there, it can then be sold or transferred to other parties.
- The system of record must be able to verify the copyright owner and enable compensation for use of the material under the laws of the relevant jurisdiction.

## How does a Blockchain-based DRM platform work?

![Blockchain Solution](https://video.udacity-data.com/topher/2021/March/60512be2_ccbl-c1-drm-solution/ccbl-c1-drm-solution.png)

Blockchain Solution

The image above conveys the solution to this complex system in a _Blockchain-based DRM platform_. How does this work?

- Composers copyright is recorded in the BC system
- When the individual acquires rights to the content, the provider’s system adds a new block in the network representing those rights.
- The provider can then send the encrypted music data, which can be decoded after verification against the user’s rights blockchain.
- This streamlines the DRM process allowing artists to focus on the production of music knowing the system will protect their rights and compensate them for their work adequately.

## Future of Blockchain

Blockchain is a relatively new technology and use cases are still emerging. There are companies building identity verification solutions on blockchain. Financial services companies are looking at simplifying trading and creating innovative payment solutions. Smart contracts that don't require any intermediary and distributed ledger have great potential to transform all industries and the public sector as well. McKinsey, a leading management consultancy firm has ranked public sector, technology, media, telecom, and financial services industries where the ease of adoption and potential impact is going to be relatively high compared to others.


# Edge Computing

![Edge Computing](https://video.udacity-data.com/topher/2021/July/60dde689_ccbl2/ccbl2.png)

Edge Computing

In the image above, you can see that Edge computing is a distributed computing paradigm that brings computation and data closer to the location where it is needed to improve response time and save bandwidth.

- **Cloud Layer**
    - A typical architectural pattern is for AI models to get trained in the cloud, and get deployed on the edge for inferencing.
- **Edge Layer**
    - There are other use cases for edge computing such as management of IoT devices, storage and caching of data, and doing certain compute offload functions such as resizing images based on the requesting device type.
- **Device Layer**
    - Actual end devices such as cars, drones, and surveillance cameras can send real-time data such as video feeds for inference on the edge for quick response time.

## Why should I use Edge Computing?

- Managed service eliminates the complexity of edge deployments
    - The cloud players are realizing the significance of edge computing and are extending their cloud model to "cloud and the edge" by providing cloud-based programming models, APIs, etc to developers to give them the flexibility to deploy the apps in the cloud or the edge.
    - Cloud providers have recently announced new services for edge computing such as AWS Wavelength or Azure Edge Zones and are forging partnerships with telecom operators to provide end-to-end edge computing solutions. Building this edge computing model with right-edge locations, network access, application ecosystem would be very difficult otherwise.
- Innovative apps to deliver new customer experiences or improve operations.
    - Edge computing unlocks new innovation opportunities. A smart factory where real-time decisions need to be made can't afford the latencies of the cloud.. edge computing lights up those scenarios, improving your operations. Gaming where latencies matter a lot to deliver interactive real-time experiences to gamers is another example. An entirely new set of experiences with augmented and virtual reality are now possible in any location such as a department store.

![Edge Computing use cases](https://video.udacity-data.com/topher/2021/March/6051338e_edsge-use-case/edsge-use-case.png)

Edge Computing use cases

## Use Cases

While edge computing combined with 5G as the new radio access technology is relatively new, it's already showing the potential for solving problems and enabling new experiences in almost all industries.

### Healthcare

Let's take Healthcare as an example. A startup in the USA has built an edge solution that would allow doctors to do a colonoscopy and detect hard-to-find polyps using AI. The way the solution works is as follows - video feed from the endoscope is sent over 5G network to a closeby edge computing location where an AI model runs to identify polyps. The results are sent back in near real-time allowing the doctor to finish the colonoscopy and deliver better results improving patient care.

### Smart factories

We touched upon Volkwagen when we discussed IoT. Volkswagen is also using edge computing to improve factory operations. The devices in the factory send data to edge equipment running AI inferencing models to assist with real-time decision-making. Imagine the power of this architecture. You can automate so many processes. You can send video feeds to check for anomalies and do quality checks in the assembly line with AI.

## Edge Computing: The new frontier for innovation

Edge computing use cases are in all industries. Companies in all industries such as Agriculture, Healthcare, Retail, Finance, Public Sector, Industrial are all looking at use cases enabled by 5G rollout, Multi-access edge computing, and advances in AI/ML. Cloud simplifies the complexity of building and deploying edge applications by bringing all these elements together in partnership with leading telecom companies such as AT&T, SK Telecom, Verizon, KDDI, etc.

Edge is rapidly becoming the new frontier for innovation. New business models are emerging. I encourage you to think about use cases relevant to your industry and try them out with your cloud provider.

`The cost of experimentation in the cloud is very low and the payoff could be very high.`

# Exercise Cloud Innovation Services

## Cloud innovation services

Pick any 3 of the recent cloud innovation services (Serverless computing, Containers, IoT, Data Analytics, AI and ML, Blockchain as a service, Edge computing). Describe how you’d use each of the three to innovate in your business. Also list the business benefits of each (e.g. new revenue stream, improved customer experience, higher operational efficiency, etc)

Please continue to use the template `Exercise Template.docx` or `Exercise Template.txt` to record your responses. This is located under the Resources section of the course, in the top left of this page.

## Solution

Serverless computing: I’d encourage my staff to conduct experiments and create new apps using Serverless technologies. Serverless dramatically improves TTM as there is nothing else to build or manage other than application logic. I can do more experiments with fewer people. Serverless would improve our operational efficiency.

AI as a service: My company is in the eCommerce space. A new feature we added recently is called “Image Search” which allows customers to upload an image of an object they like (dress, shoes, pots, etc), and our site provides a list of matching items in our inventory. This feature was built using machine learning (Computer vision) technologies.

I would use the Cloud provider’s machine learning stack (specialized hardware for training the models as well as inference, ML software, and the entire data science automation from development to production) would accelerate the feature release lifecycle. I can scale up and down quickly on the cloud with my model complexity and improve object match accuracy. In addition, I can deploy it in local geographies improving the response time and customer experience. The major business benefit is customer experience.

Edge Computing: With edge computing, we can deliver new shopping experiences in our retail stores. Customers can virtually try before they buy using Augmented reality (AR) technologies, Edge computing locations allow us to build AR applications and deploy them on multiple Edge locations provided by the cloud provider. We can significantly enhance our customer experiences with Edge Computing.

# Best Practice and Expert Intuition

## Best Practices and Expert Intuition

`Cloud is not just a technology... it's a way of running your business.`

Innovating in your business is key to staying relevant in this fast-paced world. Here are a few considerations to keep in mind as you think about innovating with the cloud.

### Complexity

While cloud providers do an excellent job of doing the heavy lifting behind the scenes for all innovation, you still need to understand the risks and complexities of the adoption of these innovative services. Each innovation will deliver tremendous value when architected right, and supported by good governance. Security, compliance, and cost management issues apply to the solutions you build utilizing these services. For instance, while containers are great, they expose new attack surfaces which fall into the shared responsibility model. You need to understand your part and ensure you take care of container security starting from your CI/CD pipeline before the containers get deployed in production.

### Risk and Rewards

Cloud significantly changes the risk/reward ratio. The cost of experimentation in the cloud is much lower than in on-prem. And if the experiment succeeds, the payoff is likely bigger as you can quickly scale and ramp up capacity. This should tie back to the culture in your organization which should evolve with this new paradigm, and encourages more risk-taking.

### Sandboxes

Innovation can't be forced or run as a program. Ideas can come from anywhere if you remove barriers, and give everyone a chance to build something. Providing sandboxes and letting people set aside some time for skunkwork projects, can be worth the effort.

### Democratize data

Innovation can suffer if people can't access company data. Creating a data lake and providing secure and controlled mechanisms for people to access data would remove a key barrier to innovation.

### Constant change

You are never done in the cloud. You need to keep re-architecting your existing services as new cloud services show up. For instance, AWS pioneered the cloud computing model with just one service S3 in 2006 and now has 200+ services, and are constantly adding more services and features to existing services. Other cloud providers are also doing the same. Keeping up with the pace of innovation in the cloud world requires a cultural and mindset change.

# Exercise Identifying Current Innovations

## Current Innovations

Identify one product, service, or application from your company that you consider innovative. Describe it in a few sentences and highlight what aspect of it do you consider to be innovative. If you were to rebuild it utilizing cloud capabilities, what specific cloud innovative capabilities would you leverage? What’s the business benefit of building it on the cloud (faster build, global scale, etc) compared to the traditional model?

Please continue to use the template `Exercise Template.docx` or `Exercise Template.txt` to record your responses. This is located under the Resources section of the course, in the top left of this page.

## Sample Solution 1

My company is in the eCommerce space. A new feature we added recently is called “Image Search” which allows customers to upload an image of an object they like (dress, shoes, pots, etc), and our site provides a list of matching items in our inventory. This feature was built using machine learning (Computer vision) technologies.

I would use the Cloud provider’s machine learning stack (specialized hardware for training the models as well as inference, ML software, and the entire data science automation from development to production) would accelerate the feature release lifecycle. I can scale up and down quickly on the cloud with my model complexity and improve object match accuracy. In addition, I can deploy it in local geographies improving the response time and customer experience.

# Lesson Review

## Lesson review

Looking back at what we studied:

- We looked at some business trends and saw how the increased pace of innovation is driving disruption in all industries.
- We discussed how some of the characteristics of the cloud are well suited for innovation
- We looked at some of the major cloud services that are being utilized to drive innovation. We also covered some typical use cases across all industry segments that are apt for these cloud services
- We shared some best practices to drive innovation in your organization.

## Case Study

While we are done with the final lesson on innovation, we are not done learning. We are going to introduce you to Capital One and look back at the journey they took as they transformed their business model into the cloud.

# Business Case Study

## Business Use Case

video below will have bullet points added at 3:20 , 3:40

## Capital One

This case study brings everything together we have learned in the course.

This is the story of Capital One, one of the leading financial services companies in the US, ranked 97 in Fortune 500 companies. The reason I picked this story is for _two reasons:_

- It exemplifies all major areas we covered in the course from building the business case to organizational capability building to setting up governance and delivering innovative services.
- It's a financial services company that is highly regulated in the US.

Regardless of the industry, you are in, I hope the story inspires you to not be intimidated by the complexity of your business situation, operating rules, and industry regulations and _instead_ make a bold move to the cloud.

---

### Building the business case for cloud

#### The role of technology

They believed in technology as a core and not a support function for the business. This meant beefing up the technology capabilities so they can be a technology company first before being a bank.

CapitalOne is mostly a digital bank with very few branches in select locations in the US. They have grown software engineering organizations to 11,000 engineers and wanted to focus on customer experiences and not running infrastructure and operations.

#### New customer experiences

CapitalOne built the business case on speed and delivering new customer experiences. in 2015, it announced that all new company applications would run in, and all existing applications would be systematically rearchitected for—the cloud. They set a goal to retire all of their 8 datacenters to be all-in on the cloud by 2020.

`They have accomplished their goal.`

#### TCO

As we covered in the course, the business case for the cloud shouldn't just be built on just the financial aspects of TCO. In the Capital One case, While the business case factored in cost savings from data centers, but the **business agility** and desire to deliver new experiences is what drove the public cloud decision.

### Leadership

In this course, we talked about how important it is to have a strong C-level exec sponsor who needs to be personally vested in the cloud-led transformation. In the Capital One case, George Brady, EVP, and CTO of Capital One was the exec sponsor. He enlisted support from other leaders by championing the value of the cloud:

- Supports faster innovation
- Support saving and finding value in more data
- Supports faster recovery from failures
- Supports shifting resources from operations to higher-value work.

Once other leaders were enlisted, things became easier as everyone was working towards a common mission to turn Capital One first into a tech company as well as a bank.

### Cultural transformation

In this course, we discussed the importance of cultural transformation and mindset changes needed to operate well in the cloud. A big part of the cultural transformation we advocated was

- DevOps
- DevSecOps

In the CapitalOne case, incorporating customer feedback into new experiences used to take a long time in the earlier more traditional waterfall method at CapitalOne. The developer engagement ended after handing it off to operations. The product managers weren't as engaged in the development cycle. CapitalOne rebooted the developer culture to adopt a DevOps mindset.

### Moving to a DevOps mindset

They saw the immediate benefits of how quickly they can turn customer feedback into features. Developers developed a more sense of ownership for uptime and monitoring of the services in production. Product managers are now more engaged and collaborative with DevOps teams to turn customer feedback into features quickly. This culture also was instrumental in attracting new talent to CapitalOne.

### A culture of learning

Transitioning People to new roles and skills enablement was another pillar we covered in the course. And this education should not be limited to technical roles but business roles as well.

In the CapitalOne case, targeted training and education for technical professionals, as well as business executives, was launched. A _culture of learning_ where employees invested working hours in getting cloud certifications was instituted. In addition, targeted workshops and other learning events were launched throughout the company.

_Clearly, all of this wouldn't have been possible without strong executive sponsorship, as we discussed in the course._

### Putting governance in place

In this course, we discussed the importance of governance. In CapitalOne's case, they didn't move a single workload until their governance model was in place.

A risk-averse attitude would be to first run non-core systems in the cloud leaving critical data and apps on-prem. Instead, CapitalOne tackled upfront the hard problems of:

- Security
- Compliance

### Team collaborations

As we had discussed earlier in this course, the people and process aspects are very important for governance. CapitalOne tasked risk managers and cloud engineers to collaborate in building controls and processes so the developer teams can build new experiences with appropriate security and compliance guardrails.

### "Cloud Custodian"

They also developed and open-sourced a compliance enforcement framework called "Cloud Custodian". Prior to Cloud Custodian, different teams were building scripts and custom code to establish compliance which was cumbersome. Cloud Custodian simplified and standardized compliance framework across CapitalOne.

### Innovation

As we discussed in the course, the key motivation to move to the cloud should be to innovate faster leveraging cloud services. Capital One has been doing that effectively now that they are _all-in_ with the cloud.

#### New customer experiences

With all of its data on the cloud, CapitalOne has built several new customer experiences using **data analytics** and **machine learning** services of the cloud provider. For example, they built "Eno" a digital assistant to track spending, provide fraud alerts, save you money, and answer any questions. Eno is built on **serverless technologies** from its cloud provider along with several **machine learning** and **A.I.** capabilities.

### The journey continues

CapitalOne cloud journey continues but surely they, _and their customers,_ are happy with the move as they are now able to innovate much faster on the cloud.

# Exercise Case Studies

## Case Studies

Pick any case study (preferably related to your own industry) published by cloud vendors via the links below.

- [AWS(opens in a new tab)](https://aws.amazon.com/solutions/case-studies/?customer-references-cards.sort-by=item.additionalFields.publishedDate&customer-references-cards.sort-order=desc)
- [IBM(opens in a new tab)](https://www.ibm.com/cloud/case-studies/)
- [Azure(opens in a new tab)](https://azure.microsoft.com/en-us/case-studies/)
- [Google(opens in a new tab)](https://cloud.google.com/customers)
- [CloudPro(opens in a new tab)](https://www.cloudpro.co.uk/case-studies)
- Identify the key pain point(s) or business innovation(s) realized with the cloud.
- In contrast, list the set of steps that would need to be taken to solve the same problem _without_ the cloud.

Please continue to use the template `Exercise Template.docx` or `Exercise Template.txt` to record your responses. This is located under the Resources section of the course, in the top left of this page.

## Sample Solution

In this sample response, I picked: [(opens in a new tab)](https://aws.amazon.com/solutions/case-studies/arneg/?did=cr_card&trk=cr_card)[https://aws.amazon.com/solutions/case-studies/arneg/?did=cr_card&trk=cr_card(opens in a new tab)](https://aws.amazon.com/solutions/case-studies/arneg/?did=cr_card&trk=cr_card)

**Key pain point:** On-prem alerting systems would send alarms only when refrigeration was malfunctioning. This put pressure on Arneg to respond quickly and resulted in customer downtime. Arneg wanted to predict failures with a high degree of accuracy to improve customer experience and overall operational efficiency. They were able to innovate with architecture on the cloud that addressed this pain point.

List of steps if the same thing were to be solved using on-prem(ise) solution:

- Hire a team of data scientists and ML experts.
- Buy specialized hardware (GPUs) and other infrastructure to build the predictive maintenance model.
- Buy massive storage to collect and store data from IoT records.
- Build a toolchain for data science and a process for the iterative process of training the model and dropping it into production.
- Deploy production infrastructure in all the sites/geographies where it had a presence.
- Make everything redundant and highly available.

# Course Review

### Congratulations!

We have covered a lot of information, let's review that to give some perspective

- In the first lesson, we looked at the business side of how the cloud can impact your organization.
    - Cloud fundamentals
    - Business case
    - ROI beyond TCO
    - Migration strategies
- Then we focused on the people and skills, two of your most powerful assets, and how they can be expanded to the extent of your capabilities
    - Why capability building is needed
    - Target state model
    - People, Process, Culture
    - CCoE
    - DevOps, DevSecOps, FinOps
- In the next lesson, we focused on how governance plays a part
    - Cost
    - Security
    - Governance at enterprise scale
- In the last lesson, we looked at several leading-edge innovations and how these might be a powerful part of your strategy
    - Why cloud for business innovation
    - Cloud Services for innovation
- Finally, We took a look at a real case study with Capital One, and how they made a transformation to the cloud. We connected their journey with the same concepts you learned in this course.

_Now, it is on to your next challenge with the Final Project._ The learning and exercises throughout the lessons were specifically targeted to help build the skills needed for you to do this effectively.

Enjoy! See you in the cloud!

# Glossary

|KeyTerm|Definition|
|---|---|
|Blockchain|A computing model for recording immutable transactions, and supporting a distributed ledger.|
|Containers|A compute abstraction within an operating system allowing you to isolate workloads within the same compute instance.|
|Data Lake|A consolidation of all of your data into a single repository.|
|Edge computing|A computing model that runs compute closer to where it is needed.|
|Internet of Things(IoT)|A model where sensors, devices and other things are connected to the internet.|
|Predictive Analytics|Based on using historical data to predict the future.|
|Predictive Maintenance|Equipment failures can be catastrophic leading to production losses, unhappy customers, and other negative consequences for your business.|
|Sandboxes|Isolated cloud accounts for training, learning, and trying out things.|
|Serverless computing|A computing model where you pay only when your code runs.|
# Further Reading and Learning

**Serverless**

[How “Financial Engines” cut costs by 90% using Serverless architecture(opens in a new tab)](https://aws.amazon.com/solutions/case-studies/financial-engines/)

**Containers**

[How MakeMytrip cut compute costs by 22% with Containers(opens in a new tab)](https://aws.amazon.com/solutions/case-studies/makemytrip/?did=cr_card&trk=cr_card)

**AI & ML**

[Hi Translate: Breaking down language barriers with real-time translation tools(opens in a new tab)](https://cloud.google.com/customers/hi-translate/)

**IoT**

[AkzoNobel: Improving factory performance with Industrial Internet of Things (IIoT) technology(opens in a new tab)](https://customers.microsoft.com/en-us/story/782142-akzonobel-manufacturing-azure-iot-netherlands-en)

**Blockchain**

[GE Aviation’s Digital Group streamlines tracking of aircraft parts, reduces inefficiencies with Azure Blockchain technologies(opens in a new tab)](https://customers.microsoft.com/en-us/story/755328-ge-aviation-manufacturing-azure)

**Edge Computing**

[**Chaotic Intersection of 5G, Edge Computing and Cloud**(opens in a new tab)](https://troposcale.com/chaotic-intersection-of-5g-edge-and-cloud/)

- [AWS Wavelength(opens in a new tab)](https://aws.amazon.com/wavelength/)
- [Azure Edge Zones(opens in a new tab)](https://azure.microsoft.com/en-us/solutions/low-latency-edge-computing/)
- [Google Anthos for the Edge](https://cloud.google.com/solutions/anthos-edge)

