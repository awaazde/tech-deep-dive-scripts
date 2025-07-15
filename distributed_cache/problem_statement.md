# Distributed Cache with Consistency

## Goal 
Build a distributed cache system that handles consistency across multiple nodes, similar to Redis Cluster or Memcached.

### Learning Objectives
- Understand distributed cache architecture patterns
- Implement cache consistency strategies
- Handle network partitions and node failures
- Experience trade-offs between consistency and availability

---

### Prerequisites
- Python 3.7+ installed
- Basic knowledge of networking and threading
- Text editor or IDE ready

#### The Challenge
"We're building a distributed cache system that needs to handle millions of requests per second across multiple servers. Our cache must remain consistent even when nodes fail or network partitions occur."

#### Key Problems to Solve
1. **Distribution**: How do we decide which node stores which data?
2. **Consistency**: How do we ensure all nodes have the same view of the data?
3. **Availability**: How do we handle node failures gracefully?
4. **Scalability**: How do we add/remove nodes without downtime?

#### Real-World Context
- Redis Cluster uses hash slots and eventual consistency
- Memcached uses client-side consistent hashing
- Cassandra uses consistent hashing with tunable consistency
