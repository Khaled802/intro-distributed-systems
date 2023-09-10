# message queue and message broker

## message queue vs message broker
   - message queue: it is a data-structure used to queue the requests
   - message broker: it is component uses message queue with additional feature like routing, filtering messages, and different communication patterns like "pub/sub"


## Kafka
   - Is kafka a message message queue?
     - it is used as a message queue but it has some features different like
       - doesn't remove the message after consumed
       - message stay for period of time
       - multiple consumer for the same message

## pub/sub pattern 
   - it is communication pattern 
   - it makes async communication between nodes
   - it used to loose coupling between nodes

## why message broker
   - it make async communication between nodes
   - makes system more scalable and reliable
   - increases the security
     - encryption
     - auth
     - routing

## applications
   - notifications & feedbacks
   - prevent duplications
   - load palancing
   
