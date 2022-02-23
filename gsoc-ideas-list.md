# Ideas List of DatenLord

## Concurrent Hashmap Bench Framework in Rust
Implement a concurrent hashmap benchmark framework which is used to test performance of a concurrent hashmap in Rust. The framework can test the performance of concurrent hashmap with different parameters.

Main functionalities：
- Different percentages of read, update, delete operations
- Different load factors
- Different numbers of concurrent threads
- Different key/value types

## RCU Library in Rust
Implement a userspace [RCU](https://liburcu.org/) library in Rust.

Prerequisite Knowledge:
- atomic operation
- memory model

## Epaxos Chaos Engineering Framework in Rust
Epaxos consensus protocol keeps cluster consistency even when some nodes fails. And Chaos Engineering test is one of the best practice to verify the correctness of the protocol implementation. We've implemented this protocol in Rust, so of source we need an Chaos Engineering framework.

Prerequisite Knowledge:
- Familiar with Rust language
- Epaxos (or Paxos/Raft) consensus protocol 
- Understand Chaos Engineering concept

## Rust RPC library on RDMA network
RDMA network is widely adopted in date centers for high performance network applications, and RPC is one of most used ways in the network communication. We've published a Rust RDMA lib, based on which a RPC lib is our next step. We can leverage this RPC library in the DatenLord cluster communication.

Prerequisite Knowledge:
- Familiar with Rust language
- Familiar with RDMA concept, familiar with RDMA lib is better
- Familiar with famous RPC libs, such as GPRC.
