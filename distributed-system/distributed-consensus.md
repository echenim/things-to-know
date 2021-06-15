## Consensus " Agreement"
### Why Distributed Consensus " Agreement"?
Fundamental problem in distributed computing and multi-agent systems is to achieve overall system reliability in the presence of a number of faulty processes and often requires coordinating processes to reach consensus "agreement" on some data value that is needed during computation.

I enjoyed the work of Leslie lamport on part-time paliment "PAXOS"

### Applications of Distributed Consensus
1. Deciding whether to commit a distributed transaction to a database. 
2. Designating node as a leader for some distributed task. 
3. Synchronizing state machine replicas and ensuring consistency among them.

### Raft VS Paxos
Raft only allows servers with up-to-date logs to become leaders.
Paxos allows any server to be leader provided it then updates its log to ensure it is up-to-date.