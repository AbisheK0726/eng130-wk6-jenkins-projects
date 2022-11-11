Hello everyone, my name is Mohamed Yusuf and this the Project Presentation for Group 2. 

[NEXT SLIDE] 

In this presentation we will going over CI/CD, Jenkins, Nodejs, MongoDB, and the security group rules for Jenkins. 

After, we will also do a demo which will show how we built our own Jenkins server to build a CI/CD pipeline with the required dependencies and plugins. 

[NEXT SLIDE] 

So what is CI/CD? 

CI/CD is an essential part of DevOps and any modern software development practice. 

It is a way to automate your software development workflows and deploy better quality code, more often.  

Using a continuous and iterative process to build, test, and deploy helps avoid bugs and code failures. 

The "CI" in CI/CD refers to continuous integration, which is an automation process for developers.  

Successful CI means new code changes to an app are regularly built, tested, and merged to a shared repository. 

By merging changes frequently and triggering automatic testing, you minimize the possibility of code conflict, even with multiple developers working on the same application 

 The "CD" in CI/CD refers to continuous delivery and/or continuous deployment, which are related concepts that sometimes get used interchangeably.  

Continous delivery automatically releases your change in code to repository, for example to your GitHub repo if your using Github. 

Continous deployment automatically deploys your code into production. 

The difference between the two is that for continous delivery, you have to manually aprove to update to production. 

Both are about automating further stages of the pipeline. 

[NEXT SLIDE] 

There are many benefits of using CI/CD but here are a few of them. 

It leads to happier users and customers: Fewer bugs and errors make it into production, so your users and customers have a better experience. 

When you can deploy anytime, you can bring products and new features to market faster.  

Your development costs are lower, and you will have a faster turnaround 

Free up developers’ time: With more of the deployment process automated, the team has time for more rewarding projects 

So What are the best practices? 

You want to have frequent check-ins to main branch, Integrating code in your main branch early and often. 

Use small segments of code and merge them into the branch as frequently as possible. 

Another thing you want to do is make it a team effort. Having more eyes on a piece of code will only benefit you, communicate with members of your team frequently to make the proccess as efficient as possible. 

 I would now like to pass it on to Abishek Jha. 

  

[NEXT SLIDE]
Page Break
ABHISHEK JHA 

Jenkins – It is an open-source automation tool built in Java, which makes it highly portable. It has plugins built for Continuous Integration Purpose. It is the most popular automation server used to implement CI/CD workflows. These workflows are also referred to as pipelines.  

Jenkins started out as a tool for continuous Integration only but over time, continuous delivery and deployment features have been added to Jenkins. 

We can see how the use of Jenkins is so useful, when we are deploying a microservice architecture. In microservice architectures we frequently update applications and services, and multiple changes should be implemented quickly. These can consume a lot of bandwidth. These small and frequent updates in quick intervals can only be achieved by the type of automation Jenkins provides. 

 

[NEXT SLIDE] The stages of Jenkins: 

A stage or a block defines a conceptually distinct subset of tasks performed through the entire pipeline e.g. “Build”, “Test” and “Deploy”. Jenkins uses many different plugins to visualize its pipeline’s status/progress.  

A pipeline can be defined as a collection of events or jobs which are interlinked with one another in a sequence. These blocks are combination of plugins that support the integration and implementation of continuous delivery pipelines using Jenkins. 

In the pipeline, every change made in the software goes through several complex processes on its manner to being released. It also involves developing the software in a repeatable and reliable manner, and progression of the built software through multiple stages of testing and deployment. 

 

[Next Slide] Job & Agent –  

Each stage in Jenkins can be defined as a job. We define explicitly all the tasks we need to achieve, and the plugins we use, inside the job. It is also referred to as Projects 

An agent enables the users to execute multiple jobs within the same Jenkins instance by distributing the load. It is typically a machine, or container, which connects to a Jenkins controller and executes tasks when directed by the controller. 

We can either use a single agent for the entire pipeline or use a distinct agent for the different stages of the pipeline. 

 

[Next Slide] 

Page Break
 

Angel: 
  
Hello, I am Angel and I will be talking about who uses Jenkins and what the benefits of Jenkins are specifically 

Who uses Jenkins? 

There are many companies using Jenkins now, in fact, more than 3000 companies use it. 

Some examples of use cases can be seen on the screen right now: Netflix, Facebook, Twitch, LinkedIn, Udemy and many more. 

How and why the companies use it I will explain by giving Netflix as an example 

When Netflix started using Jenkins, they only had one massive master node hosted in their datacentre, but now has 25 Jenkin masters hosted in AWS. Netflix has very extensive testing for deployment of code to end users. They use Nebula which is a collection of Gradle plugins to implement the same code over and over with very little interaction from programmers. Jenkins takes it further and automates this implementation. Along with the autonomous implementation, Nebula has a series of tests which test the programmers’ code automatically and push any features which pass the tests to production environment. This automation is also done by Jenkins.  

  

NEXT SLIDE 

  

So, what are the benefits of using Jenkins? 

Jenkins, as you heard just now, has many benefits, one of which is the ability to automate the majority, if not the entire CICD pipeline, test it and deliver or deploy it to customers. 

But how does a company benefit from using Jenkins? 

Jenkins is open source, meaning anyone can use it. It is in fact the go-to CICD tool for a lot of early stage companies as well as already developed companies 

It has a huge number of plugins, more than 1500 already available and tested  

It already has documentation on how to integrate it with different cloud providers such as Amazon EC2, Google Cloud, Digital Ocean and more. 

As Jenkins is Java based, it is cross platform (as every device nowadays has Java built in) 

The most attractive benefit to companies would be the cost and time savings. Automating everything apart from developing new features saves a huge amount of time and in turn, money. By having the deployment process taken care of, programmers can focus on creating new features instead of how to combine everything or deploy it for others to see. 

I will now pass it over to Abishek 

Page Break
 

 

 

[NEXT SLIDE] 

ABISHEK ANEESE 

Node 

What is Node.js? 

Node.js is an open source, cross-platform runtime environment built on Chrome's JavaScript engine for easily building fast, scalable network applications. 

Node.js uses an event-driven, non-blocking I/O model that makes it lightweight and efficient, perfect for data-intensive real-time applications and for for developing server-side and networking applications that run across distributed devices. 

  

Features of Node.js 

Node.js is Asynchronous and Event Driven 

All the APIs of Node.js library are asynchronous, that is, non-blocking. This mean that Node based server do not wait for the API to return the data. Instead it will keep executing the next API after calling it and a notification mechanism of Event Driven Callbacks is used to get the response of the previous API call. 

  

Node.js is Single Threaded but Highly Scalable 

Node.js uses a single threaded model with event looping. Event mechanism helps the server to respond in a non-blocking way and makes the server highly scalable as opposed to traditional servers which create limited threads to handle requests. 

  

Node.js uses a single threaded program and the same program can provide service to a much larger number of requests than traditional servers like Apache HTTP Server. 

  

Use cases of Node.js within Jenkins 

Provides NodeJS auto-installer, allowing to create as many NodeJS installations "profiles" as you want. The auto-installer will automatically install a given version of NodeJS, on every jenkins agent where it will be needed 

  

Allows to install globally some npm packages inside each installations, these npm packages will be made available to the PATH of the jenkins agent 

  

Allows use custom NPM user configuration file defined with config-file-provider plugin to setup custom NPM settings 

  

Relocate npm cache folder using pre defined strategies, this is useful when you have a shared workspace and you want to avoid npm cache conflicts 

 

MongoDB 

What is MongoDB? 

MongoDB is a document-oriented NoSQL database used for high volume data storage. Instead of using tables and rows as in the traditional relational databases, MongoDB makes use of collections and documents. 

Documents consist of key-value pairs which are the basic unit of data in MongoDB. Collections contain sets of documents 

  

Features and Benefits of MongoDB 

Document-oriented – Since MongoDB is a NoSQL type database, instead of having data in a relational type format with a predefined schema, it stores the data in documents. This makes MongoDB very flexible and adaptable to real business world situation and requirements. 

  

MongoDB does not have a defined schema. This means that you can store different types of data in the same collection. This is a huge advantage over relational databases where you have to define a schema for each table. 

  

Scalability – The MongoDB environments are very scalable. Companies across the world have defined clusters with some of them running 100+ nodes with around millions of documents within the database. 

  

Load balancing – MongoDB uses the concept of sharding to scale horizontally by splitting data across multiple MongoDB instances. MongoDB can run over multiple servers, balancing the load and/or duplicating data to keep the system up and running in case of hardware failure. 

 

[NEXT PAGE] 

 

What is a webhook  

It is essentially the communication between two API’s. So what you will need to do is provide the URI to the service providing the webhook and then that service will provide a HTTP request to that URI whenever an event occurs. In our case, we used GitHub to have a webhook trigger with Jenkins. So whenever we push code or anything to our github the webhook is triggered by this and then it will carry out the job of updating the repository.   

 

 