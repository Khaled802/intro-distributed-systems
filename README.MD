# Introduction to distributed systems

## definition
   - It is a collection of autonomous computer systems that are physically separated but are connected by a centralized computer network that is equipped with distributed system software.
   - Autonomous: operates independently 
   - For the user, the nodes of the systems works as a one unit (Transparent)


## Goals
   - To share hardware, software, or data between nodes
   - Easy scale-out
   - Fault-tolerance: there is a failure in the software or hardware happens and the system continues to operate
   - It can be extended to more location

## Cons
   - Security problems: because of shared data between the nodes
   - Network problems: 
     - taking more time to access data than any storage
     - may not reach for the data 
   - It is a more complex system than a monolithic
   - data consistency

<br>

## components of distributed systems

### Storage
   1. databases
   2. file systems

#### Databases
   - Relation Database
     - It has tables(relations) and these tables has relationsships with each other
     - It has strict schema

   - Nosql databases
     - Not only sql
     - EX: Document store, Graph databases, etc...
  - Cache
    - Ex of usage: A thing needs high computing power and is repeated with the same result, you can put it in the cache to get it and put the expiration date for it

#### file storage
   - to store large files that are hard for the normal database to get the file because of their size
     - The file page is small size so you cannot use index to get the file in a fast way

   - So you can use systems like S3, Hadoop, Azure storage, etc ...

### Computation nodes
   - responsible for main processing units

### Analytics
   - Get different information like
     - Where do the users live?
     - What are the most visited pages?
   - Ex: Google Analytics

### load balancer
   - Redirect the requests to the nodes
   - There is different type of load balancers

### Queue
   - Make async operations between different nodes

### streams
   - like queues
   - but without popping the information
   - More than one node can take this information
   - Tools: Kafka, Spark, etc...

<br>

## Scaling

### computational scaling
   - Scale up
     - change the hardware with hardware with more power like:
       - Memory 64Gbyte -> 256Gbyte
       - CPU with 4 cores -> 8 cores
     - Easy to use there is no change in the software
     - Limited
     - Expensive
  - Scale-out
    - Add nodes
  
### Database Scaling

#### Database Mirroring
   - You make copies of the database (read-only) to reduce the load on one database

#### Database Sharding
   - Divide one database, if one database can't have all data in one database
   - divide them into specific characteristic

## Models
   - Architectural model
     - components
   - Fundamental model
     - characteristics

### Architectural model
   - Client/Server
   - Pear to Pear (P2P)

### Fundamental
   - performance communications
     - latency
     - bandwidth
     - jitten
   - interaction model
     - synchronous
       - process is existing in known range of time
       - message is received in known bound of time
     - asynchronous
  

