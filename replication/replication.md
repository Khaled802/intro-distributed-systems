# Replication
  It is storing the data in more than place or node

## WHY?
   - to keep reliability (fault tolerance)
   - to comeover network latency
   - to make scalable system

## Sync vs Async
   - Sync: the data written in both primary and replicas at the same time (replica is always consistant) but it add more complexity
   - Async: the data copied from primary to replica (it is simple) but may cause inconsistancy or loss



## Master-slave
   - Master is responsible for writing operations 
   - slaves can be used as a read only or replace the Master when master failure 
     - can use voting algorithems to choose the best slave to be the master
   - you can use p2p style to this
     - it cause some problems
       - if the connection faiture happend that cause inconsistancy 


## Distributed Consensus
   - to make multible nodes agree on a particular value
   - examples
     - two phase commit
     - MVCC (multi-version concurrency control)
       - used by Postgres
     - SAGA
     
  
