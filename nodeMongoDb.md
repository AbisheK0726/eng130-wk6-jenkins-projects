# Node.js and MongoDB

## Node.js

### What is Node.js?

Node.js is an open source, cross-platform runtime environment built on Chrome's JavaScript engine for easily building fast, scalable network applications.

Node.js uses an event-driven, non-blocking I/O model that makes it lightweight and efficient, perfect for data-intensive real-time applications and for for developing server-side and networking applications that run across distributed devices.

### Features of Node.js

* Node.js is Asynchronous and Event Driven

All the APIs of Node.js library are asynchronous, that is, non-blocking. This mean that Node based server do not wait for the API to return the data. Instead it will keep executing the next API after calling it and a notification mechanism of Event Driven Callbacks is used to get the response of the previous API call.

* Node.js is Single Threaded but Highly Scalable

Node.js uses a single threaded model with event looping. Event mechanism helps the server to respond in a non-blocking way and makes the server highly scalable as opposed to traditional servers which create limited threads to handle requests.

Node.js uses a single threaded program and the same program can provide service to a much larger number of requests than traditional servers like Apache HTTP Server.

### Use cases of Node.js within Jenkins

* Provides NodeJS auto-installer, allowing to create as many NodeJS installations "profiles" as you want. The auto-installer will automatically install a given version of NodeJS, on every jenkins agent where it will be needed

* Allows to install globally some npm packages inside each installations, these npm packages will be made available to the PATH of the jenkins agent

* Allows use custom NPM user configuration file defined with config-file-provider plugin to setup custom NPM settings

* Relocate npm cache folder using pre defined strategies, this is useful when you have a shared workspace and you want to avoid npm cache conflicts

## MongoDB

### What is MongoDB?

MongoDB is a document-oriented NoSQL database used for high volume data storage. Instead of using tables and rows as in the traditional relational databases, MongoDB makes use of collections and documents.

Documents consist of key-value pairs which are the basic unit of data in MongoDB. Collections contain sets of documents

### Features and Benefits of MongoDB

* Document-oriented – Since MongoDB is a NoSQL type database, instead of having data in a relational type format with a predefined schema, it stores the data in documents. This makes MongoDB very flexible and adaptable to real business world situation and requirements.

* MongoDB does not have a defined schema. This means that you can store different types of data in the same collection. This is a huge advantage over relational databases where you have to define a schema for each table.

* Scalability – The MongoDB environments are very scalable. Companies across the world have defined clusters with some of them running 100+ nodes with around millions of documents within the database.

* Load balancing – MongoDB uses the concept of sharding to scale horizontally by splitting data across multiple MongoDB instances. MongoDB can run over multiple servers, balancing the load and/or duplicating data to keep the system up and running in case of hardware failure.

